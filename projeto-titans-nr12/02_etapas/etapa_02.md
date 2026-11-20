# Etapa 2 — Pesquisa de mercado (NR-12)

**Status:** [x] desenvolvida (v3, 19/11/2026) — v2 revisada com a entrevista do professor (10/11) e a validação de 12/11. Dados quantitativos de mercado ainda em coleta.
**Entregável do PDF:** 03 (Pesquisa de mercado / Mapa do Mercado da Solução)
**Legenda:** **[F]** fato com fonte · **[E]** relato de especialista (códigos E01…E18 em `04_dados_e_evidencias/entrevista_professor_leandro.md`) · **[H]** hipótese · **[S]** simulação · **[L]** lacuna
**Fontes:** códigos `[F1]`… em `00_gestao/fontes_e_validacao.md`.

---

## 1. Resumo do mapa

O mercado da NR-12 é **obrigatório por norma** e **concentrado em quem opera máquinas com risco de lesão grave**. A norma vale para máquinas novas e usadas [F10], e proíbe importar ou comercializar máquina que não a atenda (item 12.15.2) [F10]. A demanda existe, mas é **reativa**: a adequação costuma vir após acidente ou com o risco já identificado [E05], e o principal concorrente da Titans pode ser a decisão de adiar [E14] (H5). Na carteira do professor, a maioria dos projetos é de máquina velha em processo de custo baixo [E03], dentro de um raio de até ~200 km do centro de SP [E01]. A concorrência é numerosa e, em geral, comunica multa e obrigação; poucos mostram jornada completa ou prova de resultado. A oportunidade está em ligar diagnóstico, projeto, validação e documentação em uma oferta de engenharia com **responsável técnico comprovado** e casos de risco resolvido.

---

## 2. Demanda e contexto

| Indicador | Dado | Tipo | Fonte |
|---|---|---|---|
| Acidentes de trabalho (CAT) em 2022 | 612,9 mil | [F] | [F5][F12] |
| Participação de máquinas e equipamentos (2012–2022) | cerca de 15% (14,8% em outra fonte) | [F] | [F5][F13] |
| Acidentes típicos com agente exclusivo "máquinas e equipamentos" em 2021 | 60.979 | [F] | [F16] |
| Gravidade | Máquinas causam amputações e lesões graves com frequência maior que as demais causas | [F] | [F5] |
| Campanha nacional do MTE (CANPAT 2024), tema Segurança em Máquinas e Equipamentos, lançada em 18/04/2024 | Validada | [F] | [F16] |
| Notificações em 2023 | cerca de 732 mil (base possivelmente diferente; não misturar com 2022) | [F] com ressalva | [F6] |
| Alcance da norma | Máquinas novas e usadas (12.1.2) | [F] | [F10] |
| Importação de máquina fora da norma | Proibida (12.15.2) | [F] | [F10] |
| Exceções ao alcance | Máquina certificada pelo Inmetro com requisitos de segurança atendidos e máquina exclusivamente para exportação não se sujeitam à NR-12 (12.1.3 e 12.1.4 "f") | [F] | [F10] |
| Atualização das tabelas de infração da NR-28 em 2026, incluindo a NR-12 | Portaria MTE nº 1.758/2026 (30/09/2026) | [F] | [F19] |
| Participação da China nas importações de máquinas | 16,6% (2015); 32% (2025); 36% (jan–ago/2026, US$ 8,0 bi) | [F] com ressalva: fonte setorial interessada (ABIMAQ via imprensa) | [F21] |
| Importados no consumo nacional de máquinas | ≈ 47,7% no 1º semestre de 2026 | [F] com a mesma ressalva | [F21] |
| Tamanho do mercado em R$ | Desconhecido | [L] | Método na seção 10.1 |

**Uso nas peças:** o dado de ~15% e o de 60.979 são os mais fortes. Os dados de importação mostram **aumento da importação, não falta de adequação**.

---

## 3. Setores compradores

