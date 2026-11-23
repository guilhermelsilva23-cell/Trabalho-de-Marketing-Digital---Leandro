# Etapa 13 — Landing page (NR-12)

**Status:** [~] landing gerada na Lovable (16/11/2026) e revisada pelo código; não publicada. Falta destino dos leads, preço/prazo e política de privacidade.
**Entregável do PDF:** 22 (landing page)
**Onde está o briefing e o texto:** `05_prompts_ferramentas/prompt_lovable_site_nr12.md`, seção 4 (Página B)

## Resumo
- **URL:** `/adequacao-nr-12/diagnostico` (noindex, para campanha)
- **Oferta:** Diagnóstico NR-12 (degrau 1 da escada, Etapa 4). Preço: `[PREENCHER]` (decisão pendente: cobrado ou gratuito).
- **Estrutura:** Problema → Solução → Benefícios → Case → Formulário (como pede o PDF)
- **Conversão:** formulário com cargo, tipo e origem da máquina, quantidade, UTMs ocultas e consentimento LGPD
- **Eventos a medir:** form_view, form_start, form_submit, click_whatsapp, click_rfq

## Pendências
- [x] Resultado da ferramenta registrado (`resultado_lovable_2026-11-16.md`)
- [x] Leads agora são salvos no banco do projeto mesmo sem webhook (v2, 18/11/2026)
- [x] E-mail gratuito aceito, com marcação `email_corporativo` (decisão 8)
- [ ] Definir quem consulta os leads e ligar webhook ou e-mail de aviso (hoje ninguém é notificado)
- [x] Permissão de INSERT anônimo removida no código (migração `0001`, 23/11/2026); falta confirmar que rodou no banco real
- [x] Banner de cookies implementado (scripts de analytics só após "Aceitar")
- [ ] Definir preço e prazo do diagnóstico com a Titans
- [ ] Case autorizado (ou manter o bloco oculto)
- [ ] Ligar a campanha (Etapa 12) e a mídia (Etapa 11) a esta página
