# Etapa 2 — Pesquisa de mercado (NR-12)

**Status:** [x] desenvolvida (v1, 26/10/2026) — dados quantitativos de mercado ainda em coleta
**Entregável do PDF:** 03 (Pesquisa de mercado / Mapa do Mercado da Solução)
**Legenda:** **[F]** = fato com fonte · **[H]** = hipótese a validar · **[L]** = lacuna de dado

---

## 1. Resumo do mapa

O mercado da NR-12 é **obrigatório por norma** e **concentrado em quem opera máquinas com risco de lesão grave**. A demanda existe, mas é frequentemente percebida como custo. A concorrência é numerosa, em geral comunica multa e obrigação, e poucos mostram jornada completa ou prova de resultado. A oportunidade da Titans está em ligar diagnóstico, projeto, validação e documentação em uma oferta de engenharia com prova social.

---

## 2. Demanda e contexto

| Indicador | Dado | Tipo | Fonte |
|---|---|---|---|
| Acidentes de trabalho (CAT) em 2022 | 612,9 mil | [F] | Observatório SST/SmartLab [F5] |
| Participação de máquinas e equipamentos nos acidentes (2012–2022) | cerca de 15% | [F] | Observatório SST/SmartLab [F5] |
| Gravidade | Operação de máquinas causa amputações e lesões graves com frequência muito maior que as demais causas; mais acidentes fatais que a média | [F] | [F5] |
| Notificações em 2023 | cerca de 732 mil, com 2,8 mil mortes (base possivelmente diferente) | [F] com ressalva | [F6] |
| Alcance da norma | Máquinas novas e usadas | [F] | [F3][F4] |
| Campanha nacional do MTE sobre segurança em máquinas em 2024 | citada no rascunho | [H] | Sem fonte localizada. Validar antes de usar |
| Flexibilização de 2019 | O texto de 2019 simplificou exigências (ex.: reconhecimento de ISO 13849, certificação Inmetro, manual NBR 16746), e a CNI sustenta que sem reduzir a segurança | [F] | [F4] |
| Tamanho do mercado em R$ | Desconhecido | [L] | A estimar (seção 10) |

**Uso nas peças:** o dado de 15% é forte e verificável. Para 2023 usar a base do Observatório quando atualizada, e não misturar com o número de 2022.

---

## 3. Setores compradores

A priorização abaixo é **hipótese do grupo**, com critério explícito. Deve ser validada com a Titans e com dados de importação/emprego.

| Setor | Prioridade [H] | Por quê | Máquinas típicas |
|---|---|---|---|
| Metalúrgico | Alta | Alta densidade de máquinas com risco de esmagamento e corte | Prensas, dobradeiras, guilhotinas |
| Autopeças | Alta | Muitas máquinas por planta; exigência de clientes e auditorias | Prensas, células de soldagem, injetoras |
| Automotivo | Alta | Linhas automatizadas; cultura de conformidade | Células robotizadas, transportadores |
| Bens de capital | Média-alta | Fabricante pode embarcar segurança no produto | Máquinas especiais |
| Alimentos e bebidas | Média-alta | Envase e embalagem com muitas partes móveis | Embaladoras, esteiras |
| Plásticos | Média [H] | Injetoras e extrusoras | Injetoras |
| Logística | Média | AGVs, empilhadeiras, transelevadores | Transelevadores, AGVs |
| Farmacêutico | Baixa/validar | Sem dado de aderência | Envase, embalagem |

**Segmento transversal:** PMEs metalmecânicas. A NR-12 não isenta microempresa nem MEI (informação do rascunho; **conferir no texto da NR-12/NR-01**), o que amplia o mercado potencial, mas reduz o ticket e aumenta a sensibilidade a preço. [H]

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
| 1 | Comex Stat (MDIC): importações dos capítulos de máquinas (NCM 84 e 85), por ano e país de origem | Volume e valor importado e tendência |
| 2 | Cruzar com setores da seção 3 | Onde está o risco de máquina sem adequação |
| 3 | 5 a 8 entrevistas com engenheiros e gestores industriais | Se compram importadas, quem adequa, quanto pagam, o que os trava |
| 4 | Google Keyword Planner e Trends: "adequação NR-12 máquina importada", "máquina chinesa NR-12" | Intenção de busca |
| 5 | Casos da Titans | Prova interna |

**Cuidado de método:** importação alta de máquinas **não prova** falta de adequação. Só as entrevistas e os casos da Titans provam isso.

---

## 6. Concorrência (resumo; detalhe na Etapa 3)

