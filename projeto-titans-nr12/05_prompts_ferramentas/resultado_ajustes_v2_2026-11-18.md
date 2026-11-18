# Resultado dos ajustes v2 — 18/11/2026
**Prompt usado:** `prompt_lovable_ajustes_v2.md`
**Ferramenta informada pelo grupo:** Bolt.new. **Atenção:** o código entregue tem marcas da Lovable: o README manda "clicar em Publish no editor Lovable", o roadmap fala em "Lovable Cloud" e há integração Supabase no estilo Lovable. Confirmar qual ferramenta foi usada de fato antes de citar no artigo.
**Código revisado:** ZIP `sitev2-nr12-titanssolucoes.zip` (repositório `projeto-de-site`)
**Método:** leitura do código e comparação com a v1. Instalei as dependências e rodei `vitest`: **3 arquivos e 10 testes passaram**. Não rodei o build nem abri o site publicado.

---

## 1. Conferência item a item

| # | Pedido | Resultado | Situação |
|---|---|---|---|
| 1 | Leads: não perder quando o webhook está vazio | Lead sempre salvo na tabela `leads` (Supabase). Webhook enviado só se `URL_FORMULARIO_DESTINO` estiver preenchida. Falha do banco devolve erro "Fale pelo WhatsApp". **Notificação por e-mail não foi feita** (comentário no código: exige domínio de e-mail verificado) | Atendido, exceto o e-mail |
| 2 | Aceitar e-mail gratuito | Bloqueio removido; rótulo voltou a "E-mail"; campo `email_corporativo` (true/false) vai no pacote e no banco | Atendido |
| 3 | Honeypot sem erro | Preenchido: retorna sucesso sem salvar nem encaminhar. Teste cobre | Atendido |
| 4 | GA4 e Pixel só com ID | Scripts carregados em `__root.tsx` apenas se o ID existir; `dataLayer` mantido | Atendido |
| 5 | `SITE_URL` | Criado em `site.ts`, vazio; função `urlAbs()` em canonical e `og:url` das 3 páginas; sitemap usa o domínio quando preenchido | Atendido |
| 6 | Linha `Sitemap:` no robots | A linha ficou **comentada**, para descomentar à mão com o domínio; documentado no README | Parcial |
| 7 | Tela de erro em português | `error-page.ts` e a tela do `__root.tsx` traduzidas | Atendido |
| 8 | Logos no repositório | PNGs em `public/`; `Logo.tsx` aponta para eles | Atendido |
| 9 | README em português | Reescrito (rotas, configurações, `SITE_URL`, formulário). Ainda diz para publicar "no editor Lovable" | Atendido, com ressalva |
| 10 | Testes | Novo `lead-functions.test.ts` (honeypot, destino vazio, e-mail corporativo, falha do banco); `lead.test.ts` ajustado | Atendido |

## 2. Pontos de atenção

1. **Site fora do ar?** O `roadmap.md` abre com "Diagnosticar 404 no domínio publicado e republicar", e todas as caixas estão desmarcadas, embora o código mostre os itens feitos. Não sei se o site já está no ar. **Confirmar.**
2. **Política de privacidade ainda `[PREENCHER]`**, e agora o site guarda dados pessoais em banco. O texto precisa citar o armazenamento, a finalidade e o prazo de retenção. Continua bloqueando a publicação.
3. **Ninguém é avisado de novo lead.** Sem webhook e sem e-mail, o lead fica só no banco. Alguém da Titans precisa saber onde consultar, ou o webhook (Make, Zapier, CRM) deve ser ligado.
4. **Política do banco aceita inserção anônima** (`INSERT` para `anon` com `WITH CHECK (true)`). O servidor grava com a chave de serviço, então essa permissão não é necessária, e a chave anônima é pública. Na prática, qualquer pessoa poderia gravar linhas na tabela sem passar pela validação nem pelo honeypot. Recomendo remover.
5. **`encaminhado_webhook` é gravado antes do envio.** Se o webhook falhar, o lead fica marcado como encaminhado e a pessoa vê erro (pode reenviar e duplicar).
6. **GA4 e Pixel sem aviso de consentimento.** Carregam assim que o ID for preenchido. Decidir com a Titans se haverá banner de cookies (LGPD).
7. **robots.txt:** exige edição manual quando o domínio sair.
8. **Dependências com versão aberta** (`drizzle-kit` e `drizzle-orm` em `0.x`). Baixa prioridade.

## 3. Decisão do item 7 de `decisoes.md`
Resolvida na prática: o formulário aceita e-mail gratuito e marca o lead como "não corporativo" (decisão 8).

## 4. Próximo passo
Ajustes restantes em `prompt_lovable_ajustes_v3.md` (itens 4, 5 e 7 acima, mais atualização do roadmap).
