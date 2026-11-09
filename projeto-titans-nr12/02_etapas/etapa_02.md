# Etapa 2 — Pesquisa de mercado (NR-12)

**Status:** [x] desenvolvida (v2, 09/11/2026) — dados quantitativos de mercado ainda em coleta
**Entregável do PDF:** 03 (Pesquisa de mercado / Mapa do Mercado da Solução)
**Legenda:** **[F]** = fato com fonte · **[H]** = hipótese a validar · **[L]** = lacuna de dado
**Fontes:** códigos `[F1]`… em `00_gestao/fontes_e_validacao.md`.

---

## 1. Resumo do mapa

O mercado da NR-12 é **obrigatório por norma** e **concentrado em quem opera máquinas com risco de lesão grave**. A norma vale para máquinas novas e usadas [F3][F4]. A demanda existe, mas é frequentemente percebida como custo. A concorrência é numerosa, em geral comunica multa e obrigação, e poucos mostram jornada completa ou prova de resultado. A oportunidade da Titans está em ligar diagnóstico, projeto, validação e documentação em uma oferta de engenharia com prova social.

---

## 2. Demanda e contexto

| Indicador | Dado | Tipo | Fonte |
|---|---|---|---|
| Acidentes de trabalho (CAT) em 2022 | 612,9 mil | [F] | Observatório SST/SmartLab [F5] |
| Participação de máquinas e equipamentos nos acidentes (2012–2022) | cerca de 15% | [F] | [F5] |
| Gravidade | Operação de máquinas causa amputações e lesões graves com frequência muito maior que as demais causas; mais acidentes fatais que a média | [F] | [F5] |
| Notificações em 2023 | cerca de 732 mil, com 2,8 mil mortes (base possivelmente diferente; não misturar com 2022) | [F] com ressalva | [F6] |
| Alcance da norma | Máquinas novas e usadas | [F] | [F3][F4] |
| Texto de 2019 | Simplificou exigências (ex.: reconhecimento de ISO 13849, manual NBR 16746); a CNI sustenta que sem reduzir a segurança | [F] | [F4] |
| NR-28 alterada em 2026, com atualização do Anexo II (códigos de infração, inclusive da NR-12) | Em vigor | [F] | [F8] |
| Campanha nacional do MTE sobre segurança em máquinas em 2024 | Citada no rascunho | [H] | Sem fonte localizada. Validar antes de usar |
| Tamanho do mercado em R$ | Desconhecido | [L] | Método na seção 10.1 |

**Uso nas peças:** o dado de 15% é forte e verificável. Para 2023, usar a base do Observatório quando atualizada.

---

## 3. Setores compradores

A priorização é **hipótese do grupo [H]**, com critério explícito e nota de 1 a 5. As notas são provisórias e devem ser validadas com a Titans e com dados (RAIS, PIA, Comex Stat).

| Critério | Pergunta |
|---|---|
| C1 Densidade de risco | O setor usa muitas máquinas com esmagamento, corte ou projeção? |
| C2 Pressão externa | Há auditoria de cliente, seguradora ou sindicato que cobra conformidade? |
| C3 Capacidade de pagar | O ticket de diagnóstico e adequação cabe no orçamento típico? |
| C4 Aderência à Titans | Casa com a engenharia que a Titans já faz? |
| C5 Acesso | É fácil alcançar o decisor por LinkedIn, Google ou eventos? |

| Setor | C1 | C2 | C3 | C4 | C5 | Total [H] | Prioridade | Máquinas típicas |
|---|---|---|---|---|---|---|---|---|
| Autopeças | 5 | 5 | 4 | 4 | 4 | 22 | Alta | Prensas, células de soldagem, injetoras |
| Automotivo | 4 | 5 | 5 | 5 | 3 | 22 | Alta | Células robotizadas, transportadores |
| Metalúrgico | 5 | 3 | 3 | 4 | 4 | 19 | Alta | Prensas, dobradeiras, guilhotinas |
| Bens de capital | 4 | 3 | 4 | 5 | 4 | 20 | Média-alta | Máquinas especiais |
| Alimentos e bebidas | 4 | 4 | 4 | 3 | 3 | 18 | Média-alta | Embaladoras, esteiras |
| Plásticos | 4 | 3 | 3 | 3 | 3 | 16 | Média | Injetoras, extrusoras |
| Logística | 3 | 3 | 3 | 4 | 3 | 16 | Média | Transelevadores, AGVs |
| Farmacêutico | 3 | 4 | 5 | 2 | 2 | 16 | Baixa/validar | Envase, embalagem |

