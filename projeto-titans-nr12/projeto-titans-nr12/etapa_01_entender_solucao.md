# Etapa 1 — Entender o produto/serviço (NR-12)

**Status:** [x] desenvolvida (v1, 26/10/2026) — pendente de revisão do grupo e validação com a Titans
**Entregáveis do PDF atendidos:** 01 (descrição técnica) e 02 (descrição comercial)
**Escopo:** somente NR-12 (decisão nº 2 em `00_gestao/decisoes.md`). O trecho de Máquinas/Retrofit do rascunho (Grupo 1) foi retirado deste texto.
**Fontes:** códigos `[F1]`… detalhados em `00_gestao/fontes_e_validacao.md`.

---

## 1. Em duas frases

A NR-12 define as medidas de proteção obrigatórias para quem projeta, fabrica, importa, instala, opera e mantém máquinas e equipamentos. A solução Titans NR-12 transforma essa obrigação em um **projeto de engenharia**: diagnóstico da máquina, apreciação de risco, projeto e implantação das proteções, validação do sistema de segurança e documentação com responsabilidade técnica.

---

## 2. Contexto normativo (validado em fonte pública)

| Ponto | O que se confirmou | Como usar no texto |
|---|---|---|
| Alcance | A NR-12 se aplica a máquinas **novas e usadas**, com as exceções previstas no texto [F3][F4] | Base para o argumento "máquina nova e importada também precisa estar conforme" |
| Texto vigente | O texto geral foi renovado pela Portaria SEPRT nº 916/2019 [F3][F4] | Citar sempre o texto consolidado vigente, não o de 2010 |
| Máquinas importadas | Máquinas **nacionais ou importadas** projetadas conforme ABNT NBR ISO 13849 (partes 1 e 2) são consideradas em conformidade quanto às partes de comando relacionadas à segurança (item 12.1.11) [F3] | Mostra que o caminho técnico existe e é verificável: o que precisa ser comprovado é o desempenho do sistema de segurança |
| Manual | Máquinas fabricadas a partir de 2019, nacionais ou importadas, seguem a NBR 16746 para o manual de instruções; manual em português [F4][F7] | Falta de manual em português é não conformidade típica de importadas |
| Normas posteriores | Não é obrigatório observar normas técnicas publicadas depois da fabricação, importação ou adequação, desde que a máquina atenda a NR-12 vigente (item 12.1.9.2) [F3] | Limita o escopo: o diagnóstico mede a máquina contra a NR-12, não contra "o estado da arte" |
| Responsabilidade técnica | Projeto de adequação de máquina existente deve ter projeto mecânico por profissional habilitado, com ART. Para máquina nova, a ABIMAQ informa que a NR-12 não exige laudo do fabricante nem ART, mas recomenda declaração de conformidade [F7] | A distinção importa para vender "laudo + ART" com precisão |
| Penalidades | Multas seguem a NR-28, por grau da infração (1 a 4) e número de empregados; a NR-28 foi alterada em 2026 (Portaria MTE nº 104/2026), com reajuste anual e atualização do Anexo II, inclusive códigos da NR-12 [F8] | Não citar faixa de valores sem conferir a tabela vigente |

### Correções ao rascunho (importante)

1. **Prazo de 02/01/2025 não é um prazo geral da NR-12.** A Portaria MTE nº 224/2024 trata do **Anexo X (máquinas para fabricação de calçados e afins)**, para máquinas usadas não adequadas nos prazos da Portaria nº 252/2018 [F1]. O rascunho generalizou. **Não usar "prazo encerrado em jan/2025" como gatilho de urgência para todos os setores.** O gatilho legítimo é: a norma já vale para máquinas novas e usadas, e a fiscalização pode autuar.
2. **Portaria MTE nº 344/2024 não trata de digitalização de documentos.** Ela altera glossário (Anexo I da NR-01), com reflexo nas definições da NR-12 [F2]. A frase "fiscalização digital a partir de 2026" saiu do texto até ter fonte.
3. **Acidentes:** o dado de 612,9 mil é de **2022**, e não de 2023 [F5]. Para 2023 há reportagem citando 732 mil notificações [F6], em base possivelmente diferente (inclui casos sem CAT). Padronizamos: **612,9 mil CAT em 2022 (Observatório SST)**.
4. **"Redução de 95% em acidentes com cortinas de luz"** não tem fonte. Foi removido. Só volta se a Titans tiver case próprio.
5. **Cortina de luz e velocidade de aproximação (ISO 13855):** o trecho do rascunho está confuso. Não usar os valores numéricos sem revisão de quem domine a norma.