| Grupo | Exemplos citados | Observação |
|---|---|---|
| Engenharias especializadas em NR-12 | Prisma (SP), EMSEG, Engenharia Adequada, Engehall, ES Engenharia, Ibuma | As quatro últimas ainda não foram analisadas a fundo |
| Integradores/automação com NR-12 como serviço lateral | TechPlus, Grupo Atex, Tesla Automação, Garcia Automação | Benchmarkados na Etapa 3 |
| Distribuidores de componentes | Sulfran | Vendem componentes e treinamento |
| Sebraetec | Programa de consultoria subsidiada | O rascunho diz "faz só documentação", mas o edital localizado lista também identificação de necessidades de adequação e emissão de ART. **Reavaliar a afirmação** |
| Fabricantes de componentes e de máquinas | — | Hipótese: oferecem engenharia junto com o produto |

**Padrão de posicionamento observado:** foco em multa e obrigação; diagnóstico gratuito via WhatsApp e SEO local (Prisma); discurso "NR-12 como engenharia" existe, mas sem jornada nem prova (leitura do grupo, a confirmar na Etapa 3).

---

## 7. Tendências e tecnologias

- Cobots e a ISO 10218 / ISO/TS 15066 como referência de segurança
- Scanners a laser para AGVs e AMRs
- CLPs e módulos de segurança integrados ao controle da máquina
- Documentação técnica em meio digital [H] (sem portaria comprovada; ver correção na Etapa 1)
- Segurança associada a dados e Indústria 4.0 [H]
- Nova redação da NR-28 (2026) com atualização dos códigos de infração, inclusive da NR-12 [F8]

---

## 8. Oportunidades

1. **Ligar laudo a execução:** muitos concorrentes são fortes em um dos lados (laudo ou instalação). A Titans pode vender o fluxo completo.
2. **Diagnóstico como porta de entrada** com escopo fechado e prazo curto.
3. **Nicho NR-12 em automação e robótica** (integração com o restante da engenharia da Titans).
4. **Segurança embarcada para fabricantes de máquinas** (B2B de segunda ordem).
5. **Prova social real:** clientes de peso citados no site (Bombril, Cargill, CCR, CGR, DGS), **desde que a Titans autorize** o uso como case de NR-12.
6. **Parcerias** com escritórios de SST, ABIMAQ e Sebrae.
7. **Máquinas importadas** como segmento com mensagem própria.

## 9. Ameaças

1. Concorrentes com busca local forte e diagnóstico gratuito
2. NR-12 percebida como custo e "papel"
3. Simplificação de exigências em 2019 [F4]
4. Fabricantes oferecendo adequação junto com o produto
5. Fiscalização irregular reduz urgência de compra
6. Risco de reputação e responsabilidade técnica em caso de acidente com máquina adequada
7. Diluição da marca: NR-12 é 1 de 5 serviços no site atual

---

## 10. Lacunas e plano de coleta

| Lacuna | Fonte | Método | Prioridade |
|---|---|---|---|
| Tamanho do mercado em R$ | IBGE (PIA), Comex Stat, ABIMAQ | Estimar número de plantas-alvo × ticket médio da Titans | Alta |
| Preço dos concorrentes | Pedido de orçamento simulado, propostas públicas | Coleta direta | Alta |
| Região de atuação da Titans | Professor | Pergunta | Alta |
| Volume de busca | Keyword Planner, Trends | Coleta (Etapa 7) | Média |
| Demanda por máquinas importadas | Comex Stat + entrevistas | Seção 5 | Alta |
| Campanha MTE 2024 | gov.br | Localizar a fonte ou retirar | Baixa |

---

## 11. Ideias de ação (do rascunho), já no formato "por quê → para quem → ..."

| Ideia | Por quê | Para quem | Conteúdo | Objetivo | Investimento | Destino | Resultado esperado |
|---|---|---|---|---|---|---|---|
| Vídeo curto por setor | Mostrar risco real na máquina do setor do cliente | Engenheiros de manutenção/processos | "Os 3 riscos mais comuns em [prensa/embaladora]" | Gerar interesse e visitas à página | Produção interna | Página NR-12 | Visualizações, cliques, pedidos de diagnóstico |
| Eventos e congressos de NR-12 | Construir autoridade e conexões | Gestores, SST, ABIMAQ | Palestra técnica | Networking e leads | A definir | Contato direto / RFQ | Leads qualificados |
| Anúncios (Google/LinkedIn) | Alcançar quem procura a solução ou decide | Donos de PME, gerentes de planta | Oferta de diagnóstico | Gerar RFQs | Etapa 11 | Landing page | Custo por lead e por RFQ |

---

## 12. Regra principal do PDF aplicada à Etapa 2

A pesquisa de mercado só serve se alimentar decisões de **para quem** (setores e personas), **com qual conteúdo** (riscos por setor) e **levando o cliente para onde** (diagnóstico). A seção 5 define o que falta provar antes de apostar em "máquinas importadas".

## 13. Pendências

- [ ] Rodar Comex Stat e anexar os dados em `04_dados_e_evidencias`
- [ ] Marcar e fazer 5 a 8 entrevistas
- [ ] Obter da Titans a região de atuação
- [ ] Reavaliar a afirmação sobre o Sebraetec
- [ ] Confirmar o enquadramento de PME/MEI na NR-01/NR-12
