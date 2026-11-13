# Relatório de validação — rodada de 12/11/2026
Escopo: itens marcados **A VALIDAR** em `fontes_e_validacao.md`, afirmações do professor que podiam ser checadas em fonte pública e a afirmação sobre o MiroFish. O que não pode ser verificado em fonte pública está em `plano_de_validacao_respostas_1_a_5.md`.

## 1. Resultado resumido
| Item | Antes | Depois | Efeito no projeto |
|---|---|---|---|
| Campanha nacional do MTE em 2024 | A VALIDAR | **VALIDADO** (CANPAT 2024, 18/04/2024) | Pode ser usada em conteúdo e no artigo |
| Sebraetec "só documentação" | A VALIDAR | **VALIDADO COM RESSALVA** | Reformular: "não inclui adequação física" |
| NR-12 sem isenção ME/MEI | A VALIDAR | **CORRIGIDO** | Não há isenção geral, mas há tratamentos pontuais |
| Multas R$ 670 a R$ 134 mil | A VALIDAR | **CORRIGIDO** | Usar faixa por item (~R$ 670 a ~R$ 6,7 mil) e só com ressalva; **R$ 134 mil removido** |
| Portaria 104/2026 inclui NR-12 | Afirmado | **CORRIGIDO** | O que inclui a NR-12 é a Portaria 1.758/2026 (30/09/2026) |
| Itens 12.1.2, 12.1.9.2, 12.1.11 | "Conferir no texto" | **VALIDADO** (texto lido) | Pode citar |
| "A China não tem norma" (E11) | A VALIDAR | **CORRIGIDO** | Não usar a frase; existem normas chinesas |
| Importação de máquinas da China crescente (E12 contexto) | HIPÓTESE | **VALIDADO** como tendência (fonte setorial interessada) | H1 ganha apoio de contexto, sem provar falta de adequação |
| MiroFish "prêmio do GitHub" | Relato de colega | **CORRIGIDO** | Foi 1º lugar no GitHub Trending, não prêmio |
| ISO 13855 (1600 e 2000 mm/s) | A VALIDAR | **A VALIDAR** | Continua sem uso; exige a norma original |
| Valor vigente das multas 2026 | A VALIDAR | **A VALIDAR** | Falta tabela atualizada do Anexo I (fonte primária) |

## 2. Achados novos que mudam a oferta
1. **Item 12.15.2:** é proibida a importação, comercialização, locação e exposição de máquinas que não atendam à NR-12. Isso reforça a oferta "máquina importada" com base na própria norma.
2. **Limitações a declarar:** máquinas certificadas pelo Inmetro (com requisitos de segurança atendidos) e máquinas exclusivamente para exportação não se sujeitam à NR-12 (12.1.3 e 12.1.4 "f"). O diagnóstico deve verificar isso primeiro, para não vender adequação onde não há obrigação.
3. **Dados de contexto da importação (ABIMAQ, entidade que representa fabricantes nacionais):** China com 32% das importações de máquinas em 2025, contra 16,6% em 2015; 36% de janeiro a agosto de 2026 (US$ 8,0 bilhões); importados ≈ 47,7% do consumo no 1º semestre de 2026. Cuidado: mostra aumento da importação, **não** falta de adequação.
4. **Dado de acidente por máquina:** 60.979 acidentes típicos em 2021 com agente "máquinas e equipamentos" (MTE) e ~15% do total em 2012–2022.