**Segmento transversal:** PMEs metalmecânicas. A NR-12 não isentaria microempresa nem MEI (informação do rascunho; **conferir no texto da NR-12/NR-01**), o que amplia o mercado potencial, mas reduz o ticket e aumenta a sensibilidade a preço. [H]

---

## 4. Principais aplicações

1. Prensas, dobradeiras e guilhotinas
2. Células robotizadas e cobots (ISO 10218 e ISO/TS 15066 como referência técnica)
3. Esteiras, embaladoras e injetoras
4. Transelevadores, AGVs/AMRs e empilhadeiras
5. Máquinas importadas sem adequação (hipótese central, seção 5)
6. Máquinas antigas sem documentação (reconstituição de manual e diagrama)

---

## 5. Segmento "máquinas importadas" — plano para comprovar a hipótese

**Hipótese H1:** há demanda relevante por adequação NR-12 em máquinas importadas. **Status: não comprovada.**

| Passo | Fonte/método | O que mede |
|---|---|---|
| 1 | Comex Stat (MDIC): importações dos capítulos de máquinas (NCM 84 e 85), por ano e país de origem | Volume, valor e tendência |
| 2 | Cruzar com os setores da seção 3 | Onde está o risco de máquina sem adequação |
| 3 | 5 a 8 entrevistas com engenheiros e gestores industriais | Se compram importadas, quem adequa, quanto pagam, o que os trava |
| 4 | Google Keyword Planner e Trends: "adequação NR-12 máquina importada", "máquina chinesa NR-12" | Intenção de busca |
| 5 | Casos da Titans | Prova interna |

**Cuidado de método:** importação alta **não prova** falta de adequação. Só as entrevistas e os casos da Titans provam isso.

**Decisão provisória (ver `00_gestao/decisoes.md`, nº 3):** enquanto H1 não for comprovada, "máquinas importadas" é **campanha dentro da oferta geral**, e não o recorte único do projeto.

---

## 6. Concorrência (resumo; detalhe na Etapa 3)

| Grupo | Exemplos citados | Observação |
|---|---|---|
| Engenharias especializadas em NR-12 | Prisma (SP), EMSEG, Engenharia Adequada, Engehall, ES Engenharia, Ibuma | Prisma é a mais parecida com a porta de entrada proposta; as quatro últimas ainda não foram analisadas a fundo |
| Integradores/automação com NR-12 como serviço lateral | TechPlus, Grupo Atex, Tesla Automação, Garcia Automação | Benchmarkados na Etapa 3 |
| Distribuidores de componentes | Sulfran | Componentes e treinamento |
| Sebraetec | Consultoria subsidiada | O rascunho diz "faz só documentação", mas o edital localizado lista também identificação de necessidades de adequação e emissão de ART [F9]. **Reavaliar a afirmação** |
| Fabricantes de componentes e de máquinas | — | Hipótese: oferecem engenharia junto com o produto [H] |

**Padrão de posicionamento observado:** foco em multa e obrigação; diagnóstico gratuito via WhatsApp e SEO local (Prisma); discurso "NR-12 como engenharia" existe, mas sem jornada nem prova (leitura do grupo, a confirmar na Etapa 3).

---

## 7. Tendências e tecnologias

- Cobots e a ISO 10218 / ISO/TS 15066 como referência de segurança
- Scanners a laser para AGVs e AMRs
- CLPs e módulos de segurança integrados ao controle da máquina
- Atualização dos códigos de infração da NR-12 na NR-28 (2026) [F8]
- Documentação técnica em meio digital [H] (sem portaria comprovada; ver correção na Etapa 1)
- Segurança associada a dados e Indústria 4.0 [H]

---

## 8. Oportunidades

1. **Ligar laudo a execução:** muitos concorrentes são fortes em um dos lados (laudo ou instalação). A Titans pode vender o fluxo completo.
2. **Diagnóstico como porta de entrada**, com escopo fechado e prazo curto.
3. **Nicho NR-12 em automação e robótica**, integrado ao restante da engenharia da Titans.
4. **Segurança embarcada para fabricantes de máquinas** (B2B de segunda ordem).
5. **Prova social real:** clientes citados no site (Bombril, Cargill, CCR, CGR, DGS), **desde que a Titans autorize** o uso como case de NR-12.
6. **Parcerias** com escritórios de SST, ABIMAQ e Sebrae.
7. **Máquinas importadas** como segmento com mensagem própria (a comprovar).

## 9. Ameaças

