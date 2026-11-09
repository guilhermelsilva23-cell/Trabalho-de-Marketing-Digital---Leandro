# Etapa 1 — Entender o Produto/Serviço
## Descrição Técnica e Comercial da Solução **Titans NR-12 — Segurança de Máquinas como Engenharia**

**Projeto Aplicado — Marketing Digital Titans | Grupo 4: NR-12**
**Entregáveis do PDF atendidos:** 01 (Descrição técnica da solução) e 02 (Descrição comercial da solução)
**Versão:** v2 — aprofundamento da v1 de 26/10/2026
**Escopo:** somente NR-12 (decisão nº 2 em `00_gestao/decisoes.md`). Retrofit e automação ficam estacionados.

**Legenda de marcadores**
- `[F#]` = fato com fonte em `00_gestao/fontes_e_validacao.md`
- `[CONFIRMAR]` = informação que só a Titans pode confirmar antes de publicar
- `[VERIFICAR NORMA]` = item a conferir no texto consolidado da NR-12 (gov.br)
- `[HIPÓTESE]` = ainda sem dado que a sustente

---

## 1. Resumo executivo

A NR-12 define as medidas de proteção obrigatórias para quem projeta, fabrica, importa, instala, opera e mantém máquinas e equipamentos `[F3][F4]`. Na prática, muitas empresas tratam o tema como papelada (um laudo) e não como o que ele é: um **projeto de engenharia** que altera a máquina, o comando elétrico e a rotina de operação.

A **Titans NR-12** transforma essa obrigação em um fluxo único de engenharia:

> **Diagnóstico → Análise de risco → Projeto → Adequação → Validação → Documentação**

O cliente recebe a máquina **avaliada, protegida e documentada**, com responsável técnico habilitado e ART, em vez de contratar separadamente laudo, projeto e instalação.

---

## 2. Contexto normativo (o que já foi validado)

| Ponto | O que se confirmou | Como usar |
|---|---|---|
| Alcance | A norma se aplica a máquinas **novas e usadas**, com as exceções previstas `[F3][F4]` | "Máquina nova ou importada também precisa estar conforme" |
| Texto vigente | Texto geral renovado pela Portaria SEPRT nº 916/2019 `[F3][F4]` | Citar sempre o texto consolidado vigente |
| Máquinas importadas | Máquinas nacionais ou importadas projetadas conforme ABNT NBR ISO 13849 (partes 1 e 2) são consideradas conformes quanto às partes de comando relacionadas à segurança (item 12.1.11) `[F3]` `[VERIFICAR NORMA]` | O caminho técnico existe; o que se precisa comprovar é o desempenho do sistema de segurança |
| Manual | Máquinas fabricadas a partir de 2019, nacionais ou importadas, seguem a NBR 16746; manual em português `[F4][F7]` | Falta de manual em português é não conformidade típica de importadas |
| Normas posteriores | Não é obrigatório observar normas técnicas publicadas depois da fabricação, importação ou adequação, desde que se atenda a NR-12 vigente (item 12.1.9.2) `[F3]` `[VERIFICAR NORMA]` | O diagnóstico mede a máquina contra a NR-12, não contra "o estado da arte" |
| Responsabilidade técnica | Projeto de adequação de máquina existente exige profissional habilitado com ART. Para máquina nova, a ABIMAQ informa que a norma não exige laudo do fabricante nem ART, mas recomenda declaração de conformidade `[F7]` | Vender "laudo + ART" com precisão |
| Penalidades | Seguem a NR-28 (grau 1 a 4 e número de empregados); a NR-28 foi alterada em 2026 (Portaria MTE nº 104/2026) `[F8]` | **Não citar faixa de valores** sem conferir a tabela vigente |

### Afirmações do rascunho original que **não devem ser usadas**

