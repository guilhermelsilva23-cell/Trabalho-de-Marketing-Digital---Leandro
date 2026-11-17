# Etapa 07 — Google e SEO (NR-12)

**Status:** [x] desenvolvida (v1, 16/11/2026) — **volumes de busca não coletados**. A prioridade abaixo é por intenção de busca [H] e deve ser confirmada no Google Keyword Planner.
**Entregáveis do PDF:** 11 (15 palavras-chave SEO) e 12 (estratégia Google)
**Lista completa e agrupamento por página:** `04_dados_e_evidencias/seo_palavras_chave.md`

---

## 1. O que o cliente digitaria no Google

Três momentos de busca, ligados às personas da Etapa 5:

| Momento | Exemplo de busca | Persona | Página que atende |
|---|---|---|---|
| Aprender | "o que é NR-12", "apreciação de risco de máquinas" | Técnica | Blog (Etapa 9) |
| Comparar | "empresa de adequação NR-12", "laudo NR-12 com ART" | Técnica e Decisora | `/adequacao-nr-12` |
| Contratar | "adequação NR-12 de prensa", "diagnóstico NR-12" | Decisora e Compras | `/adequacao-nr-12` e landing |

## 2. Palavras-chave (22) por prioridade [H]

Critério: **Alta** = intenção de contratar e aderência direta à oferta; **Média** = pesquisa de solução ou termo técnico; **Baixa** = busca informativa ampla, de pouca intenção de compra.

| Prioridade | Palavras-chave |
|---|---|
| **Alta (8)** | adequação NR-12 · empresa de adequação NR-12 · laudo NR-12 · adequação de máquinas NR-12 · adequação NR-12 de prensa · apreciação de risco de máquinas · adequação NR-12 de máquina importada · diagnóstico NR-12 |
| **Média (9)** | projeto de segurança de máquinas · inventário de máquinas NR-12 · laudo NR-12 com ART · cortina de luz NR-12 · consultoria NR-12 · adequação NR-12 de dobradeira · adequação NR-12 de injetora · NR-12 cobot · quanto custa adequação NR-12 |
| **Baixa (5)** | o que é NR-12 · NR-12 multa · norma NR-12 · curso NR-12 · treinamento NR-12 |

Observações:
- "NR-12 multa" atrai busca baseada em medo (hipótese H3 pede teste contra conteúdo técnico). Se usada, não citar valores sem conferir a tabela vigente da NR-28 (ver `fontes_e_validacao.md`).
- "Curso" e "treinamento" atraem público que não compra adequação. Servem só para autoridade de blog.
- Variações com cidade ("adequação NR-12 em [cidade]") dependem da região da Titans `[PREENCHER]`.

## 3. Elementos on-page da página principal

| Elemento | Proposta | Tamanho |
|---|---|---|
| URL | `/adequacao-nr-12` | — |
| Title | Adequação NR-12 de Máquinas \| Titans Engenharia | 47 caracteres |
| Meta description | Adequação NR-12 com engenharia: diagnóstico, apreciação de risco, projeto, validação e laudo com ART. Solicite um diagnóstico com a Titans. | 139 caracteres |
| H1 | Adequação NR-12 de máquinas tratada como engenharia | — |
| H2 | Sua máquina está protegida e documentada? · Um fluxo de engenharia, um responsável técnico · Máquinas e setores atendidos · O que você recebe · Como fazemos · Como a Titans conduz o projeto · Experiência comprovada · Perguntas frequentes | — |

**Landing do diagnóstico:** URL `/adequacao-nr-12/diagnostico`; title "Diagnóstico NR-12 de Máquinas | Titans Engenharia" (46 caracteres); meta description de 118 caracteres; `noindex, follow`. H1: "Sua máquina está em conformidade com a NR-12?"

## 4. Estratégia Google

| Frente | Ação | Observação |
|---|---|---|
| Indexação | Entregar conteúdo no HTML (SSG/SSR) e gerar sitemap | Possível falha atual de indexação por JavaScript [H], a verificar |
| Página-pilar | `/adequacao-nr-12` com FAQ e dados estruturados | Alvo: palavras de prioridade alta |
| Conteúdo de apoio | Artigos do blog sobre apreciação de risco, ISO 13849, máquina importada | Calendário na Etapa 9; links para a página-pilar |
| Google Meu Negócio | Criar ou revisar o perfil com serviço NR-12 | Depende da cidade/UF `[PREENCHER]` |
| Google Ads | Campanha de pesquisa nas palavras de prioridade alta, destino na landing | Orçamento de R$ 1.000 na Etapa 11 |
| Medição | Search Console e GA4 com eventos de formulário e WhatsApp | KPIs na Etapa 16 |

## 5. Como verificar o problema de indexação (de Etapa 3)

- [ ] Buscar `site:titanssolucoes.com.br` e contar as páginas indexadas
- [ ] Abrir "ver código-fonte" da home e checar se o texto aparece no HTML
- [ ] Inspecionar a URL no Search Console (precisa de acesso)

## 6. Regra principal do PDF aplicada à Etapa 7

- **Por quê:** concorrentes dominam busca local e por palavra-chave (Etapa 3).
- **Para quem:** quem pesquisa solução de NR-12 no Google.
- **Conteúdo:** página-pilar, FAQ e artigos de apoio.
- **Objetivo:** tráfego qualificado para o diagnóstico.
- **Investimento:** produção de conteúdo e ajustes técnicos; mídia na Etapa 11.
- **Destino:** página NR-12 e landing do diagnóstico.
- **Resultado esperado:** crescimento de cliques orgânicos e de pedidos de diagnóstico a partir do Google (medir no Search Console).

## 7. Pendências

- [ ] Rodar o Keyword Planner e anexar o CSV em `04_dados_e_evidencias`
- [ ] Reclassificar as prioridades com volume e concorrência
- [ ] Confirmar a cidade/UF para versões locais
- [ ] Verificar a indexação do site atual