## 3. Correções para aplicar nas etapas (localizar → substituir)
| Arquivo | Texto atual | Texto proposto |
|---|---|---|
| `02_etapas/etapa_01_entender_solucao.md`, tabela da seção 2, linha "Penalidades" | "...a NR-28 foi alterada em 2026 (Portaria MTE nº 104/2026), com reajuste anual e atualização do Anexo II, inclusive códigos da NR-12 [F8]" | "A NR-28 prevê reajuste anual dos valores (item 28.3.3, incluído pela Portaria MTE nº 104/2026). A atualização das tabelas de infração que inclui a NR-12 consta da Portaria MTE nº 1.758/2026, de 30/09/2026 [F8][F19]. Não citar faixa de valores sem conferir a tabela vigente." |
| `02_etapas/etapa_02.md`, seção 2, linha "Campanha nacional do MTE em 2024" | "[H] Sem fonte localizada. Validar antes de usar" | "[F] CANPAT 2024 (MTE), lançada em 18/04/2024, tema Segurança em Máquinas e Equipamentos [F16]" |
| `02_etapas/etapa_02.md`, seção 3 (parágrafo "Segmento transversal") | "A NR-12 não isenta microempresa nem MEI (informação do rascunho; conferir...)" | "A NR-12 não traz isenção geral para ME/MEI; há tratamentos pontuais (12.13.5.3 e 12.16.3.1) [F10]. A NR-01 (item 1.8) dispensa o MEI de PGR, o que não alcança a empresa contratante [F17]. [H] sobre o efeito no ticket e na sensibilidade a preço." |
| `02_etapas/etapa_02.md`, seção 6, linha "Sebraetec" | "O rascunho diz 'faz só documentação', mas o edital localizado lista também identificação de necessidades de adequação e emissão de ART. Reavaliar a afirmação" | "A ficha do Sebrae MG limita a consultoria à documentação técnica, diagnóstico de conformidade e treinamento, sem adequação física [F15]; o edital nacional inclui identificação de necessidades e ART [F9]. Escrever: 'não inclui a adequação física'." |
| `02_etapas/etapa_02.md`, seção 7 | "Nova redação da NR-28 (2026) com atualização dos códigos de infração, inclusive da NR-12 [F8]" | "Atualização das tabelas de infração da NR-28 em 2026; a Portaria MTE nº 1.758/2026 inclui a NR-12 [F19]" |
| `02_etapas/etapa_02.md`, seção 5 (H1) | "Status: não comprovada" | "Status: apoio qualitativo [E] e de contexto [F21] (China 32% das importações em 2025; 36% em jan–ago/2026). Falta evidência de que máquinas importadas chegam sem adequação (Comex Stat não prova isso; entrevistas e casos da Titans sim)." |
| `02_etapas/etapa_04.md`, seção 5 | (lista de argumentos que não usar) | Acrescentar: "'A China não tem norma de segurança de máquinas' (existem normas chinesas, algumas equivalentes à ISO) [F20]" e "'Multa de até R$ 134 mil' (sem fonte)" |
| `02_etapas/etapa_04.md`, seção 6 | (lista de argumentos que podem ser usados) | Acrescentar: "É proibida a importação e a comercialização de máquina que não atenda à NR-12 (item 12.15.2) [F10]" e "Máquina certificada pelo Inmetro ou destinada só à exportação não se sujeita à norma: o diagnóstico começa por esse enquadramento [F10]" |
| `02_etapas/etapa_01_entender_solucao.md`, seção 5 | "Por que a hipótese é plausível... Máquina projetada para outro mercado pode não vir com isso." | Acrescentar: "Existem normas técnicas chinesas de segurança de máquinas, muitas equivalentes a ISO/IEC, mas isso não garante o atendimento aos requisitos brasileiros nem manual/inscrições em português [F20][F10]." |

## 4. O que continua aberto
- Valor vigente das multas em 2026 (Anexo I da NR-28, fonte primária).
- Se a Portaria 1.758/2026 alterou o enquadramento de itens específicos da NR-12 usados no discurso.
- Texto original da ISO 13855.
- Credencial e registro do professor, prazo, preços e cases (ver `plano_de_validacao_respostas_1_a_5.md`).
- Dados primários de importação (Comex Stat) por NCM 84 e 85.

## 5. Limites desta validação
- Foram consultadas fontes secundárias para NR-28, Sebraetec, ME/MEI e importações. Para o artigo, trocar por DOU/gov.br e Comex Stat.
- Não foi possível acessar as bases oficiais de multas atualizadas nem o Comex Stat nesta rodada.