| Afirmação | Motivo |
|---|---|
| "Prazo encerrado em 02/01/2025" como regra geral | A Portaria MTE nº 224/2024 trata do Anexo X (calçados), não é prazo geral `[F1]` |
| "Portaria 344/2024 incentiva digitalização" | Ela altera glossário da NR-01 `[F2]` |
| "612 mil acidentes em 2023" | 612,9 mil é de **2022** `[F5]` |
| "Redução de 95% de acidentes com cortinas de luz" | Sem fonte; só volta se a Titans tiver case próprio |
| "Multas de R$ 670 a R$ 134.000" | A validar na tabela vigente da NR-28 |
| Velocidades de aproximação da ISO 13855 | Redação confusa; revisar com quem domine a norma |

---

## 3. As 9 perguntas do PDF

| Pergunta | Resposta |
|---|---|
| **O que é?** | Serviço de engenharia de segurança de máquinas: levanta a máquina, avalia o risco, projeta e implanta proteções e comandos de segurança, valida o desempenho e entrega documentação técnica com responsável habilitado. |
| **Como funciona?** | Seis fases encadeadas (seção 4), cada uma com entrada e saída definidas. |
| **Para que serve?** | Proteger pessoas e manter a máquina operando dentro da norma. Para a empresa: reduzir risco de acidente, autuação e interdição. Para a operação: manter a produtividade com a máquina protegida. |
| **Quais problemas resolve?** | *Legal:* não conformidade. *Segurança:* pontos de esmagamento, corte, choque e projeção sem proteção. *Operacional:* paradas por interdição ou por proteções mal integradas. *Financeiro:* custo de multa, afastamento e acidente. *Documental:* ausência de apreciação de risco, manual e laudo. |
| **Quais tecnologias estão envolvidas?** | Seção 5. |
| **Quais aplicações industriais existem?** | Seção 6. |
| **Quais resultados podem ser obtidos?** | Seção 7. |
| **Quais são as limitações?** | Seção 8. |
| **O que a Titans precisa dominar?** | Seção 9. |

---

## 4. Como funciona: o fluxo em seis fases

```
DIAGNÓSTICO → ANÁLISE DE RISCO → PROJETO → ADEQUAÇÃO → VALIDAÇÃO → DOCUMENTAÇÃO
```

| Fase | O que acontece | Entrada | Saída |
|---|---|---|---|
| **1. Diagnóstico** | Inventário das máquinas; identificação de zonas de perigo (esmagamento, corte, choque, projeção); checagem de documentação existente | Máquinas da planta, manuais, esquemas elétricos | Inventário e lista de não conformidades |
| **2. Análise de risco** | Apreciação conforme ABNT NBR ISO 12100; classificação e priorização por criticidade (ex.: HRN, ISO/TR 14121-2); definição do **PLr** requerido | Inventário, ciclo de operação, formas de acesso do operador | Documento de apreciação de risco; PLr por função de segurança |
| **3. Projeto** | Especificação de proteções, sensores, relés/CLPs de segurança, intertravamentos, parada de emergência; projeto elétrico (diálogo com NR-10) | Apreciação de risco | Projeto mecânico e elétrico de segurança |
| **4. Adequação** | Instalação e integração das medidas na máquina | Projeto aprovado e janela de parada | Máquina adequada fisicamente |
| **5. Validação** | Verificação de que o sistema de segurança atinge o PLr (ABNT NBR ISO 13849-2), inclusive análise de falhas | Máquina adequada | Relatório de validação |
| **6. Documentação** | Laudo de conformidade, manual de instruções em português, registros de capacitação, tudo com ART | Resultados das fases anteriores | Pacote documental com responsabilidade técnica |

**Por que a análise de risco é o centro da "engenharia":** duas máquinas aparentemente iguais podem exigir soluções diferentes, conforme layout, forma de acesso do operador e frequência de uso. Por isso a solução **não é de prateleira**.

**Por que não basta comprar o dispositivo:** um relé de segurança errado ou mal ligado pode anular a função de segurança mesmo com o equipamento correto. É preciso projeto e integração. *(Argumento coerente com a ISO 13849; revisar com engenheiro da Titans.)*

