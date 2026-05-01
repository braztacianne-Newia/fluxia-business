# Fluxia Business — Growth Hacking para Salões, Clínicas e Pequenos Negócios

Projeto real de Growth Hacking e automação digital para salões de beleza, clínicas de estética e pequenos negócios, desenvolvido do zero em menos de 30 dias.

---

## 📌 Sobre o Projeto

A Fluxia Business é uma consultoria especializada em crescimento digital. Utilizamos estratégias de **Growth Hacking** para estruturar funil de captação, anúncios no Meta Ads, automação de atendimento com IA e acompanhamento de resultados em tempo real.

A dor que resolvemos: donos de salões e clínicas perdem em média 48 horas por mês em tarefas repetitivas e ficam invisíveis no digital — sem funil, sem automação, sem estrutura.

- **Site ao vivo:** fluxiabusiness.netlify.app
- **Dashboard interno:** fluxiabusiness.netlify.app/dashboard
- **Instagram:** @fluxia_business
- **LinkedIn:** Fluxia Business
- **WhatsApp:** (11) 95292-8873

---

## 🚀 O que foi construído

### 1. Landing Page *(atualizada — maio 2026)*
- HTML/CSS puro, responsivo, sem frameworks
- Posicionamento atualizado para **Growth Hacking** — salões, clínicas e pequenos negócios
- Design editorial com identidade visual consistente
- 3 pacotes de preço — Starter R$997, Pro R$2.500, Full R$4.500
- Formulário de captação integrado via Tally.so
- Pixel do Meta ativo e rastreando visitas
- **Botão flutuante do WhatsApp** com tooltip animado e mensagem automática pré-preenchida
- Hospedagem gratuita via Netlify

### 2. Funil de Captação Automático
- Formulário de leads via Tally.so
- Integração Tally → Brevo via Make.com (webhook)
- Sequência de 5 emails automáticos em 7 dias
- Gatilho: lead entra na lista → emails disparam sozinhos

### 3. Sequência de Email Marketing
- 5 emails configurados no Brevo
- Personalização com variáveis dinâmicas
- Delays configurados: 0, 1, 3, 5 e 7 dias
- Email 5 com link direto para pagamento via Kiwify

### 4. Produto e Pagamento
- 3 produtos configurados na Kiwify:
  - **Starter:** R$997 — 1 automação completa
  - **Pro:** R$2.500 — 3 automações integradas
  - **Full:** R$4.500 — 5 automações + suporte estendido
- Checkout com cartão, boleto e Pix
- Parcelamento em até 12x

### 5. Chatbot com IA — Instagram Direct
- Fluxo conversacional construído no Typebot
- Integração com OpenAI GPT-4o mini via API
- 4 fluxos principais: Serviços, Preços, Falar com equipe, Outros assuntos
- Resposta automática configurada no Meta Business Suite

### 6. Onboarding Automático Pós-Venda
Sistema completo disparado automaticamente após cada compra na Kiwify.

```
Cliente paga na Kiwify
        ↓
Kiwify dispara Webhook
        ↓
Make.com recebe e adiciona contato no Brevo
        ↓
Brevo dispara email com link do briefing
        ↓
Cliente preenche formulário (Tally.so)
        ↓
Entrega em até 7 dias
```

### 7. Campanha Meta Ads
- Campanha ativa com R$15/dia
- Criativo: Reel antes e depois
- Público: donos de salões e clínicas no Brasil
- Pixel conectado e rastreando conversões

### 8. Google Ads *(configurado — abril 2026)*
- Campanha configurada e salva como rascunho
- Orçamento planejado: R$20/dia
- Palavras-chave segmentadas por nicho
- Crédito de R$1.200 disponível para ativar

### 9. Dashboard Interno *(novo — maio 2026)*
Dashboard interativo em HTML puro para acompanhamento interno de todos os clientes.