**Filtro geográfico antes da nota:** só entram plantas dentro de ~200 km do centro de SP [E01]. Fora disso, só projeto de faturamento expressivo (ex.: célula robótica) [E02]. A Titans não deve prometer atendimento nacional.

A priorização abaixo é **hipótese do grupo [H]**, com nota de 1 a 5. **As notas não foram alteradas nesta versão, mas C3 (capacidade de pagar) pode estar superestimado:** o professor diz que a maioria dos projetos é de clientes em processo de custo baixo [E03]. Revisar após o SAM (seção 10.1).

| Critério | Pergunta |
|---|---|
| C1 Densidade de risco | O setor usa muitas máquinas com esmagamento, corte ou projeção? |
| C2 Pressão externa | Há auditoria de cliente, seguradora ou sindicato que cobra conformidade? |
| C3 Capacidade de pagar | O ticket cabe no orçamento típico? |
| C4 Aderência à Titans | Casa com a engenharia que a Titans já faz? |
| C5 Acesso | É fácil alcançar o decisor por LinkedIn, Google ou indicação? |

| Setor | C1 | C2 | C3 | C4 | C5 | Total [H] | Prioridade | Máquinas típicas |
|---|---|---|---|---|---|---|---|---|
| Autopeças | 5 | 5 | 4 | 4 | 4 | 22 | Alta | Prensas, células de soldagem, injetoras |
| Automotivo | 4 | 5 | 5 | 5 | 3 | 22 | Alta | Células robotizadas, transportadores |
| Metalúrgico | 5 | 3 | 3 | 4 | 4 | 19 | Alta | Prensas, dobradeiras, guilhotinas, serras |
| Bens de capital | 4 | 3 | 4 | 5 | 4 | 20 | Média-alta | Máquinas especiais |
| Alimentos e bebidas | 4 | 4 | 4 | 3 | 3 | 18 | Média-alta | Embaladoras, esteiras |
| Plásticos | 4 | 3 | 3 | 3 | 3 | 16 | Média | Injetoras, extrusoras |
| Logística | 3 | 3 | 3 | 4 | 3 | 16 | Média | Transelevadores, AGVs |
| Farmacêutico | 3 | 4 | 5 | 2 | 2 | 16 | Baixa/validar | Envase, embalagem |

**Segmento transversal (PMEs metalmecânicas):** a NR-12 não traz isenção geral para ME/MEI; há tratamentos pontuais (12.13.5.3 e 12.16.3.1) [F10]. A NR-01 (item 1.8) dispensa o MEI de PGR, o que não alcança a empresa contratante [F17]. **[H]** sobre o efeito no ticket e na sensibilidade a preço.

---

## 4. Principais aplicações

1. Prensas, dobradeiras e guilhotinas
2. Serras de corte, inclusive de perfil extrudado (caso em andamento, [E04])
3. Células robotizadas e cobots (ISO 10218 e ISO/TS 15066 como referência técnica)
4. Esteiras, embaladoras e injetoras
5. Transelevadores, AGVs/AMRs e empilhadeiras
6. **Máquinas antigas** em processo de custo baixo (maioria dos projetos da carteira, [E03])
7. **Máquinas importadas**, inclusive chinesas (casos já adequados, [E04][E10]; hipótese H1)
8. Máquinas sem documentação técnica (reconstituição de manual e diagrama)

---

## 5. Segmento "máquinas importadas" — o que se sabe e o que falta

**Hipótese H1:** há demanda relevante por adequação NR-12 em máquinas importadas.
**Status (v3):** apoio qualitativo [E10][E12][E15] e de contexto [F21] (China 32% das importações em 2025; 36% em jan–ago/2026). **Falta** evidência de que máquinas importadas chegam sem adequação: o Comex Stat não prova isso; casos documentados da Titans e relatos externos provam.

