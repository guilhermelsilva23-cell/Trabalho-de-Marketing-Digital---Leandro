# Resultado da Lovable — 16/11/2026
**Ferramenta:** Lovable (projeto conectado ao GitHub)
**Repositório:** https://github.com/guilhermelsilva23-cell/projeto-de-site (revisado a partir do ZIP `projeto-de-site-main.zip`)
**Prompt usado:** `prompt_lovable_site_nr12.md`
**Método da revisão:** leitura do código-fonte. **Build, testes e site publicado não foram executados nem abertos**; o que está dito sobre aparência e funcionamento vem do código e precisa de conferência visual.

---

## 1. O que foi criado

| Item | Detalhe |
|---|---|
| Stack | TanStack Start (React + TypeScript) com SSR, Tailwind, componentes shadcn/ui; build para Cloudflare (via Lovable) |
| Rotas | `/` (redireciona 301 para `/adequacao-nr-12`), `/adequacao-nr-12`, `/adequacao-nr-12/diagnostico`, `/politica-de-privacidade`, `/sitemap.xml` |
| Configuração única | `src/config/site.ts` (contatos, webhook, analytics, `SHOW_CASE`); cores em `src/styles.css` (`--cor-*`) |
| Formulário | `src/lib/lead.ts` (validação com zod, usada no cliente e no servidor) e `src/lib/lead.functions.ts` (envio ao webhook) |
| Componentes | Logo, rodapé, botões, `MediaSlot` (espaço de imagem com legenda) e `Preencher` (marcador visível) |
| Testes | 4 testes do formulário e 1 de roteamento (não executados nesta revisão) |

## 2. Conferência com o prompt

| Item do prompt | Resultado | Situação |
|---|---|---|
| Página A: 10 seções, textos, H1, title e meta description | Textos e SEO idênticos ao prompt; FAQ com 5 perguntas; dado de 15% com fonte | Conforme |
| Landing: 7 blocos, `noindex, follow`, menu mínimo | Conforme; bloco de case oculto por `SHOW_CASE=false` | Conforme |
| Paleta preto, branco e vermelho em variáveis | `--cor-primaria: #E10600` (provisório), mais `--cor-primaria-escura: #B80500` para hover | Conforme (+ extra) |
| Logo como espaço reservado | Logos reais da Titans (branco e preto) aplicados | Melhor que o pedido, com ressalva (ver 3, item 8) |
| Fontes | Barlow e Barlow Condensed via Google Fonts | Conforme |
| SSG/SSR | SSR do TanStack Start; `head()` com meta e JSON-LD por rota | Conforme |
| JSON-LD | Organization e Service nas duas páginas; FAQPage só na Página A | Conforme (Organization só com nome e e-mail) |
| Sitemap e robots | `sitemap.xml` dinâmico (só páginas indexáveis); `robots.txt` liberando tudo | Parcial: robots sem a linha `Sitemap:` |
| Imagens com width/height | Sim, com `loading="lazy"` | Conforme |
| Marcadores `[PREENCHER]` | Componente `Preencher`; lista abaixo | Conforme |
| Config única | `src/config/site.ts` | Conforme |
| Formulário: campos, LGPD, UTMs ocultas, honeypot | Todos presentes | Conforme |
| Formulário: enviar ao webhook **e** ao e-mail | Só webhook; o e-mail vai dentro do pacote como `destino_email`, mas **nenhum e-mail é enviado** | Diferente |
| Eventos de análise | Os 5 eventos existem; `click_whatsapp` e `click_rfq` só na Página A | Parcial |
| Variáveis para GA4 e Meta Pixel | Existem, mas **nenhum script de GA4 ou Pixel é carregado** | Parcial |
| Link entre as duas páginas | Ida e volta presentes | Conforme |
| Política de privacidade | Página criada, com texto `[PREENCHER]` | Extra, incompleta |

## 3. Diferenças e riscos (ordem de prioridade)

1. **Lead pode se perder sem aviso.** Se `URL_FORMULARIO_DESTINO` estiver vazia (hoje está), o servidor só escreve um aviso no log e a pessoa vê "Recebemos sua solicitação". Antes de qualquer campanha, ligar o webhook (ou outro destino) e testar o envio de ponta a ponta.
2. **Rejeição de e-mail pessoal (gmail, hotmail etc.), que não estava no prompt.** O campo exige e-mail corporativo e bloqueia domínios gratuitos. A Persona 2 inclui o dono de PME metalmecânica (Etapa 5), que pode usar e-mail gratuito. Decisão em aberto (ver `decisoes.md`).
3. **Analytics não funcionam só preenchendo o ID.** `track()` só dispara se `window.gtag` ou `window.fbq` já existirem, e o código não carrega esses scripts. Sem isso, a Etapa 16 (KPIs) fica sem dados.
4. **Canonical e `og:url` relativos** (`/adequacao-nr-12`). O ideal é URL absoluta com o domínio, que ainda não existe no projeto.
5. **`robots.txt` sem a linha `Sitemap:`.**
6. **Tela de erro do template em inglês** ("This page didn't load"). A tela 404 está em português.
7. **Honeypot:** o schema rejeita o campo preenchido antes do trecho que "finge sucesso" para robôs, então o robô recebe erro. Efeito prático pequeno.
8. **Logos só no armazenamento da Lovable.** O repositório guarda apenas arquivos `.asset.json` apontando para `/__l5e/assets-v1/...`. Em outra hospedagem, o logo pode não carregar. Guardar os PNGs originais no projeto.
9. **README ainda é de rascunho** ("espere eu mandar a outra parte do prompt").

## 4. Marcadores `[PREENCHER]` que seguem abertos

| Onde | O que falta |
|---|---|
| `src/config/site.ts` | WHATSAPP_NUMERO, EMAIL_RFQ, CIDADE_UF, ENDERECO, URL_FORMULARIO_DESTINO, PRAZO_RETORNO, GA4_ID, META_PIXEL_ID |
| Página A, seção Cases | Logos autorizados e 3 cases (setor, máquina, desafio, o que foi feito, resultado) |
| Página A, mídias | Vídeo/foto do hero, 2 fotos de aplicação, 3 fotos de case |
| Landing | Confirmação de "responsável técnico e ART", preço do diagnóstico, escopo e prazo, case autorizado |
| Rodapé | Endereço, cidade/UF, WhatsApp e e-mail (aparecem como marcador enquanto vazios) |
| Política de privacidade | Texto completo (controlador, finalidade, base legal, retenção, direitos do titular, encarregado). **Bloqueia a publicação**, pois o formulário linka para ela |

## 5. Antes de publicar

- [ ] Ligar e testar o destino dos leads
- [ ] Texto da política de privacidade fornecido pela Titans
- [ ] Domínio definido, com canonical e Sitemap ajustados
- [ ] Revisão do conteúdo técnico por engenheiro da Titans (inclui a frase sobre relé, ver `fontes_e_validacao`)
- [ ] Dados reais de contato e cor exata da marca
- [ ] Conferir o site no celular e no computador (não feito aqui)

Os ajustes de código estão em `prompt_lovable_ajustes_v2.md`.
