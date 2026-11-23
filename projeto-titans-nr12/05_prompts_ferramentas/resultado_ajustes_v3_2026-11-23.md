# Resultado dos ajustes v3 — 23/11/2026
**Prompt usado:** `prompt_lovable_ajustes_v3.md`
**Código revisado:** ZIP `projeto-de-site-main_1.zip` (repositório `projeto-de-site`)
**Método:** comparação com a versão v2 e leitura do código. Rodei os testes: **4 arquivos e 15 testes passaram**. Não rodei o build, não abri o site publicado e não consegui ver o banco real (só os arquivos de migração).

---

## 1. Conferência item a item

| # | Pedido | Resultado | Situação |
|---|---|---|---|
| 1 | Remover INSERT anônimo no banco | Migração `0001_leads_somente_servidor.sql` retira a política e revoga o INSERT de `anon`. O servidor segue gravando com a chave de serviço | Atendido no código. **Falta confirmar que foi aplicada no banco real** |
| 2 | `encaminhado_webhook` só após sucesso | Lead nasce com `false`; vira `true` quando o webhook responde bem. Se o webhook falha, o visitante recebe sucesso e o erro vai ao log | Atendido (3 testes novos) |
| 3 | Aviso de novo lead por e-mail | Não feito; o comentário no código explica que exige domínio de e-mail verificado | Não atendido (dependência da Titans) |
| 4 | Banner de cookies | `CookieBanner` com "Recusar" e "Aceitar" de peso igual; GA4 e Pixel só carregam depois de "Aceitar" e se houver ID; escolha salva no navegador | Atendido |
| 5 | `robots.txt` dinâmico | Rota `/robots.txt` com função `montarRobots`; linha `Sitemap:` aparece quando `SITE_URL` está preenchido; arquivo estático removido | Atendido (2 testes) |
| 6 | README e roadmap | README sem referência à Lovable no trecho de publicação, com seções "Onde ver os leads" e "robots.txt"; roadmap reorganizado em "Feito" e "Falta" | Atendido, com um erro no README (ver 2.3) |
| 7 | Testes | 15 testes passando, incluindo robots e webhook | Atendido |

## 2. Pontos de atenção

1. **Regressão na tela de erro.** A tela de erro do `__root.tsx` voltou para o inglês ("This page didn't load", "Try again"). O ajuste v2 (item 7) havia traduzido. O arquivo `error-page.ts` segue em português, então só o componente da página voltou.
2. **Banner aparece mesmo sem IDs de analytics.** Com `GA4_ID` e `META_PIXEL_ID` vazios, o banner pergunta sobre cookies que nada usa. Hoje o efeito é só visual.
3. **README com frase desatualizada:** manda "editar a rota /robots.txt e descomentar a linha Sitemap", mas o robots agora é automático. Basta preencher `SITE_URL`.
4. **`.env` dentro do repositório** e fora do `.gitignore`. O conteúdo é a URL e a chave pública do Supabase (não é a chave de serviço, que fica no ambiente de hospedagem), então o risco é baixo, mas o arquivo deveria ser ignorado. Com o repositório público e o INSERT anônimo removido, a tabela de leads fica protegida, desde que a migração `0001` esteja aplicada no banco.
5. **Pasta `supabase/migrations` removida;** restam as migrações em `drizzle/migrations`. Conferir no painel do banco se a tabela e as políticas estão como esperado.
6. **Roadmap não cita mais o 404** do domínio publicado, e "Publicar após cada rodada" segue aberto. Continuo sem saber se o site está no ar.

## 3. O que falta para publicar

- [ ] Texto da política de privacidade (cita armazenamento de leads e cookies)
- [ ] Dados da Titans em `src/config/site.ts`: WhatsApp, e-mail de RFQ, cidade/UF, endereço, prazo, domínio (`SITE_URL`), webhook
- [ ] Preço e escopo do diagnóstico; cases e logos autorizados
- [ ] Alguém responsável por ver os leads (ou webhook/e-mail ligado)
- [ ] Confirmar que a migração `0001` rodou no banco
- [ ] Corrigir a tela de erro em português (prompt v4)
- [ ] Publicar e conferir no celular e no computador

## 4. Próximo passo
Ajustes pequenos em `prompt_lovable_ajustes_v4.md`.