---

## 5. Tecnologias envolvidas

| Grupo | Itens | Papel |
|---|---|---|
| **Proteções físicas** | Fixas (enclausuramento) e móveis com intertravamento | Impedem o acesso à zona de perigo |
| **Dispositivos de detecção** | Cortinas de luz, scanners a laser, barreiras ópticas, tapetes, sensores de posição | Detectam a presença e acionam a parada |
| **Intertravamentos** | Chaves mecânicas, magnéticas ou codificadas (RFID) | Mantêm a proteção fechada até a máquina parar |
| **Comando de segurança** | Relés de segurança, CLPs de segurança, módulos de monitoração | Executam a parada segura |
| **Parada de emergência e bimanual** | Botões e comandos bimanuais | Medida auxiliar; **não substitui** proteções adequadas |
| **Projeto elétrico** | Painéis, circuitos de comando, diálogo com NR-10 | Evitam choque, incêndio e falha de comando |
| **Adequação mecânica** | Enclausuramentos, distâncias de segurança, eliminação de pontos de esmagamento | Atingem fisicamente a categoria definida |

**Normas de referência:** ABNT NBR ISO 12100 (apreciação de risco), ISO/TR 14121-2 (guia prático), ABNT NBR ISO 13849-1 e -2 (partes de comando e validação), ISO 13855 (posicionamento de dispositivos), IEC 61496 (dispositivos sensíveis), NBR 16746 (manual), NR-10 (elétrica).

`[CONFIRMAR]` com a Titans: o que é feito internamente e o que é subcontratado (fabricação de proteções, montagem de painéis, calibração).

---

## 6. Aplicações industriais

| Máquina / ambiente | Risco típico | Prioridade de mercado `[HIPÓTESE]` |
|---|---|---|
| Prensas, dobradeiras, guilhotinas | Esmagamento, corte, amputação | Alta (metalúrgico, autopeças) |
| Células de soldagem e injetoras | Esmagamento, projeção, queimadura | Alta (autopeças, plásticos) |
| Células robotizadas e cobots | Impacto, aprisionamento (ISO 10218, ISO/TS 15066 como referência) | Alta (automotivo) |
| Embaladoras e esteiras | Partes móveis, arrastamento | Média-alta (alimentos e bebidas) |
| Transelevadores, AGVs/AMRs, empilhadeiras | Colisão, acesso a áreas de operação | Média (logística) |
| Máquinas importadas sem adequação | Comando de segurança não verificável, falta de manual em português | **Hipótese central, ainda sem prova** (Etapa 2, seção 5) |
| Máquinas antigas sem documentação | Falta de esquema e manual | Média |

**Segmento transversal:** PMEs metalmecânicas. A isenção (ou não) de ME/MEI **precisa ser conferida no texto vigente** antes de ser usada em comunicação.

---

## 7. Resultados que podem ser obtidos

**Promessa comercial segura:** *"Máquina avaliada, protegida e documentada."*

Resultados defensáveis:
1. Máquina com **apreciação de risco documentada**.
2. Sistema de segurança com **nível de desempenho verificado** (ISO 13849).
3. Laudo de conformidade com **ART**, manual em português e registros de capacitação em ordem.
4. Riscos **priorizados por criticidade**, permitindo decidir o investimento com critério.
5. Menor exposição a autuação e interdição.

**Evitar prometer:** redução percentual de acidentes, "zero multa" ou "100% de conformidade garantida". A Titans não controla a fiscalização.

---

## 8. Limitações da solução

