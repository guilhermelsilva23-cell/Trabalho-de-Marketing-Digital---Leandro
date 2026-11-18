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