**KPIs monitorados:**
- Leads gerados
- Taxa de conversão
- Custo por lead
- Faturamento
- Agendamentos

**Funcionalidades:**
- Seletor de cliente — suporte a múltiplos clientes
- Filtro de período: 7, 30 e 90 dias
- Gráfico de evolução de leads
- Funil de conversão visual
- Agendamentos recentes com status
- Faturamento por serviço
- Canais de aquisição com gráfico
- Conexão com Google Sheets — atualização em tempo real
- Painel de atualização manual de dados

**URL:** fluxiabusiness.netlify.app/dashboard

### 10. Dashboard do Cliente *(novo — maio 2026)*
Versão limpa e profissional do dashboard para entregar ao cliente como produto.

**Diferenças do dashboard interno:**
- Mostra apenas os dados do cliente específico
- Sem painel de edição manual
- Header com Fluxia Business + nome do salão/clínica
- Resumo executivo automático em texto
- Barra de progresso por KPI mostrando % da meta
- Seção de destaques e insights do período
- Rodapé com WhatsApp da Fluxia para contato
- Link personalizado por cliente

**Como personalizar por cliente:**
1. Duplicar o arquivo `dashboard-cliente.html`
2. Alterar `CLIENT_NAME` e `CLIENT_ROW`
3. Subir no Netlify com nome do cliente

**Exemplo:** fluxiabusiness.netlify.app/salao-piloto-01

### 11. Google Sheets — Banco de Dados *(novo — maio 2026)*
- Planilha pública conectada aos dashboards
- Colunas: Cliente | Leads | Conversão | CPL | Faturamento | Agendamentos
- 4 clientes piloto configurados
- Atualização manual por enquanto — integração Make.com planejada

### 12. Presença Digital e Perfis Freelancer
- Instagram: @fluxia_business
- LinkedIn: Fluxia Business
- Google Business criado e otimizado ✅
- Perfil Workana: 100% completo
- **99Freelas Pro:** assinatura ativa — 3 propostas enviadas ✅
- WhatsApp Business: (11) 95292-8873 ✅

### 13. Lista de Prospecção *(novo — maio 2026)*
- 118 contatos extraídos via Instant Data Scraper do Google Maps
- Segmento: salões de beleza, barbearias e clínicas de estética em São Paulo
- Classificação em Modelo A (presença digital) e Modelo B (sem presença)
- Abordagens ativas via Instagram e WhatsApp
- Meta: 13 contatos por dia no Instagram + 6 no Workana/99Freelas

### 14. Materiais de Vendas
- **Guia de Objeções** — 5 objeções com respostas e dicas
- **Script de Abordagem Instagram** — 5 etapas + 3 modelos personalizados
- **Modelo de mensagem padrão** — adaptável por perfil sem soar genérico

### 15. Propostas Freelancer Enviadas *(novo — maio 2026)*
- **Agente de IA para atendimento** — Typebot + GPT + WhatsApp — R$850
- **Automação de atendimento comercial** — CHATCENTER + Make + Sheets — R$997
- **Automação Make + Gmail + Google Sheets** — disparo automático de emails — R$350

---

## 🛠️ Stack Tecnológica

| Categoria | Ferramenta | Função |
|-----------|------------|--------|
| Frontend | HTML/CSS puro | Landing page e dashboards |
| Hospedagem | Netlify | Deploy gratuito |
| Formulário leads | Tally.so | Captação de leads |
| Formulário briefing | Tally.so | Onboarding de clientes |
| Automação | Make.com | Integração entre ferramentas |
| Email | Brevo | Sequência automática + onboarding |
| Chatbot | Typebot | Fluxo conversacional |
| IA | OpenAI GPT-4o mini | Respostas inteligentes |
| Pagamento | Kiwify | Checkout e gestão de produtos |
| Social | Meta Business Suite | Automação e agendamento |
| Tráfego pago | Meta Ads | Campanha ativa R$15/dia |
| Tráfego pago | Google Ads | Configurado — aguardando ativação |
| Presença local | Google Business | Perfil da empresa |
| Banco de dados | Google Sheets | KPIs dos clientes |
| Freelancer | Workana | Prospecção de clientes |
| Freelancer | 99Freelas Pro | Prospecção + propostas |
| WhatsApp | WhatsApp Business | Atendimento e prospecção |
| Prospecção | Instant Data Scraper | Extração de leads Google Maps |
| Versionamento | GitHub | Documentação e portfólio |