| Limitação | Consequência | Como a Titans trata |
|---|---|---|
| Máquina sem documentação técnica | Exige reconstituição de esquema e manual | Incluir no diagnóstico e na estimativa |
| Máquina importada com comando de segurança não verificável | Pode exigir substituição do sistema de comando | Check-up documental e inspeção antes da proposta |
| Dependência da parada da máquina | Adequação precisa de janela de produção | Planejar parada programada |
| Fiscalização fora do controle da Titans | Não há garantia de ausência de autuação | Linguagem de comunicação cuidadosa |
| Responsabilidade técnica | Risco de reputação em caso de acidente após adequação | Processo documentado, validação e ART |
| Equipamentos além do escopo | Retrofit funcional, peças fora do projeto | Escopo "não inclui" claro na proposta |

---

## 9. O que a Titans precisa dominar

1. Apreciação de risco (ISO 12100) e métodos de classificação (HRN).
2. Determinação do **PLr** e verificação do **PL** (ISO 13849-1 e -2).
3. Projeto elétrico e de comando de segurança (NR-10).
4. Seleção e integração de cortinas de luz, scanners, intertravamentos e relés/CLPs de segurança.
5. Adequação mecânica (enclausuramentos, distâncias, pontos de esmagamento).
6. Emissão de documentos com ART (laudo, apreciação de risco, manual NBR 16746).
7. Gestão de projeto com parada programada de produção.
8. Capacitação de operadores e manutenção, com registro.
9. Relacionamento comercial: diagnóstico claro, proposta comparável, RFQ.

---

## 10. Descrição técnica da solução (Entregável 01)

> A solução **Titans NR-12** é um serviço de engenharia de segurança de máquinas e equipamentos industriais, estruturado em seis fases: diagnóstico, análise de risco, projeto, adequação, validação e documentação. O serviço parte do inventário das máquinas, identifica perigos e estima riscos conforme a ABNT NBR ISO 12100, define o nível de desempenho requerido (PLr) dos sistemas de segurança e projeta as medidas de proteção: proteções fixas e móveis intertravadas, dispositivos sensíveis (cortinas de luz, scanners, tapetes), chaves de segurança, relés ou CLPs de segurança, paradas de emergência e circuitos de comando. A implantação é seguida da validação do desempenho dos circuitos de segurança segundo a ABNT NBR ISO 13849-2 e da emissão da documentação técnica (apreciação de risco, laudo de conformidade, manual de instruções em português e registros de capacitação), com responsabilidade técnica de profissional habilitado e ART. O serviço se aplica a máquinas nacionais e importadas, novas e usadas.

---

## 11. Descrição comercial da solução (Entregável 02)

> A Titans trata a NR-12 como **engenharia**, e não como papelada. Em vez de entregar apenas um laudo, conduz o cliente do diagnóstico da máquina até a documentação final, com **um único responsável técnico** `[CONFIRMAR: equipe com formação de mestres e doutores]`. O cliente enxerga o que está fora de conformidade, o que precisa ser feito, em que ordem e com que custo, e recebe a máquina protegida, validada e documentada.
>
> A porta de entrada é um **diagnóstico de baixo atrito** (inventário e triagem de risco), que permite ao cliente conhecer a Titans antes de contratar o projeto completo. Para empresas que importam máquinas, o serviço verifica se o equipamento atende à norma brasileira **antes de entrar em produção**.

### 11.1 Proposta de valor (provisória)

**Da máquina em risco à máquina protegida e documentada, em um só fluxo de engenharia.**

### 11.2 Matriz de mensagens

| Dimensão | Mensagem |
|---|---|
| **Racional** | Um contrato e um responsável cobrem diagnóstico, projeto, implantação, validação e documentação. |
| **Técnica** | Apreciação de risco conforme ISO 12100 e desempenho do sistema de segurança verificado conforme ISO 13849. |
| **Emocional** | "Não é papelada, é proteger quem opera a máquina." Dado de apoio: cerca de 15% dos acidentes de trabalho de 2012 a 2022 vieram de máquinas e equipamentos `[F5]`. |
| **Comercial** | Comece pelo diagnóstico e decida o investimento com a lista de riscos na mão. |

### 11.3 Diferenciais a sustentar

