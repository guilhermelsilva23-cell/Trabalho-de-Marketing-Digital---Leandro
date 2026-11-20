# Registro de decisões
Formato: **Decisão** | **Alternativas consideradas** | **Justificativa** | **Data**

1. Tema do grupo = NR-12 (Grupo 4 do PDF), com recorte em máquinas importadas. Justificativa: _escreva com suas palavras_.

2. **Escopo = somente NR-12.** Retrofit e automação (ideia do professor para uma segunda fase) ficam estacionados. Alternativa: manter como cross-sell. Justificativa: foco e profundidade. Data: 26/10/2026. Reavaliar ao final do ciclo 3.

3. **Duas páginas no site: institucional (`/adequacao-nr-12`, indexável) e landing do diagnóstico (`/adequacao-nr-12/diagnostico`, noindex).** Alternativa: uma página só. Justificativa: separar SEO de conversão e evitar canibalização [H]. Data: 16/11/2026.

4. **Protótipo do site por ferramenta de criação (Lovable e similares), via prompt versionado em `05_prompts_ferramentas`.** Alternativa: construir o site do zero. Justificativa: velocidade e entrega de protótipo visual exigida na Etapa 6. O resultado não vira entrega final sem revisão da Titans. Data: 16/11/2026.

5. **Paleta provisória: preto, branco e vermelho (#E10600).** O vermelho exato da marca será confirmado com a Titans; cores ficam em variáveis. Data: 16/11/2026.

6. **Stack do protótipo: TanStack Start (React/TypeScript) com SSR, gerado pela Lovable.** Alternativa: HTML estático. Justificativa: a Lovable entrega com SSR, o que atende à exigência de conteúdo no HTML (Etapa 3, alerta de indexação). O código é protótipo e só vira entrega final após os ajustes e a revisão da Titans. Data: 16/11/2026.

7. **RESOLVIDA em 18/11/2026 (ver item 8). Era: bloquear ou aceitar e-mails gratuitos no formulário.** A Lovable bloqueou (gmail, hotmail etc.), o que o prompt não pedia. Alternativas: manter o bloqueio (filtra lead, mas pode perder dono de PME, Persona 2) ou aceitar e marcar o lead como "e-mail não corporativo". O prompt v2 propõe a segunda. Decidir com a Titans. Data: 16/11/2026.

8. **Formulário aceita e-mail gratuito e marca o lead como "não corporativo" (`email_corporativo=false`).** Alternativa: manter o bloqueio. Justificativa: não perder o dono de PME (Persona 2) e ainda permitir a qualificação do lead. Data: 18/11/2026.

9. **Leads são gravados em banco do projeto (tabela `leads`), além do webhook opcional.** Alternativa: só webhook. Justificativa: evitar perda de lead enquanto o webhook não existe. Consequência: a política de privacidade precisa descrever o armazenamento (LGPD). Data: 18/11/2026.

10. **EM ABERTO: banner de consentimento para GA4 e Meta Pixel.** O prompt v3 propõe carregar os scripts só após "Aceitar". Decidir com a Titans. Data: 18/11/2026.

11. **PROPOSTA: "máquinas importadas" = campanha dentro da oferta geral, e não recorte único do projeto.** Alternativas: manter como recorte único (decisão 1); descartar o ângulo. Justificativa: H1 tem apoio qualitativo [E10][E12][E15] e de contexto [F21], mas não há evidência de que as máquinas importadas chegam sem adequação; a maioria dos projetos da carteira é de máquina velha em processo de custo baixo [E03]. Consequência se aceita: revisar a decisão 1 e a pergunta central em `01_fundamentacao_academica/hipoteses_de_pesquisa.md`. Data: 19/11/2026. **Status: proposta, o grupo decide.**

12. **PROPOSTA: incluir a Prisma (SP) no benchmarking, como 6ª empresa ou no lugar da Sulfran.** Alternativa: manter as 5 originais. Justificativa: é o concorrente mais parecido com a porta de entrada, mas com modelo diferente (gratuito x híbrido [E08]). Coleta pelo protocolo da Etapa 3, seção 5. Data: 19/11/2026. **Status: proposta, confirmar com o professor.**

13. **PROPOSTA: diagnóstico com modelo híbrido (~R$ 200; isento em projeto grande ou cliente atual), em vez do "modelo C" (cobrado com abatimento).** Alternativas: gratuito; cobrado sem abatimento; modelo C. Justificativa: é a prática real do responsável técnico [E08]. Critérios de isenção ainda precisam ser escritos. O valor é ordem de grandeza [E], não publicável como tabela. Testar em H2 (simulação S03 e, depois, campanha real [C]). Data: 19/11/2026. **Status: depende da Titans.**

14. **PROPOSTA: validar as personas por conversas com SST/manutenção fora da carteira do professor, pesquisa anônima e simulação [S], no lugar de entrevistas com compradores de importadas.** Alternativa: manter o roteiro original. Justificativa: clientes que importam tratam o fornecedor como segredo competitivo [E13]. Limitação a declarar no artigo: amostra pequena e enviesada; simulação nunca prova demanda. Data: 19/11/2026. **Status: proposta, o grupo decide.**