| # | Ameaça | Mitigação proposta |
|---|---|---|
| 1 | Concorrentes com busca local forte e diagnóstico gratuito | Diagnóstico com escopo e entrega claros; conteúdo técnico profundo |
| 2 | NR-12 percebida como custo e "papel" | Mensagem de engenharia; decisão baseada em risco priorizado |
| 3 | Simplificação de exigências em 2019 [F4] | Não prometer urgência regulatória sem fonte |
| 4 | Fabricantes oferecendo adequação junto com o produto | Foco em máquinas usadas, importadas e integração |
| 5 | Fiscalização irregular reduz urgência de compra | Argumento de segurança e continuidade operacional |
| 6 | Risco de reputação e responsabilidade técnica em acidente com máquina adequada | Escopo contratual claro; ART; revisão por engenheiro habilitado |
| 7 | Diluição da marca: NR-12 é 1 de 5 serviços no site atual | Página e landing page dedicadas (Etapas 6 e 13) |

---

## 10. Lacunas e plano de coleta

| Lacuna | Fonte | Método | Prioridade |
|---|---|---|---|
| Tamanho do mercado em R$ | IBGE (PIA), RAIS, Comex Stat, ABIMAQ | Seção 10.1 | Alta |
| Preço dos concorrentes | Pedido de orçamento simulado, propostas públicas | Coleta direta | Alta |
| Região de atuação da Titans | Professor | Pergunta | Alta |
| Demanda por máquinas importadas | Comex Stat + entrevistas | Seção 5 | Alta |
| Volume de busca | Keyword Planner, Trends | Coleta (Etapa 7) | Média |
| Campanha MTE 2024 | gov.br | Localizar a fonte ou retirar | Baixa |

### 10.1 Como estimar o tamanho do mercado

Sem inventar número, a estimativa usa três camadas, a preencher com dados públicos:

| Camada | Definição | Fórmula | Insumos |
|---|---|---|---|
| **TAM** | Plantas industriais nos setores-alvo no Brasil | nº de estabelecimentos × % com máquinas de risco | IBGE (PIA), RAIS, CNAE dos setores da seção 3 |
| **SAM** | Parte atendível pela Titans (região e porte) | TAM × % na região de atuação × % no porte-alvo | Região da Titans `[PREENCHER]` |
| **SOM** | Parte capturável em 12 meses | SAM × taxa de conversão do funil | KPIs das Etapas 14 e 16 |

Receita potencial = SOM × ticket médio do degrau 1 (Etapa 4) `[PREENCHER]`. Todo valor deve ser rotulado como **estimativa**, com as premissas à vista.

---

## 11. Ideias de ação (do rascunho), no formato "por quê → para quem → ..."

| Ideia | Por quê | Para quem | Conteúdo | Objetivo | Investimento | Destino | Resultado esperado |
|---|---|---|---|---|---|---|---|
| Vídeo curto por setor | Mostrar risco real na máquina do setor do cliente | Engenheiros de manutenção/processos | "Os 3 riscos mais comuns em [prensa/embaladora]" | Gerar interesse e visitas à página | Produção interna | Página NR-12 | Visualizações, cliques, pedidos de diagnóstico |
| Eventos e congressos de NR-12 | Construir autoridade e conexões | Gestores, SST, ABIMAQ | Palestra técnica | Networking e leads | `[PREENCHER]` | Contato direto / RFQ | Leads qualificados |
| Anúncios (Google/LinkedIn) | Alcançar quem procura a solução ou decide | Donos de PME, gerentes de planta | Oferta de diagnóstico | Gerar RFQs | Etapa 11 | Landing page | Custo por lead e por RFQ |

---

## 12. Regra principal do PDF aplicada à Etapa 2

A pesquisa só serve se alimentar decisões de **para quem** (setores e personas), **com qual conteúdo** (riscos por setor) e **levando o cliente para onde** (diagnóstico). A seção 5 define o que falta provar antes de apostar em "máquinas importadas".

## 13. Pendências

- [ ] Rodar Comex Stat e anexar os dados em `04_dados_e_evidencias`
- [ ] Marcar e fazer 5 a 8 entrevistas (roteiro na Etapa 5; registro em `04_dados_e_evidencias/entrevistas_personas.md`)
- [ ] Obter da Titans a região de atuação
- [ ] Estimar TAM/SAM/SOM (seção 10.1)
- [ ] Reavaliar a afirmação sobre o Sebraetec [F9]
- [ ] Confirmar o enquadramento de PME/MEI na NR-01/NR-12
- [ ] Revisar as notas de setor (seção 3) com a Titans
