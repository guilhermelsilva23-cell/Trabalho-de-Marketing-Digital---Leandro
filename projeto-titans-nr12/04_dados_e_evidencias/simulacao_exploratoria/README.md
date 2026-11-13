# Simulação exploratória com agentes de IA — protocolo (MiroFish)
**Tipo de evidência:** [S] simulado. Nunca misturar com [F] (fato) nem [E] (especialista).
**Ferramenta escolhida:** MiroFish — https://github.com/666ghj/MiroFish (consultado em 12/11/2026).
**Status:** protocolo e material de entrada prontos. **Nenhuma rodada foi executada ainda**; não existe resultado [S] neste repositório.

## 1. O que é o MiroFish (conforme o README)
- Motor de simulação multiagente: extrai "sementes" de materiais reais (notícias, relatórios, documentos), monta um mundo digital com milhares de agentes com personalidade e memória, simula a interação e gera um relatório de previsão. É possível conversar com agentes e com o agente-relator depois.
- Fluxo em 5 etapas: construção de grafo (GraphRAG), preparação do ambiente e das personas, simulação em duas plataformas paralelas, relatório, interação posterior.
- O motor de simulação usa o OASIS (camel-ai/oasis).
- Licença **AGPL-3.0**: ao modificar e oferecer o software em rede, o código modificado deve ser disponibilizado. Para uso acadêmico sem modificação, citar o repositório.
- Requisitos: Node.js 18+, Python 3.11 a 3.12, uv; chave de API de um modelo de linguagem (padrão OpenAI SDK; o README recomenda Qwen-plus) e chave do Zep Cloud. O README avisa que o consumo é alto e recomenda testar com menos de 40 rodadas.

## 2. Sobre a ideia de "prêmio"
O MiroFish **não ganhou um prêmio**: chegou ao 1º lugar do **GitHub Trending** em 07/03/2026, que é um ranking de popularidade diária. Na data da consulta, o repositório tinha ~85 mil estrelas. Popularidade não é prova de acerto: o README que li não apresenta métrica de acurácia ou validação das previsões. Por isso o resultado entra como **[S]**.

## 3. Adequação ao problema do projeto
| Ponto | Avaliação |
|---|---|
| O que a ferramenta simula | Interações sociais em plataformas parecidas com Twitter e Reddit (formação de opinião) |
| O que queremos saber | Como engenheiros, gestores e compradores reagiriam a mensagens e ofertas de NR-12, e quais objeções surgiriam |
| Encaixe | **Parcial.** Serve para testar mensagens e levantar objeções em ambiente social profissional. **Não** simula uma decisão de compra B2B com RFQ, orçamento e aprovação |
| Risco principal | Agentes são gerados por modelo de linguagem: refletem padrões do treinamento, não compradores reais |

## 4. O que pode e não pode ser feito com o resultado
| Pode | Não pode |
|---|---|
| Comparar a reação das 3 personas (Etapa 5) a 3 mensagens e 2 ofertas | Provar H1, H2 ou H3 |
| Listar objeções de preço e de prazo para tratar na landing page e nos vídeos | Estimar demanda, volume ou disposição a pagar |
| Gerar hipóteses e perguntas para entrevistas reais | Substituir entrevistas e o teste real de mídia (Etapa 11) |
| Justificar o desenho do experimento A/B | Aparecer no artigo como resultado de mercado |

## 5. Passo a passo para o grupo
1. Clonar o repositório e configurar `.env` (LLM e Zep). Anotar modelo, versão e data.
2. Carregar `seed_nr12_titans.md` como material-semente.
3. Informar `requisito_de_previsao.md` como pedido de previsão.
4. Rodar **piloto com menos de 40 rodadas** e salvar relatório, número de agentes e parâmetros.
5. Repetir **pelo menos 3 vezes** cada cenário para ver a variação entre execuções.
6. Registrar tudo em `registro_de_rodadas.md` (cada linha com status [S]).
7. Comparar com os relatos reais do professor (E05, E08, E09, E14). Divergências viram perguntas para a entrevista.

## 6. Como citar no artigo
"Simulação exploratória com agentes de linguagem (MiroFish, repositório 666ghj/MiroFish, licença AGPL-3.0), usada para geração de hipóteses e teste de mensagens; não constitui evidência de demanda." Declarar modelo, rodadas, parâmetros e versão do repositório.

## 7. Alternativa de menor custo (se o MiroFish consumir demais a cota da API)
Entrevistas simuladas manuais com as 3 personas, com o mesmo `seed_nr12_titans.md`, em um modelo de linguagem comum. Também é [S] e vale as mesmas ressalvas.
