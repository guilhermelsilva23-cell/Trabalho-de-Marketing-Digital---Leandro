# Simulação exploratória com agentes de IA — protocolo
**Tipo de evidência:** [S] simulado. Nunca misturar com [F] (fato) nem [E] (especialista).
**Status:** protocolo definido; aplicação ainda não adaptada ao cenário NR-12. Falta indicar o repositório da aplicação usada como base (campo abaixo).

## 1. Objetivo
Testar mensagens, ofertas e objeções de preço do diagnóstico e da adequação NR-12 com personas simuladas, **antes** de gastar mídia e para gerar perguntas de entrevistas reais.

## 2. O que a simulação pode e não pode fazer
| Pode | Não pode |
|---|---|
| Comparar a reação das 3 personas (Etapa 5) a mensagens e ofertas | Provar H1, H2 ou H3 |
| Antecipar objeções de preço e de prazo | Estimar demanda, volume ou disposição a pagar |
| Gerar hipóteses e perguntas para entrevistas | Substituir pesquisa com compradores reais |
| Justificar o desenho do experimento de mídia (Etapa 11) | Aparecer no artigo como resultado de mercado |

Motivo: os respondentes são gerados por modelo de linguagem e refletem padrões do treinamento, não compradores reais.

## 3. Cenário NR-12 (a preencher e fixar antes de rodar)
- **Repositório/aplicação base:** `[PREENCHER link]`
- **Modelo e versão:** `[PREENCHER]`
- **Número de agentes por persona:** `[PREENCHER]`
- **Rodadas por mensagem:** `[PREENCHER]`
- **Parâmetros (temperatura etc.):** `[PREENCHER]`
- **Prompts usados:** salvar em `prompts/` (um arquivo por rodada)

### Ancoragem das personas em dados reais [E]
| Parâmetro | Valor de referência | Fonte |
|---|---|---|
| Região | SP capital e raio de ~200 km | E01 |
| Ticket da adequação (máquina pequena) | ~R$ 8 mil (até ~R$ 20 mil) | E09 |
| Diagnóstico | ~R$ 200; isento em cliente atual ou projeto grande | E08 |
| Perfil do cliente | Máquina velha, custo baixo, compra reativa após risco ou acidente | E03, E05 |
| Objeções reais a incluir | "NR-12 é custo" · "não é prioridade" · aprovou e não executou · "já tenho laudo" | Etapa 5, E14 |
| Responsável técnico | Um engenheiro mestre e doutor que assina | E06 |
| Máquina importada | Esquema em mandarim; sem código-fonte do CLP | E10 |

### Variáveis a testar
1. **Preço do diagnóstico:** gratuito x R$ 200 x valor intermediário.
2. **Mensagem:** técnica (engenharia, ISO 12100/13849) x risco (acidente, multa) x inércia ("risco já identificado").
3. **Oferta de entrada:** "Diagnóstico NR-12" x "Check-up NR-12 para máquina importada".
4. **Persona:** técnica, decisora e compras.

## 4. Como comparar com a realidade
Comparar a saída simulada com o relato real do professor (E05, E08, E09, E14). Registrar concordâncias e divergências. Divergência não invalida nem confirma: vira pergunta para a entrevista.

## 5. Como citar no artigo
"Simulação exploratória com agentes de linguagem, usada para geração de hipóteses e teste de mensagens; não constitui evidência de demanda." Declarar modelo, prompts, rodadas e parâmetros no método.

## 6. Registro de rodadas
Usar `registro_de_rodadas.md`.
