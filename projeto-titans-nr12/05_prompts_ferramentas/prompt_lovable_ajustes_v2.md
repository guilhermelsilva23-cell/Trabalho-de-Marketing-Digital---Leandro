# Prompt de ajustes (v2) — Lovable
Como usar: cole o texto entre as linhas no chat da Lovable, no mesmo projeto. Depois registre o resultado no campo no fim.
Decisão pendente antes de enviar: item 2 (e-mail corporativo). Apague o item 2 do prompt se o grupo preferir manter o bloqueio.

---
## INÍCIO DO PROMPT

Faça os ajustes abaixo no projeto atual. Não altere textos, layout, cores nem rotas que não forem citados.

1. ENVIO DE LEADS. Em src/lib/lead.functions.ts, se URL_FORMULARIO_DESTINO estiver vazia, não retorne sucesso: salve o lead no banco do próprio projeto (ou, se não for possível, retorne erro com a mensagem "Não foi possível enviar agora. Fale pelo WhatsApp."). Se o webhook estiver configurado, envie ao webhook como hoje. Se houver conector de e-mail disponível, envie também uma notificação para EMAIL_RFQ; se não houver, informe na resposta.
2. E-MAIL. Em src/lib/lead.ts, pare de bloquear e-mails gratuitos (gmail, hotmail etc.). Mantenha a validação de formato e inclua no pacote enviado o campo email_corporativo (true ou false). Mantenha o rótulo "E-mail".
3. HONEYPOT. Se o campo website vier preenchido, o servidor deve retornar sucesso sem encaminhar o lead, sem lançar erro de validação.
4. ANALYTICS. Em src/lib/analytics.ts e no layout raiz, carregue o script do GA4 apenas se GA4_ID estiver preenchido e o do Meta Pixel apenas se META_PIXEL_ID estiver preenchido. Com os IDs vazios, nada deve ser carregado. Mantenha o push no dataLayer. Na Landing, mantenha os eventos form_view, form_start e form_submit.
5. URL ABSOLUTA. Adicione SITE_URL em src/config/site.ts (vazio por padrão, com comentário [PREENCHER: domínio com https://]). Quando preenchido, use-o em canonical, og:url e no sitemap.xml. Quando vazio, mantenha o comportamento atual.
6. ROBOTS. Em public/robots.txt, adicione a linha "Sitemap: {SITE_URL}/sitemap.xml" quando SITE_URL existir, e mantenha a regra atual. Documente no README como preencher.
7. TELA DE ERRO. Traduza a tela de erro para português do Brasil ("Esta página não carregou", "Algo deu errado do nosso lado. Tente atualizar ou volte ao início.", botão "Tentar de novo").
8. LOGOS. Mantenha os logos no projeto de forma que fiquem salvos no repositório (por exemplo, em public/), não apenas no armazenamento da Lovable.
9. README. Reescreva o README em português: o que é o projeto, as rotas, onde ficam as configurações (src/config/site.ts e src/styles.css) e como publicar. Remova a frase "espere eu mandar a outra parte do prompt".
10. Rode os testes existentes e adicione um teste para o honeypot e outro para o caso de URL_FORMULARIO_DESTINO vazia.

Entrega: resumo do que foi alterado, o que não foi possível e quais testes passaram.

## FIM DO PROMPT
---

## Registro do resultado (único campo a preencher)
**Ferramenta informada:** Bolt.new (o código tem marcas da Lovable; confirmar) · **Data:** 18/11/2026
**Repositório:** https://github.com/guilhermelsilva23-cell/projeto-de-site
**Resultado:** 9 dos 10 itens atendidos; o item 6 (robots) ficou parcial e a notificação por e-mail do item 1 não foi feita. 10 testes passam (rodados na revisão).
**Detalhes e pontos de atenção:** `resultado_ajustes_v2_2026-11-18.md`.
