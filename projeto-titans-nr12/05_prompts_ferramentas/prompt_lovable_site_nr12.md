# Prompt — Lovable / Bolt / v0 / Framer / similares
Como usar: copie tudo entre "INÍCIO DO PROMPT" e "FIM DO PROMPT" e cole na ferramenta. Depois registre o resultado no campo no final deste arquivo.

---
## INÍCIO DO PROMPT

Você é um designer e desenvolvedor web sênior, especialista em sites B2B industriais e em SEO técnico. Crie as duas páginas abaixo para a Titans Soluções de Engenharia (empresa brasileira de engenharia industrial). Idioma: português do Brasil. Os textos já estão escritos abaixo; use-os como estão, sem alterar o sentido e sem acrescentar dados.

### 1. REGRAS GERAIS
- Estilo: industrial, técnico, sóbrio e confiável. Nada de visual de startup, gradientes chamativos ou ilustrações infantis.
- Paleta: preto (#0A0A0A) como fundo de seções de destaque, branco (#FFFFFF) como fundo principal e vermelho (#E10600) apenas em CTAs, ícones, linhas e números. Cinzas de apoio: #F3F3F3 e #6B6B6B. O vermelho é provisório: defina as cores como variáveis CSS (--cor-primaria etc.) para troca fácil.
- Tipografia: uma sans-serif técnica e legível (ex.: Inter ou Barlow), títulos em peso forte.
- Mobile-first, responsivo, acessível (contraste AA, rótulos de formulário, alt em imagens, foco visível).
- Desempenho: leve, imagens otimizadas com lazy-load, sem bibliotecas desnecessárias.
- Logo: deixe um espaço reservado "LOGO TITANS" no cabeçalho e no rodapé, fácil de trocar por SVG.
- Imagens: use áreas reservadas com legenda descritiva (ex.: "FOTO: máquina com cortina de luz instalada"). Não use fotos de banco que sugiram ser da Titans.
- PROIBIDO inventar: números, percentuais, nomes de clientes, depoimentos, certificações, prêmios, valores de multa, prazos legais ou resultados. Onde faltar dado, mostre um marcador visível no formato [PREENCHER: descrição], fácil de achar no código.
- Todos os dados de contato ficam em um único arquivo de configuração: WHATSAPP_NUMERO, EMAIL_RFQ, CIDADE_UF, URL_FORMULARIO_DESTINO.

### 2. SEO TÉCNICO (obrigatório nas duas páginas)
- O conteúdo deve estar no HTML entregue ao navegador: use pré-renderização estática (SSG) ou renderização no servidor (SSR). O site atual da Titans carrega conteúdo por JavaScript, o que pode prejudicar a indexação. Se a ferramenta não permitir SSG/SSR, avise na entrega.
- HTML semântico: um único H1 por página, hierarquia H2/H3 correta, landmarks (header, main, section, footer).
- Meta title, meta description, canonical, Open Graph e URL amigável conforme definido abaixo.
- JSON-LD: Organization e Service nas duas páginas; FAQPage só na Página A. Não inclua avaliações nem dados não fornecidos.
- Gerar sitemap.xml e robots.txt. Imagens com width e height definidos.
- Links internos: a Página A aponta para a landing; a landing aponta de volta para a Página A.

### 3. PÁGINA A — "ADEQUAÇÃO NR-12" (página institucional da solução)
URL: /adequacao-nr-12
Title: Adequação NR-12 de Máquinas | Titans Engenharia
Meta description: Adequação NR-12 com engenharia: diagnóstico, apreciação de risco, projeto, validação e laudo com ART. Solicite um diagnóstico com a Titans.
H1: Adequação NR-12 de máquinas tratada como engenharia

Cabeçalho fixo com menu (Solução | Metodologia | Aplicações | Cases | Contato) e botão vermelho "Solicitar diagnóstico".

SEÇÃO 1 — HERO (fundo preto, texto branco)
- H1 acima.
- Subtítulo: Do diagnóstico ao laudo, em um só fluxo: inventário, apreciação de risco, projeto, adequação, validação e documentação, com responsável técnico e ART.
- CTA principal: "Solicite um diagnóstico NR-12" (leva à landing). CTA secundário (contorno branco): "Envie sua RFQ".
- Mídia: área reservada para vídeo ou foto de máquina industrial protegida.

SEÇÃO 2 — PROBLEMA (H2: Sua máquina está protegida e documentada?)
Texto: A NR-12 vale para máquinas novas e usadas, nacionais e importadas. Máquina sem apreciação de risco, sem sistema de segurança verificado e sem documentação expõe pessoas e empresa. Comprar o dispositivo de segurança não basta: escolha ou ligação incorreta pode anular a função de segurança.
Card de destaque: "Cerca de 15%" dos acidentes de trabalho registrados entre 2012 e 2022 envolveram máquinas e equipamentos. Fonte, em letra pequena: Observatório de Segurança e Saúde no Trabalho (SmartLab).
Três cards de dor: "Sem apreciação de risco documentada" · "Máquina importada sem verificação de conformidade" · "Laudo sem execução: o risco continua na máquina".

SEÇÃO 3 — SOLUÇÃO TITANS (H2: Um fluxo de engenharia, um responsável técnico)
Texto: A Titans conduz a máquina do diagnóstico à documentação final, com projeto, implantação e validação do sistema de segurança. Você recebe a máquina avaliada, protegida e documentada, e decide o investimento com os riscos priorizados.
Escada visual de 5 degraus numerados em vermelho: 1 Diagnóstico NR-12 · 2 Apreciação de Risco · 3 Projeto de Segurança · 4 Adequação · 5 Validação e Documentação. Texto abaixo: cada degrau pode ser contratado separadamente, ou no pacote "Titans NR-12 Completo".

SEÇÃO 4 — APLICAÇÕES (H2: Máquinas e setores atendidos)
Máquinas: prensas, dobradeiras, guilhotinas, injetoras, embaladoras, esteiras, células robotizadas e cobots, transelevadores e AGVs. Nacionais, importadas, novas e usadas.
Setores (chips): metalúrgico, autopeças, automotivo, bens de capital, alimentos e bebidas, plásticos, logística.

SEÇÃO 5 — BENEFÍCIOS (H2: O que você recebe)
- Máquina avaliada, protegida e documentada.
- Riscos priorizados por criticidade.
- Decisão de investimento baseada em apreciação de risco, não em estimativa.
- Um contrato, um responsável técnico.
- Laudo e documentação com responsabilidade técnica e ART.
Aviso pequeno ao final: "A Titans não garante ausência de autuação; entrega engenharia e documentação técnica."

SEÇÃO 6 — TECNOLOGIAS (H2: Como fazemos)
Itens com ícones: proteções fixas e móveis intertravadas; chaves de segurança; cortinas de luz; scanners e tapetes de segurança; relés e CLPs de segurança; parada de emergência; comando bimanual; projeto elétrico de comando.
Normas de referência (chips): ABNT NBR ISO 12100 · ABNT NBR ISO 13849-1/-2 · NR-12 · NR-10.

SEÇÃO 7 — METODOLOGIA (H2: Como a Titans conduz o projeto)
Linha do tempo horizontal (vertical no celular) com 6 fases. Cada fase mostra "O que acontece" e "O que você recebe":
1. Diagnóstico: inventário de máquinas, zonas de perigo e checagem de documentação. Recebe: inventário e lista de não conformidades.
2. Análise de risco: apreciação conforme ISO 12100 e priorização. Recebe: documento de apreciação de risco e PLr requerido.
3. Projeto: proteções, sensores, relés, intertravamentos, parada de emergência e projeto elétrico. Recebe: projeto mecânico e elétrico de segurança.
4. Adequação: instalação e integração das medidas. Recebe: máquina adequada fisicamente.
5. Validação: verificação do desempenho do sistema de segurança conforme ISO 13849-2. Recebe: relatório de validação.
6. Documentação: laudo de conformidade, manual em português e registros de capacitação. Recebe: pacote documental com ART.

SEÇÃO 8 — CASES (H2: Experiência comprovada)
3 cards de case com os campos: Setor · Máquina · Desafio · O que foi feito · Resultado. Preencha com [PREENCHER: case autorizado pela Titans]. Acima, faixa de logos de clientes com [PREENCHER: logos autorizados]. Não use nomes de clientes sem autorização.

SEÇÃO 9 — FAQ (H2: Perguntas frequentes), também em JSON-LD FAQPage
- A NR-12 vale para máquinas importadas? Sim. A norma se aplica a máquinas novas e usadas, nacionais ou importadas.
- Qual a diferença entre laudo e adequação? O laudo documenta a situação; a adequação implanta as medidas na máquina. A Titans conduz os dois no mesmo fluxo.
- Preciso parar a máquina? A adequação física exige uma janela de parada, planejada junto com o cliente.
- Quem assina a documentação? Profissional habilitado, com ART.
- Por onde começar? Pelo diagnóstico: ele mostra o que está fora de conformidade e a ordem de prioridade.

SEÇÃO 10 — CTA FINAL (fundo preto)
Título: Comece pelo diagnóstico. Decida com os riscos na mão.
Botões: "Solicite um diagnóstico NR-12" · "Fale com nossa engenharia" (WhatsApp) · "Envie sua RFQ".
Rodapé: logo, [PREENCHER: endereço], WHATSAPP_NUMERO, EMAIL_RFQ, links institucionais.

### 4. PÁGINA B — LANDING PAGE "DIAGNÓSTICO NR-12" (conversão)
URL: /adequacao-nr-12/diagnostico
Title: Diagnóstico NR-12 de Máquinas | Titans Engenharia
Meta description: Descubra o que está fora da NR-12 na sua máquina e o que priorizar. Solicite o diagnóstico com a engenharia da Titans.
Meta robots: noindex, follow (página de campanha).
Layout: sem menu completo, só logo e um botão. Há uma única ação na página: o formulário. Todos os CTAs rolam até ele.

BLOCO 1 — HERO (preto)
H1: Sua máquina está em conformidade com a NR-12?
Subtítulo: Descubra o que está fora da norma, o que priorizar e como corrigir, antes de decidir quanto investir.
CTA: "Solicitar diagnóstico". Linha de confiança abaixo do botão: "Engenharia com responsável técnico e ART" [PREENCHER: confirmar com a Titans antes de publicar].

BLOCO 2 — PROBLEMA (branco)
H2: Máquina sem diagnóstico é risco sem prioridade
Três itens com ícone: "Você não sabe o que está fora da norma" · "Laudo sozinho não protege o operador" · "Máquina importada pode chegar sem manual em português e sem sistema de segurança verificável".

BLOCO 3 — SOLUÇÃO (branco)
H2: O que é o Diagnóstico NR-12 da Titans
Texto: Uma avaliação de engenharia da sua máquina: inventário, identificação das zonas de perigo, checagem da documentação e lista de não conformidades priorizada.
Entregáveis (checklist): inventário da máquina · lista de não conformidades · prioridades de correção · caminho estimado de adequação [PREENCHER: confirmar o que está incluído e o prazo].
Linha de preço: [PREENCHER: gratuito ou valor de entrada; decisão pendente da Titans].

BLOCO 4 — BENEFÍCIOS (cinza claro)
H2: Por que começar pelo diagnóstico
- Escopo fechado e prazo definido [PREENCHER: prazo].
- Riscos priorizados por criticidade.
- Base para decidir o investimento sem estimar.
- Um único responsável técnico.

BLOCO 5 — CASE (branco)
H2: Experiência em máquinas industriais
Um card de case: [PREENCHER: case autorizado]. Controle por variável SHOW_CASE; enquanto for false, o bloco fica oculto.

BLOCO 6 — FORMULÁRIO (preto, destaque)
H2: Solicite seu diagnóstico
Campos: Nome · Cargo (select: Engenharia/Manutenção, Segurança do Trabalho, Gerência/Direção, Compras, Outro) · Empresa · E-mail corporativo · Telefone/WhatsApp · Tipo de máquina (select: prensa, dobradeira, guilhotina, injetora, embaladora, esteira, célula robotizada/cobot, AGV/transelevador, outra) · Origem da máquina (nacional / importada / não sei) · Quantidade de máquinas (1, 2 a 5, 6 a 20, mais de 20) · Mensagem (opcional) · Checkbox de consentimento LGPD com link para a política de privacidade.
Botão: "Solicitar diagnóstico". Mensagem de sucesso: "Recebemos sua solicitação. Nossa engenharia entra em contato em [PREENCHER: prazo]."
UTM: ler utm_source, utm_medium, utm_campaign, utm_content e utm_term da URL e enviar como campos ocultos. Enviar o formulário para URL_FORMULARIO_DESTINO (webhook) e para EMAIL_RFQ. Validação de campos e honeypot contra spam.
Eventos de análise (preparar, sem inventar IDs): form_view, form_start, form_submit, click_whatsapp, click_rfq. Deixe variáveis vazias e configuráveis para GA4 e Meta Pixel.

BLOCO 7 — RODAPÉ mínimo (logo, contatos, política de privacidade).

### 5. ENTREGA ESPERADA
1. As duas páginas funcionando e publicadas em URL de teste.
2. Lista de todos os marcadores [PREENCHER] encontrados.
3. Arquivo único de configuração com contatos, cores e variáveis.
4. Resumo do que foi implementado, do que não foi possível e das suposições feitas.

## FIM DO PROMPT
---

## Registro do resultado (único campo a preencher)
Cole abaixo o que a ferramenta fez: nome da ferramenta, data, link de teste, o que ficou diferente do prompt e a lista de [PREENCHER] pendentes.

**Ferramenta:** Lovable · **Data:** 16/11/2026
**Repositório:** https://github.com/guilhermelsilva23-cell/projeto-de-site
**Resultado:** as duas páginas foram criadas com os textos e o SEO do prompt, em TanStack Start com SSR, mais página de política de privacidade, sitemap dinâmico e logos reais.
**Diferenças e pendências:** detalhadas em `resultado_lovable_2026-11-16.md`. As principais: o formulário só envia para webhook (hoje vazio, e mesmo assim mostra sucesso), os scripts de GA4 e Pixel não são carregados, canonical relativo, e a política de privacidade está só com `[PREENCHER]`.
**Link de teste:** [PREENCHER: URL de preview da Lovable]