---

## 3. As 9 perguntas do PDF

| Pergunta | Resposta |
|---|---|
| **O que é?** | Serviço de engenharia de segurança de máquinas: levanta a máquina, avalia o risco, projeta e implanta proteções e comandos de segurança, valida o desempenho e entrega documentação técnica com responsável habilitado. |
| **Como funciona?** | Fluxo em 6 etapas (seção 4): Diagnóstico → Análise de risco → Projeto → Adequação → Validação → Documentação. |
| **Para que serve?** | Proteger pessoas e manter a máquina operando dentro da norma. Para a empresa: reduzir risco de acidente, de autuação e de interdição; para a operação: manter produtividade com a máquina protegida. |
| **Problemas que resolve** | *Legal:* não conformidade com a NR-12. *Segurança:* pontos de esmagamento, corte, choque e projeção sem proteção. *Operacional:* paradas por interdição ou por proteções mal integradas. *Financeiro:* custo de multa, afastamento e acidente. *Documental:* ausência de apreciação de risco, manual e laudo. |
| **Tecnologias** | Proteções fixas e móveis intertravadas; chaves de segurança; cortinas de luz; scanners; tapetes; relés e CLPs de segurança; parada de emergência; comando bimanual; projeto elétrico (diálogo com NR-10). Normas: ABNT NBR ISO 12100, ISO/TR 14121-2, ABNT NBR ISO 13849-1/-2, ISO 13855, IEC 61496. *A confirmar com a Titans: o que é feito internamente e o que é subcontratado.* |
| **Aplicações** | Prensas, dobradeiras, guilhotinas, injetoras, embaladoras, esteiras, células robotizadas e cobots, transelevadores e AGVs (fonte: rascunho; validar prioridade na Etapa 2). |
| **Resultados possíveis** | Máquina com apreciação de risco documentada; sistema de segurança com nível de desempenho verificado; laudo e ART; manual e registros de capacitação em ordem. **Promessa comercial segura:** "máquina avaliada, protegida e documentada". **Evitar:** prometer redução percentual de acidentes ou "zero multa". |
| **Limitações** | Máquina sem documentação técnica (esquemas elétricos, manual) exige reconstituição; máquina importada com comando de segurança não verificável pode exigir substituição do sistema de comando; a Titans não controla a fiscalização nem garante ausência de autuação; a adequação depende da parada da máquina. |
| **O que a Titans precisa dominar** | Apreciação de risco (ISO 12100); determinação do PLr e verificação do PL (13849-1/-2); projeto elétrico e de comando de segurança; adequação mecânica; emissão de documentos com ART; gestão de projeto com parada programada. |

---

## 4. Fluxo da solução (do PDF) com entradas e saídas

| Fase | O que acontece | Entrada | Saída |
|---|---|---|---|
| 1. Diagnóstico | Inventário de máquinas; identificação de zonas de perigo (esmagamento, corte, choque, projeção); checagem de documentação | Máquinas da planta, manuais, esquemas | Inventário + lista de não conformidades |
| 2. Análise de risco | Apreciação conforme ISO 12100; método de classificação (ex.: HRN) e priorização | Inventário, ciclo de operação, acessos do operador | Documento de apreciação de risco; PLr requerido |
| 3. Projeto | Especificação de proteções, sensores, relés, intertravamentos, parada de emergência; projeto elétrico | Apreciação de risco | Projeto mecânico e elétrico de segurança |
| 4. Adequação | Instalação e integração das medidas na máquina | Projeto aprovado, janela de parada | Máquina adequada fisicamente |
| 5. Validação | Verificação de que o sistema de segurança atinge o PLr (ISO 13849-2), incluindo falhas | Máquina adequada | Relatório de validação |
| 6. Documentação | Laudo de conformidade, manual de instruções, registros de capacitação | Resultados das fases anteriores | Pacote documental com ART |

