# Etapa 06 — Reposicionamento do site (NR-12)

**Status:** [x] desenvolvida (v1, 16/11/2026). Protótipo gerado na Lovable (repositório: https://github.com/guilhermelsilva23-cell/projeto-de-site), revisado pelo código. Pendente: dados da Titans, ajustes v2 e conferência visual.
**Entregáveis do PDF:** 09 (página da solução para o site) e 10 (protótipo visual da página)
**Onde estão os textos finais:** `05_prompts_ferramentas/prompt_lovable_site_nr12.md`, seção 3 (Página A). O protótipo visual é gerado pela ferramenta a partir desse prompt.
**Legenda:** **[F]** fato com fonte · **[H]** hipótese · `[PREENCHER]` dado que só a Titans tem

---

## 1. Diagnóstico do site atual (de Etapas 2 e 3)

| Problema | Origem | Como a nova página responde |
|---|---|---|
| NR-12 é 1 de 5 serviços, sem página própria | Etapas 2 e 3 | Página dedicada `/adequacao-nr-12` |
| Escopo descrito em 4 tópicos genéricos, sem inventário, validação e documentação | Etapa 3 | Seção de metodologia com 6 fases e entregas |
| Logos de clientes sem case com resultado | Etapa 3 | Seção de cases com estrutura fixa (só com autorização) |
| Conteúdo carregado por JavaScript, com possível problema de indexação [H] | Etapa 3 | Exigência de SSG/SSR no prompt; verificação pendente (ver Etapa 7) |
| Blog parado desde 22/10/2025 [reverificar] | Etapa 3 | Tratado na Etapa 9 (calendário) |

## 2. Estrutura da página (mínima do PDF + extras)

| # | Seção do PDF | Conteúdo | Persona que atende |
|---|---|---|---|
| 1 | Hero | H1, subtítulo, mídia, CTA "Solicite um diagnóstico NR-12" e "Envie sua RFQ" | Todas |
| 2 | Problema | Sua máquina está protegida e documentada? Dado: cerca de 15% dos acidentes de 2012 a 2022 envolvem máquinas [F5] | Decisora e Técnica |
| 3 | Solução Titans | Fluxo único e escada de 5 degraus | Decisora |
| 4 | Aplicações | Máquinas e setores (Etapa 2) | Técnica |
| 5 | Benefícios | 5 benefícios sem promessa percentual | Decisora |
| 6 | Tecnologias | Proteções, sensores, relés e normas (ISO 12100, 13849) | Técnica |
| 7 | Metodologia | 6 fases com "o que acontece" e "o que você recebe" | Técnica e Compras |
| 8 | Cases | 3 cards com estrutura fixa; `[PREENCHER]` | Decisora |
| extra | FAQ | 5 perguntas; alimenta SEO (Etapa 7) | Técnica |
| 9 | CTA | Diagnóstico, WhatsApp e RFQ | Todas |

## 3. Textos-chave

- **H1:** Adequação NR-12 de máquinas tratada como engenharia
- **Subtítulo:** Do diagnóstico ao laudo, em um só fluxo: inventário, apreciação de risco, projeto, adequação, validação e documentação, com responsável técnico e ART.
- **Frase da marca (Etapa 4, opção A):** Segurança de máquinas tratada como engenharia. A menção a "mestres e doutores" só entra após confirmação da Titans.
- **CTAs:** "Solicite um diagnóstico NR-12" (primário), "Envie sua RFQ" (secundário), "Fale com nossa engenharia" (WhatsApp).

## 4. Imagens e mídias necessárias (a produzir ou autorizar)

| Seção | Imagem | Origem sugerida |
|---|---|---|
| Hero | Máquina industrial com proteção instalada, ou vídeo curto (Etapa 10) | Foto/vídeo real da Titans `[PREENCHER]` |
| Problema | Ícones dos 3 riscos (esmagamento, corte, projeção) | Ícones próprios |
| Tecnologias | Cortina de luz, chave de segurança, relé | Fotos de componentes (checar direitos de uso) |
| Cases | Antes e depois | Fotos autorizadas `[PREENCHER]` |

## 5. Jornada até a RFQ

Google (busca por solução) ou LinkedIn (conteúdo técnico) → Página `/adequacao-nr-12` → CTA diagnóstico → Landing `/adequacao-nr-12/diagnostico` → formulário → qualificação por WhatsApp ou telefone → visita de diagnóstico → proposta por degrau → RFQ.
Quem já conhece a Titans e quer cotar entra pelo botão "Envie sua RFQ" (Persona 3). Detalhamento do funil: Etapa 14.

## 6. Decisões tomadas nesta etapa

1. **Duas páginas:** institucional (indexável, SEO) e landing (campanha, `noindex`) para evitar canibalização. [H]
2. **Ferramenta de criação:** o grupo gera o protótipo por prompt em ferramentas como Lovable. O código gerado não é entrega final sem revisão da Titans.
3. **Sem promessa quantitativa:** a página não usa o percentual de redução de acidentes nem valores de multa (ver Etapa 4, seção 5).

## 7. Regra principal do PDF aplicada à Etapa 6

- **Por quê:** a NR-12 está escondida no site e o escopo é genérico.
- **Para quem:** engenheiro de manutenção/segurança, gerente de planta e compras (Etapa 5).
- **Conteúdo:** fluxo de 6 fases, escada de valor, FAQ e cases.
- **Objetivo:** gerar pedidos de diagnóstico e RFQs.
- **Investimento:** produção da página e das fotos `[PREENCHER]`.
- **Destino:** landing do diagnóstico e formulário de RFQ.
- **Resultado esperado:** o diagnóstico passa a ser a principal conversão do site (medir na Etapa 16).

## 8. Pendências

- [x] Resultado da ferramenta registrado (`05_prompts_ferramentas/resultado_lovable_2026-11-16.md`)
- [ ] Enviar `prompt_lovable_ajustes_v2.md` e conferir o resultado
- [ ] Abrir o preview e conferir o protótipo no celular e no computador (a revisão foi só do código)
- [ ] Obter da Titans: cor exata da marca (logo já aplicado), WhatsApp, e-mail de RFQ, cidade/UF, domínio e texto da política de privacidade
- [ ] Obter cases e fotos autorizados
- [ ] Confirmar a equipe (mestres e doutores) e o que é feito internamente
- [ ] Revisar a página com um engenheiro da Titans (argumentos técnicos)