---

## 🔄 Arquitetura Completa do Sistema

```
CAPTAÇÃO PASSIVA
Visitante → Landing Page (Netlify)
         → Botão WhatsApp flutuante → Conversa direta
         → Formulário (Tally.so)
         → Make.com [webhook]
         → Lista Brevo — "Leads Agência FLUXIA"
         → 5 emails automáticos em 7 dias
         → Email 5: Link de pagamento (Kiwify)

CAPTAÇÃO ATIVA
Lista 118 contatos (Google Maps SP)
         → Instagram 13/dia — Modelo A e B
         → WhatsApp Business
         → Propostas Workana
         → Propostas 99Freelas Pro (3/dia)
         → Meta Ads R$15/dia (paralelo)
         → Google Ads R$20/dia (quando ativar)

VENDA & ONBOARDING
Cliente paga (Kiwify)
         → Webhook → Make.com
         → Brevo — "Clientes Fluxia Business"
         → Email de boas-vindas + briefing
         → Formulário Tally → entrega em 7 dias

ATENDIMENTO
Instagram Direct
         → Auto reply (Meta Business Suite)
         → Typebot + GPT-4o mini
         → Qualificação → Landing page

ACOMPANHAMENTO
Dashboard interno (fluxiabusiness.netlify.app/dashboard)
         → Todos os clientes
         → KPIs em tempo real via Google Sheets
         → Funil, agendamentos, faturamento, canais

Dashboard do cliente (fluxiabusiness.netlify.app/nome-cliente)
         → Dados específicos do cliente
         → Resumo executivo automático
         → Insights do período
```

---

## 📊 Projeção de Resultados

### Mês 1 — 30 dias de execução

| Canal | Contatos/dia | Total mês | Conversas | Clientes (15%) |
|-------|-------------|-----------|-----------|----------------|
| Instagram | 13 | 390 | ~39 | ~6 |
| Workana | 3 | 90 | ~6 | ~1 |
| 99Freelas | 3 | 90 | ~6 | ~1 |
| Meta Ads | — | ~12 leads | ~12 | ~2 |
| **Total** | **19** | **~580** | **~63** | **~10** |

**Faturamento estimado mês 1:**
- Conservador (10%): R$6.000 — R$8.000
- Realista (15%): R$10.000 — R$12.000
- Otimista (20%): R$14.000 — R$16.000

---

## ✅ Status do Projeto

### Fase 1 — Estrutura (concluída)
- [x] Landing page com Growth Hacking + botão WhatsApp
- [x] Funil de captação (Tally → Brevo → 5 emails)
- [x] 3 produtos na Kiwify
- [x] Chatbot com IA (Typebot + GPT-4o mini)
- [x] Onboarding automático pós-venda
- [x] Meta Ads ativo (R$15/dia)
- [x] Google Ads configurado
- [x] Google Business criado
- [x] WhatsApp Business configurado
- [x] Perfis Workana e 99Freelas Pro
- [x] Dashboard interno com Google Sheets
- [x] Dashboard do cliente personalizado
- [x] 118 leads extraídos e classificados
- [x] Guia de objeções e script de abordagem
- [x] Abordagens ativas iniciadas
- [x] 3 propostas enviadas no 99Freelas