**Observação de funil:** o diagnóstico/inventário é o serviço de menor atrito e a melhor porta de entrada comercial (hipótese H2 do projeto).

---

## 5. O ângulo "máquinas importadas" (hipótese a comprovar)

- **Ponto de partida:** relato do professor de que empresas compram máquinas (por exemplo, da China) sem adequação à NR-12. **Status: hipótese.** Não há dado no projeto que a sustente ainda.
- **Por que a hipótese é plausível tecnicamente:** a norma exige que máquina importada atenda ao texto brasileiro, inclusive manual em português e sistemas de comando de segurança com desempenho comprovável (itens 12.1.11 e correlatos) [F3][F4]. Máquina projetada para outro mercado pode não vir com isso.
- **Como virar oferta:** "Check-up NR-12 de máquina importada" (nome provisório), como serviço de entrada com escopo fechado: análise documental + inspeção + lista de não conformidades + estimativa de adequação.
- **Como comprovar (Etapa 2):** (a) importações de máquinas por NCM no Comex Stat/MDIC; (b) entrevistas com 5 a 8 compradores industriais; (c) volume de busca por termos como "adequação NR-12 máquina importada"; (d) casos da própria Titans.
- **Perguntas para a Titans:** já adequou máquina importada? Tem acesso aos esquemas elétricos? Quem contratou: usuário final ou importador?

---

## 6. Entrega A — Descrição técnica da solução

A solução Titans NR-12 é um serviço de engenharia de segurança de máquinas e equipamentos industriais, estruturado em seis fases (diagnóstico, análise de risco, projeto, adequação, validação e documentação). Parte do inventário das máquinas, identifica perigos e estima riscos conforme a ABNT NBR ISO 12100, define o nível de desempenho requerido do sistema de segurança e projeta as medidas de proteção: proteções fixas e móveis intertravadas, dispositivos sensíveis (cortinas de luz, scanners, tapetes), chaves de segurança, relés ou CLPs de segurança, paradas de emergência e circuitos de comando. A implantação é seguida de validação do desempenho dos circuitos de segurança segundo a ABNT NBR ISO 13849-2 e da emissão da documentação técnica (apreciação de risco, laudo de conformidade, manual de instruções em português e registros de capacitação), com responsabilidade técnica de profissional habilitado e ART. O serviço se aplica a máquinas nacionais e importadas, novas e usadas.

## 7. Entrega B — Descrição comercial da solução

A Titans trata a NR-12 como engenharia, e não como papelada. Em vez de entregar apenas um laudo, conduz o cliente do diagnóstico da máquina até a documentação final, com um único responsável técnico e uma equipe com formação de mestres e doutores *(confirmar com a Titans antes de publicar)*. O cliente enxerga o que está fora de conformidade, o que precisa ser feito, em que ordem e com que custo, e recebe a máquina protegida, validada e documentada. A porta de entrada é um diagnóstico de baixo atrito (inventário e triagem de risco), que permite ao cliente conhecer a Titans antes de contratar o projeto completo. Para empresas que importam máquinas, o serviço verifica se o equipamento atende à norma brasileira antes de entrar em produção.

**Proposta de valor (provisória):** Da máquina em risco à máquina protegida e documentada, em um só fluxo de engenharia.

---

## 8. Regra principal do PDF aplicada à Etapa 1

- **Por quê:** a NR-12 vale para máquinas novas e usadas, e a falta de adequação expõe pessoas e empresa.
- **Para quem:** indústrias que operam ou importam máquinas.
- **Com qual conteúdo:** explicações técnicas do fluxo e do que cada fase entrega.
- **Com qual objetivo:** gerar pedidos de diagnóstico e RFQs.
- **Resultado esperado:** o cliente entende o serviço como um projeto de engenharia com entregas definidas.

## 9. Pendências antes de fechar a Etapa 1

- [ ] Confirmar com a Titans: cidade/estado, equipe (mestres/doutores), o que é feito internamente, cases de NR-12 autorizáveis
- [ ] Conferir itens da NR-12 citados (12.1.9.2, 12.1.11 e os de manual) no texto consolidado do gov.br
- [ ] Decidir se "máquinas importadas" é recorte principal ou campanha dentro da oferta geral
- [ ] Revisar com o professor