| Diferencial | Status |
|---|---|
| Fluxo completo em um único contrato (laudo + execução) | Defensável pelo desenho do serviço |
| Responsabilidade técnica com ART | Defensável |
| Equipe com mestres e doutores | `[CONFIRMAR]` com a Titans |
| Clientes de peso (Bombril, Cargill, CCR, CGR, DGS) | `[CONFIRMAR autorização]` para uso como cases de NR-12 |
| Engenharia integrada (CAD/CAE, estruturas, robótica) | `[CONFIRMAR]` capacidades por área |

---

## 12. Ângulo "máquinas importadas" (hipótese a comprovar)

- **Origem:** relato do professor de que empresas compram máquinas (por exemplo, da China) sem adequação à NR-12. **Status: hipótese**, sem dado no projeto que a sustente `[HIPÓTESE]`.
- **Plausibilidade técnica:** a norma exige que a máquina importada atenda ao texto brasileiro, inclusive manual em português e sistemas de comando de segurança com desempenho comprovável `[F3][F4]`.
- **Oferta de entrada sugerida:** *Check-up NR-12 de Máquina Importada* (nome provisório): análise documental, inspeção, lista de não conformidades e estimativa de adequação.
- **Como comprovar (Etapa 2):** Comex Stat/MDIC por NCM, entrevistas com 5 a 8 compradores industriais, volume de busca no Google e casos da própria Titans.
- **Cuidado de método:** importação alta de máquinas **não prova** falta de adequação.

---

## 13. Regra principal do PDF aplicada à Etapa 1

| Pergunta | Resposta |
|---|---|
| **Por quê** | A NR-12 vale para máquinas novas e usadas, e a falta de adequação expõe pessoas e empresa. |
| **Para quem** | Indústrias que operam ou importam máquinas. |
| **Com qual conteúdo** | Explicações técnicas do fluxo e do que cada fase entrega. |
| **Com qual objetivo** | Gerar pedidos de diagnóstico e RFQs. |
| **Investimento** | Definir nas Etapas 6 e 11. |
| **Levando o cliente para onde** | Página NR-12 e landing page do diagnóstico. |
| **Resultado esperado** | O cliente entende o serviço como projeto de engenharia com entregas definidas. |

**Validação do entregável:** *"Isto poderia realmente ser utilizado pela Titans?"* Sim, para as seções 10 e 11, após confirmação dos itens marcados com `[CONFIRMAR]`.

---

## 14. Pendências antes de fechar a Etapa 1

- [ ] Confirmar com a Titans: cidade/estado de atuação, equipe (mestres/doutores), o que é feito internamente e o que é subcontratado
- [ ] Obter da Titans cases de NR-12 autorizáveis (fotos, resultados, depoimentos)
- [ ] Conferir no texto consolidado da NR-12 os itens 12.1.9.2, 12.1.11 e os relativos a manual
- [ ] Conferir a tabela vigente de multas da NR-28 (Portaria MTE nº 104/2026) antes de qualquer menção a valores
- [ ] Conferir enquadramento de ME/MEI na NR-01/NR-12
- [ ] Decidir se "máquinas importadas" é recorte principal ou campanha dentro da oferta geral
- [ ] Trocar fontes secundárias (portais, reportagens) por fontes primárias (DOU/gov.br) para o artigo
- [ ] Revisar com o professor

---

## 15. Fontes

Códigos detalhados em `00_gestao/fontes_e_validacao.md` (acesso em 26/10/2026):

- **F1** Portaria MTE nº 224/2024
- **F2** Portaria MTE nº 344/2024
- **F3** Portaria SEPRT nº 916/2019 (texto da NR-12)
- **F4** CBIC/CNI — texto da NR-12 de 2019
- **F5** Observatório SST/SmartLab (dados de acidentes, 2012–2022)
- **F7** ABIMAQ — materiais sobre NR-12
- **F8** Portaria MTE nº 104/2026 (NR-28)
