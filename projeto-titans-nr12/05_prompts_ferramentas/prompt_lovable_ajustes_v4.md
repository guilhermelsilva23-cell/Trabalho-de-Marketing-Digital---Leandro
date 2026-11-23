# Prompt de ajustes (v4) — pequenos acertos
Como usar: cole o texto entre as linhas na ferramenta, no mesmo projeto. Registre o resultado no campo ao fim.

---
## INÍCIO DO PROMPT

Faça só os ajustes abaixo. Não altere textos, layout, cores nem rotas que não forem citados.

1. TELA DE ERRO. Em src/routes/__root.tsx, o componente de erro voltou para o inglês. Traduza para português do Brasil: "Esta página não carregou", "Algo deu errado do nosso lado. Tente atualizar ou volte ao início.", botão "Tentar de novo". Mantenha igual o texto de src/lib/error-page.ts.
2. BANNER DE COOKIES. Mostre o banner somente quando GA4_ID ou META_PIXEL_ID estiver preenchido. Com os dois vazios, não exibir o banner.
3. README. Na seção "SITE_URL e sitemap", remova a frase que manda editar a rota /robots.txt e descomentar a linha Sitemap. Explique que basta preencher SITE_URL.
4. .ENV. Adicione .env ao .gitignore. Não apague o arquivo .env do projeto.
5. TESTES. Adicione um teste que confirme o banner oculto quando os dois IDs estão vazios. Rode todos os testes.

Entrega: resumo do que foi alterado, o que não foi possível e quais testes passaram.

## FIM DO PROMPT
---

## Registro do resultado (único campo a preencher)
[COLE AQUI O RESULTADO DA FERRAMENTA]
