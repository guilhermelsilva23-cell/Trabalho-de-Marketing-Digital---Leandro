# Prompt de ajustes (v3)
Como usar: cole o texto entre as linhas na ferramenta, no mesmo projeto. Registre o resultado no campo ao fim.
Antes de enviar, decidir o item 4 (banner de cookies) com a Titans; se não quiserem, apague o item.

---
## INÍCIO DO PROMPT

Faça só os ajustes abaixo. Não altere textos, layout, cores nem rotas que não forem citados.

1. BANCO. Crie uma nova migração que remova a permissão de INSERT para o papel anon e a política "Qualquer visitante pode enviar um lead" na tabela leads. O envio continua pelo servidor com a chave de serviço. Confirme que o formulário segue gravando leads após a mudança.
2. WEBHOOK. Em src/lib/lead.functions.ts, grave o campo encaminhado_webhook como false na criação do lead e atualize para true somente depois de o webhook responder com sucesso. Se o webhook falhar, retorne sucesso ao visitante (o lead já está salvo) e registre o erro no log.
3. AVISO DE NOVO LEAD. Se houver conector de e-mail disponível, envie notificação para EMAIL_RFQ a cada novo lead. Se não houver, não invente: apenas informe na resposta o que é necessário para ativar.
4. COOKIES. Adicione um banner de consentimento simples em português, com "Aceitar" e "Recusar". Os scripts de GA4 e Meta Pixel só carregam depois de "Aceitar". A escolha fica salva no navegador. O link do banner aponta para /politica-de-privacidade.
5. ROBOTS. Transforme /robots.txt em rota dinâmica que inclua "Sitemap: {SITE_URL}/sitemap.xml" quando SITE_URL estiver preenchido e mantenha as regras atuais. Remova o arquivo estático public/robots.txt.
6. README e ROADMAP. No README, troque "No editor Lovable, clique em Publish" por instruções de publicação genéricas e explique onde ver os leads salvos (tabela leads). Atualize o roadmap.md marcando o que já foi feito e mantendo só o que falta.
7. TESTES. Adicione testes para os itens 2 e 5. Rode todos os testes.

Entrega: resumo do que foi alterado, o que não foi possível e quais testes passaram.

## FIM DO PROMPT
---

## Registro do resultado (único campo a preencher)
[COLE AQUI O RESULTADO DA FERRAMENTA]