| O que já se sabe | Tipo | Fonte |
|---|---|---|
| A Titans já adequou máquina importada; dificuldades: esquemas elétricos em mandarim e falta de acesso ao código-fonte do CLP; contorno com IHM e CLP de segurança separados | [E] a documentar | E10 |
| Nos últimos 2 anos, todos os clientes do professor importam | [E] vale só para a carteira dele | E12 |
| Importar compensa para mecânica simples; fabricante nacional ou representante vale para equipamentos problemáticos que exigem garantia | [E] | E15 |
| Clientes que importam tratam o fornecedor como segredo competitivo (alguns removem a etiqueta) | [E] | E13 |
| Existem normas técnicas chinesas de segurança de máquinas (ex.: GB/T 8196-2018, GB/T 18831), inclusive compulsórias; não há como afirmar nada sobre fiscalização | [F] | F20 |
| Manual e inscrições em português (12.13.2 e 12.12.4); projeto do sistema de segurança em português pode ser exigido (12.5.17) | [F] | F10 |

**Não usar:** "a China não tem norma equivalente" (E11, corrigido em 12/11/2026).

| Passo | Fonte/método | Situação |
|---|---|---|
| 1 | Comex Stat (MDIC), NCM 84 e 85, por ano e país de origem | [L] não coletado |
| 2 | Cruzar com os setores da seção 3 | Depende do passo 1 |
| 3 | ~~5 a 8 entrevistas com compradores de importadas~~ | **Inviável como planejado** [E13]. Substituído por: profissionais de SST/manutenção fora da carteira do professor, pesquisa anônima e simulação [S] (Etapa 5, seção 5; decisão 14) |
| 4 | Keyword Planner e Trends: "adequação NR-12 máquina importada", "máquina chinesa NR-12" | [L] não coletado |
| 5 | Casos da Titans (vídeos, ficha, autorização escrita) | Pendente com o professor |

**Decisão provisória (proposta 11 em `00_gestao/decisoes.md`):** enquanto H1 não tiver evidência de falta de adequação, "máquinas importadas" é **campanha dentro da oferta geral**, e não o recorte único do projeto. Se o grupo aceitar, a decisão 1 e a pergunta central em `hipoteses_de_pesquisa.md` precisam ser revistas.

---

## 6. Concorrência (resumo; detalhe na Etapa 3)

| Grupo | Exemplos citados | Observação |
|---|---|---|
| Engenharias especializadas em NR-12 | Prisma (SP), EMSEG, Engenharia Adequada, Engehall, ES Engenharia, Ibuma | Prisma: diagnóstico gratuito via WhatsApp e SEO local (rascunho); a Titans pratica modelo híbrido (R$ ~200 ou isento) [E08]. As quatro últimas não foram analisadas |
| Integradores/automação com NR-12 como serviço lateral | TechPlus, Grupo Atex, Tesla Automação, Garcia Automação | Benchmarkados na Etapa 3 |
| Distribuidores de componentes | Sulfran | Componentes e treinamento |
| Sebraetec | Consultoria subsidiada | A ficha do Sebrae MG limita a consultoria à documentação técnica, diagnóstico de conformidade e treinamento, sem adequação física [F15]; o edital nacional inclui identificação de necessidades e ART [F9]. Escrever: "**não inclui a adequação física**" |
| Fabricantes de componentes e de máquinas | — | Hipótese: oferecem engenharia junto com o produto [H] |
| **A decisão de adiar** | — | Concorrente principal segundo o professor: cliente que aprovou melhorias e não executou por 3 anos [E14] (H5) |

**Padrão observado:** foco em multa e obrigação; diagnóstico gratuito e SEO local (Prisma); discurso "NR-12 como engenharia" existe, mas sem jornada nem prova (leitura do grupo, a confirmar na Etapa 3).

---

## 7. Tendências e tecnologias

- Cobots e a ISO 10218 / ISO/TS 15066 como referência de segurança
- Scanners a laser para AGVs e AMRs
- CLPs e módulos de segurança integrados ao controle da máquina
- Atualização das tabelas de infração da NR-28 em 2026; a Portaria MTE nº 1.758/2026 inclui a NR-12 [F19]
- Aumento da importação de máquinas, com a China à frente [F21]
- Documentação técnica em meio digital [H] (sem portaria comprovada)
- Segurança associada a dados e Indústria 4.0 [H]