### Em andamento
- [ ] Abordagens diárias — 13 Instagram + 6 Workana/99Freelas
- [ ] Primeiro cliente piloto com depoimento em vídeo
- [ ] Verificação do Instagram para liberar Direct
- [ ] Integração Make.com → Google Sheets (Meta Ads + Kiwify)

### Fase 2 — Escala (planejada)
- [ ] ERP conectado ao funil completo
- [ ] Relatório automatizado via Make.com
- [ ] Dashboard com dados automáticos das ferramentas
- [ ] Expansão para outros nichos
- [ ] Contratação de assistente operacional

---

## 📁 Estrutura do Repositório

```
fluxia-business/
│
├── index.html                          # Landing page Growth Hacking + WhatsApp
├── dashboard.html                      # Dashboard interno — todos os clientes
├── dashboard-cliente.html              # Dashboard do cliente — template
│
├── emails/
│   └── emails-brevo-fluxia.html        # 5 emails da sequência automática
│
├── automacoes/
│   └── FLUXIA_BUSINESS_AUTOMACAO.md    # Documentação técnica do onboarding
│
├── materiais-vendas/
│   ├── guia-objecoes-fluxia.docx       # 5 objeções com respostas prontas
│   └── script-instagram-fluxia.docx   # Script de abordagem em 5 etapas
│
├── prospeccao/
│   └── lista_leads_fluxia.xlsx         # 118 leads classificados SP
│
├── posts/
│   ├── post2-case-clinica.html
│   ├── post3-dica-valor.html
│   ├── post4-prova-social.html
│   ├── post5-como-funciona.html
│   ├── post6-oferta-lancamento.html
│   └── reels-post2-frames.html
│
├── identidade-visual/
│   ├── perfil-instagram-fluxia.svg
│   ├── banner-linkedin-v2.html
│   └── imagem-produto-fluxia-business.svg
│
├── planejamento/
│   └── calendario-maio-2026.md
│
└── README.md
```

---

## 💡 Decisões Técnicas

**Por que Growth Hacking e não social media tradicional?**
Growth Hacking entrega sistema que cresce sozinho — funil automatizado, dados, otimização contínua. O cliente precisa de resultado, não só de presença.

**Por que HTML puro em vez de React ou Next.js?**
Performance crítica para páginas de conversão. HTML/CSS puro carrega mais rápido, sem dependências, hospedagem gratuita.

**Por que Make.com em vez de Zapier?**
1.000 operações gratuitas por mês vs 100 do Zapier.

**Por que Brevo em vez de Mailchimp?**
Automações completas no plano gratuito.

**Por que Kiwify em vez de Hotmart?**
Interface mais simples e checkout mais limpo.

**Por que GPT-4o mini em vez de GPT-4o?**
Custo ~10x menor com qualidade suficiente para atendimento conversacional.

**Por que dashboard em HTML puro em vez de Power BI ou Looker?**
Zero custo, hospedado no Netlify, acesso por link direto, sem login, personalizável por cliente.

**Por que Google Sheets como banco de dados?**
Gratuito, familiar pro cliente, fácil de atualizar, integra com Make.com e com o dashboard via CSV público.

---

## 👩‍💻 Sobre a Autora

Desenvolvido por **Tacianne Braz** como projeto prático aplicado durante estudos em Data Science, Analytics e Inteligência Artificial.

Este projeto demonstra na prática:
- Growth Hacking aplicado a negócios locais
- Integração de múltiplas APIs e plataformas no-code/low-code
- Automação de funil de vendas completo
- Aplicação de LLMs em produto real
- Prospecção ativa e estratégia de vendas B2B
- Design e desenvolvimento frontend
- Arquitetura de sistemas de atendimento automatizado
- Estratégia de conteúdo e marketing digital orientado a dados

---

## 📬 Contato

- **Site:** fluxiabusiness.netlify.app
- **WhatsApp:** (11) 95292-8873
- **Instagram:** @fluxia_business
- **LinkedIn:** Fluxia Business

---

*Última atualização: maio 2026*