---

## 8. Oportunidades

1. **Ligar laudo a execução:** muitos concorrentes são fortes em um dos lados. A Titans pode vender o fluxo completo, com ART [F10, 12.5.2 "b"].
2. **Diagnóstico como porta de entrada**, com escopo fechado e prazo curto.
3. **Enquadramento inicial:** o diagnóstico começa verificando se a máquina está no alcance da norma (Inmetro, exportação), para não vender adequação onde não há obrigação [F10].
4. **Casos de risco resolvido** (máquinas chinesas, pós-mutilação com atuação do MTE, serra em andamento [E04]), enquadrados como "risco resolvido", não "sucesso" [E05]. Dependem de material e autorização escrita.
5. **Prova social:** os clientes do site (Bombril, Cargill, CCR, CGR, DGS) **não foram confirmados como clientes de NR-12**; não usar como case de NR-12.
6. **Mensagem para quem já conhece o risco e adia** (inércia) [E14].
7. **Máquinas importadas** como segmento com mensagem própria, sustentada por 12.15.2 (a comprovar a demanda).
8. **Parcerias** com escritórios de SST, ABIMAQ e Sebrae.

## 9. Ameaças

| # | Ameaça | Mitigação proposta |
|---|---|---|
| 1 | Concorrentes com busca local forte e diagnóstico gratuito | Entregável claro no diagnóstico; conteúdo técnico profundo |
| 2 | NR-12 percebida como custo e "papel" | Mensagem de engenharia; decisão baseada em risco priorizado |
| 3 | **Inércia:** o cliente identifica o risco e adia [E14] | Mensagem M3; gatilho "risco já identificado" (Etapa 12) |
| 4 | **Compra reativa:** só depois de acidente [E05] | Conteúdo para quem já tem o risco mapeado; não depender de campanha de medo (H3) |
| 5 | **Capacidade:** um só responsável técnico assina tudo [E06] | Medir antes de escalar a mídia; limite de projetos/mês |
| 6 | **Raio geográfico:** fora de ~200 km o deslocamento não compensa [E01][E02] | Geosegmentação (Etapa 11); não prometer atendimento nacional |
| 7 | **Clientes chegam por indicação** [E16]; o canal digital ainda não existe | Baseline = ~5 projetos em 12 meses [E07]; medir leads novos separados da indicação |
| 8 | Simplificação do texto em 2019 [F4] e fiscalização irregular | Não prometer urgência regulatória sem fonte |
| 9 | Risco de reputação e responsabilidade técnica | Escopo contratual claro; ART; revisão por engenheiro habilitado |
| 10 | Diluição da marca: NR-12 é 1 de 5 serviços no site atual | Página e landing dedicadas (Etapas 6 e 13) |

---

## 10. Lacunas e plano de coleta

| Lacuna | Situação (19/11/2026) | Método | Prioridade |
|---|---|---|---|
| Tamanho do mercado em R$ | [L] | Seção 10.1 | Alta |
| Região de atuação | **Respondida [E01–E03]:** SP capital e interior, até ~200 km | Confirmar com mapa das cidades dos últimos projetos | Média |
| Preço dos concorrentes | [L] | Pedido de orçamento simulado, identificando-se como estudante | Alta |
| Preço da Titans | Parcial [E08][E09]; prazo não respondido | Propostas reais anonimizadas | Alta |
| Demanda por máquinas importadas | Apoio qualitativo e de contexto; falta Comex Stat | Seção 5 | Alta |
| Volume de busca | [L] | Keyword Planner (`seo_palavras_chave.md`) | Alta |
| Capacidade (projetos/mês) | [L] | Pergunta 13 de `perguntas_abertas.md` | Alta |
| Valor vigente das multas em 2026 | A VALIDAR | Anexo I da NR-28, fonte primária | Média |

### 10.1 Como estimar o tamanho do mercado

| Camada | Definição | Fórmula | Insumos |
|---|---|---|---|
| **TAM** | Plantas industriais nos setores-alvo no Brasil | nº de estabelecimentos × % com máquinas de risco | IBGE (PIA), RAIS, CNAE |
| **SAM** | Plantas dentro de ~200 km do centro de SP [E01] | TAM × % localizado no raio × % no porte-alvo | RAIS/CNAE por município |
| **SOM** | Parte capturável em 12 meses | SAM × taxa de conversão do funil, **limitada pela capacidade de um responsável técnico** [E06] | KPIs das Etapas 14 e 16 |

Referências já conhecidas, **todas [E] e não publicáveis**: ~5 projetos de NR-12 em 12 meses [E07]; ticket de ~R$ 8 mil por serra pequena e até ~R$ 20 mil nas maiores [E09]. Receita potencial = SOM × ticket. Todo valor é **estimativa**, com as premissas à vista. Regra de sanidade: se o SOM passar da capacidade de entrega, o gargalo é a entrega, não a demanda.

---

## 11. Ideias de ação, no formato "por quê → para quem → ..."

| Ideia | Por quê | Para quem | Conteúdo | Objetivo | Investimento | Destino | Resultado esperado |
|---|---|---|---|---|---|---|---|
| Vídeo curto por tipo de máquina | Mostrar o risco real na máquina do cliente | Engenheiros de manutenção/processos (SP e raio de ~200 km) | "Os 3 riscos mais comuns em [prensa/serra/embaladora]" | Interesse e visitas à página | Produção interna | Página NR-12 | Visualizações, cliques, pedidos de diagnóstico |
| Conteúdo sobre importadas | Dor real e pouco coberta pelos concorrentes | Gestores e manutenção de quem importa | Esquema em mandarim, CLP sem código-fonte, IHM e CLP de segurança separados [E10] | Autoridade técnica | Produção interna; depende da autorização do professor | Blog e landing | Leitura e pedidos de diagnóstico de importadas |
| Caso de risco resolvido | Prova sem chamar de "sucesso" [E05] | Decisor | Ficha: setor, máquina, risco, ação, resultado | Confiança | Vídeos do professor | Página e apresentação comercial | Conversas comerciais |
| Anúncios geosegmentados | Alcançar o decisor na área atendida | Donos de PME e gerentes de planta, SP e raio de ~200 km | Oferta de diagnóstico; mensagem de inércia | RFQs | R$ 1.000 (Etapa 11) | Landing do diagnóstico | Custo por lead e por RFQ |
| Eventos de SST | Autoridade e conexões | Gestores, SST, ABIMAQ | Palestra técnica | Networking | `[PREENCHER]` | Contato direto | Leads qualificados |

---

## 12. Regra principal do PDF aplicada à Etapa 2

A pesquisa só serve se alimentar **para quem** (setores no raio de ~200 km e as três personas), **com qual conteúdo** (risco por máquina, importadas, risco resolvido), **levando o cliente para onde** (diagnóstico) e **esperando qual resultado** (mais pedidos de diagnóstico do que o baseline de ~5 projetos em 12 meses, a medir na Etapa 16).

## 13. Pendências

- [ ] Rodar o Comex Stat (NCM 84 e 85) e anexar em `04_dados_e_evidencias`
- [ ] Rodar o Keyword Planner e anexar o CSV (Etapa 7)
- [ ] Estimar TAM/SAM/SOM (seção 10.1) com o raio de ~200 km
- [ ] Revisar as notas de setor (C3) após o SAM
- [ ] Pedir ao professor: cidades dos últimos 5 projetos, prazo e capacidade
- [ ] Obter o valor vigente das multas (Anexo I da NR-28)
- [ ] Substituir fontes secundárias (ABIMAQ via imprensa, portais) por Comex Stat e DOU para o artigo
