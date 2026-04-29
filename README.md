# Fluxia Business — Growth Hacking para Salões, Clínicas e pequenos negócios

Projeto real de Growth Hacking e automação digital para salões de beleza, clínicas de estética e pequenos negócios, desenvolvido do zero em menos de 30 dias.

---

## 📌 Sobre o Projeto

A Fluxia Business é uma consultoria especializada em crescimento digital para salões de beleza, clínicas de estética e pequenos negócios. Utilizamos estratégias de **Growth Hacking** para estruturar funil de captação, anúncios no Meta Ads, automação de atendimento com IA e acompanhamento de resultados em tempo real.

A dor que resolvemos: donos de salões e clínicas perdem em média 48 horas por mês em tarefas repetitivas e ficam invisíveis no digital — sem funil, sem automação, sem estrutura.

- **Site ao vivo:** fluxiabusiness.netlify.app
- **Instagram:** @fluxia_business
- **LinkedIn:** Fluxia Business
- **WhatsApp:** (11) 95292-8873

---

## 🚀 O que foi construído

### 1. Landing Page
- HTML/CSS puro, responsivo, sem frameworks
- Design editorial com identidade visual consistente (paleta dourada e escura)
- 3 pacotes de preço — Starter R$997, Pro R$2.500, Full R$4.500
- Seções: hero, métricas, como funciona, resultados reais, serviços, dados de mercado, pacotes, história da fundadora, formulário
- Formulário de captação integrado via Tally.so
- Pixel do Meta ativo e rastreando visitas
- **Botão flutuante do WhatsApp** com tooltip animado e mensagem automática pré-preenchida *(novo — abril 2026)*
- Hospedagem gratuita via Netlify

### 2. Funil de Captação Automático
- Formulário de leads via Tally.so
- Integração Tally → Brevo via Make.com (webhook)
- Sequência de 5 emails automáticos em 7 dias
- Gatilho: lead entra na lista → emails disparam sozinhos

### 3. Sequência de Email Marketing
- 5 emails configurados no Brevo
- Personalização com variáveis dinâmicas (`{{ contact.FIRSTNAME }}`, `{{ contact.SEGMENTO }}`, `{{ contact.DOR }}`)
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
- 4 fluxos principais:
  - Serviços — apresentação completa
  - Preços — 3 pacotes com valores
  - Falar com a equipe — redirecionamento para landing page
  - Outros assuntos — resposta livre com IA
- Resposta automática configurada no Meta Business Suite
- Link do Typebot enviado automaticamente no primeiro contato

### 6. Onboarding Automático Pós-Venda
Sistema completo de onboarding disparado automaticamente após cada compra confirmada na Kiwify.

**Fluxo:**
```
Cliente paga na Kiwify
        ↓
Kiwify dispara Webhook (evento: Compra Aprovada)
        ↓
Make.com recebe e adiciona contato no Brevo
        ↓
Brevo adiciona cliente na lista "Clientes Fluxia Business"
        ↓
Brevo dispara email automático com link do briefing
        ↓
Cliente preenche formulário de briefing (Tally.so)
        ↓
Equipe Fluxia inicia a entrega em até 7 dias
```

**Componentes configurados:**
- Webhook Kiwify → Make.com (evento: Compra Aprovada)
- Cenário Make.com: `Integration Webhooks, Brevo`
- Lista Brevo: `Clientes Fluxia Business (#6)`
- Automação Brevo: `Briefing - Nova Compra`
- Formulário de briefing Tally: `https://tally.so/r/BzLbRA`

### 7. Campanha Meta Ads
- Campanha ativa com R$15/dia
- Criativo: Reel antes e depois
- Público: donos de salões e clínicas no Brasil
- Pixel do Meta conectado e rastreando conversões
- Pontuação de oportunidade: 100 pontos

### 8. Google Ads *(configurado — abril 2026)*
- Campanha configurada e salva como rascunho
- Meta: leads pelo site
- Orçamento planejado: R$20/dia
- Palavras-chave segmentadas:
  - marketing digital salão de beleza
  - marketing digital clínica estética
  - growth hacking pequenas empresas
  - gestão digital salão São Paulo
  - como atrair clientes salão
  - marketing digital consultório odontológico
  - marketing digital imobiliária
  - e outras 5 variações
- Crédito de R$1.200 disponível para ativar quando houver primeiro cliente

### 9. Presença Digital e Perfis Freelancer
- Instagram: @fluxia_business
- LinkedIn: Fluxia Business
- **Google Business** criado com descrição otimizada *(novo — abril 2026)*
- Perfil Workana: 100% completo com case real e SEO
- Perfil 99Freelas: 100% completo com histórico profissional
- Calendário de conteúdo — 19 posts planejados para abril/maio 2026

### 10. Dashboard de Métricas *(novo — abril 2026)*
Dashboard interativo em HTML puro para acompanhamento de resultados dos clientes.

**KPIs monitorados:**
- Leads gerados
- Taxa de conversão (lead → cliente)
- Custo por lead (Meta Ads)
- Faturamento do cliente
- Agendamentos realizados

**Funcionalidades:**
- Seletor de cliente (suporte a múltiplos clientes)
- Filtro de período: 7, 30 e 90 dias
- Gráfico de evolução de leads
- Funil de conversão visual (Visitante → Lead → Contato → Cliente)
- Lista de agendamentos recentes com status
- Distribuição de faturamento por serviço
- Painel de atualização de dados em tempo real

### 11. WhatsApp Business *(novo — abril 2026)*
- Número dedicado: (11) 95292-8873
- WhatsApp Business configurado com perfil da Fluxia
- Mensagem de boas-vindas e ausência configuradas
- Status: *"Growth Hacking para salões e clínicas 🚀"*
- Integração pendente com automação Make.com

### 12. Lista de Prospecção *(novo — abril 2026)*
- 118 contatos extraídos via Instant Data Scraper do Google Maps
- Segmento: salões de beleza, barbearias e clínicas de estética em São Paulo
- Planilha organizada com nome, avaliação, categoria, endereço, observação e modelo de abordagem
- Classificação em Modelo A (presença digital) e Modelo B (sem presença digital)
- Processo de abordagem ativo via Instagram e WhatsApp

### 13. Materiais de Vendas *(novo — abril 2026)*
- **Guia de Objeções** — 5 objeções mais comuns com respostas prontas e dicas de condução
- **Script de Abordagem Instagram** — fluxo em 5 etapas com 3 modelos de mensagem personalizados por situação
- Regras de ouro de vendas documentadas

---

## 🛠️ Stack Tecnológica

| Categoria | Ferramenta | Função |
|-----------|------------|--------|
| Frontend | HTML/CSS puro | Landing page e dashboard |
| Hospedagem | Netlify | Deploy gratuito |
| Formulário leads | Tally.so | Captação de leads |
| Formulário briefing | Tally.so | Onboarding de clientes |
| Automação | Make.com | Integração entre ferramentas |
| Email | Brevo | Sequência automática + onboarding |
| Chatbot | Typebot | Fluxo conversacional Instagram Direct |
| IA | OpenAI GPT-4o mini | Respostas inteligentes no chatbot |
| Pagamento | Kiwify | Checkout e gestão de produtos |
| Social | Meta Business Suite | Automação de respostas e agendamento |
| Tráfego pago | Meta Ads | Campanha ativa R$15/dia |
| Tráfego pago | Google Ads | Campanha configurada — aguardando ativação |
| Presença local | Google Business | Perfil da empresa |
| Freelancer | Workana + 99Freelas | Prospecção de clientes |
| WhatsApp | WhatsApp Business | Atendimento e prospecção |
| Prospecção | Instant Data Scraper | Extração de leads do Google Maps |
| Versionamento | GitHub | Documentação e portfólio |

---

## 🔄 Arquitetura Completa do Sistema

```
CAPTAÇÃO
Visitante → Landing Page (Netlify)
         → Botão WhatsApp flutuante → Conversa direta
         → Formulário (Tally.so)
         → Make.com [webhook]
         → Lista de contatos (Brevo) — "Leads Agência FLUXIA"
         → Workflow automático → 5 emails em 7 dias
         → Email 5: Proposta + Link de pagamento (Kiwify)

PROSPECÇÃO ATIVA
Lista 118 contatos (Google Maps)
         → Abordagem Instagram (13/dia) — Modelo A e B
         → Abordagem WhatsApp Business
         → Propostas Workana (3/dia)
         → Propostas 99Freelas (3/dia)
         → Meta Ads R$15/dia (paralelo)
         → Google Ads R$20/dia (quando ativar)

VENDA & ONBOARDING
Cliente paga (Kiwify)
         → Webhook → Make.com [imediato]
         → Adiciona contato no Brevo — "Clientes Fluxia Business"
         → Automação Brevo dispara email de boas-vindas
         → Email com CTA → Formulário de briefing (Tally.so)
         → Cliente preenche briefing
         → Produção e entrega em até 7 dias

ATENDIMENTO
Mensagem no Instagram Direct
         → Auto reply (Meta Business Suite)
         → Link do Typebot
         → Chatbot com IA (Typebot + GPT-4o mini)
         → Qualificação → Redirecionamento para landing page

ACOMPANHAMENTO
Dashboard de métricas (HTML interativo)
         → KPIs em tempo real por cliente
         → Funil de conversão visual
         → Relatório de agendamentos e faturamento
```

---

## 📊 Projeção de Resultados

### Projeção mês 1 — 30 dias de execução consistente

| Canal | Contatos/dia | Total mês | Conversas reais | Clientes (15%) |
|-------|-------------|-----------|-----------------|----------------|
| Instagram | 13 | 390 | ~39 | ~6 |
| Workana | 3 | 90 | ~6 | ~1 |
| 99Freelas | 3 | 90 | ~6 | ~1 |
| Meta Ads | — | ~12 leads | ~12 | ~2 |
| **Total** | **19** | **~580** | **~63** | **~10** |

**Faturamento estimado mês 1:**
- Conservador (10%): R$6.000 — R$8.000
- Realista (15%): R$10.000 — R$12.000
- Otimista (20%): R$14.000 — R$16.000

### Projeção mês 2 — com cases e depoimentos

| Cenário | Clientes | Faturamento |
|---------|----------|-------------|
| Conservador | 14 | R$14.000 |
| Realista | 18 | R$18.000 |
| Otimista | 21 | R$21.000 |

---

## 💡 Decisões Técnicas

**Por que HTML puro em vez de React ou Next.js?**
Performance é crítica para páginas de conversão. HTML/CSS puro carrega mais rápido, sem dependências, e é trivial de hospedar gratuitamente.

**Por que Make.com em vez de Zapier?**
1.000 operações gratuitas por mês vs 100 do Zapier. Para o volume inicial, Make é suficiente e gratuito.

**Por que Brevo em vez de Mailchimp?**
Automações completas no plano gratuito. Mailchimp restringe automações para planos pagos.

**Por que Kiwify em vez de Hotmart?**
Interface mais simples, checkout mais limpo e taxa similar (~9,99% por venda).

**Por que GPT-4o mini em vez de GPT-4o?**
Custo ~10x menor com qualidade suficiente para atendimento conversacional.

**Por que Typebot em vez de ManyChat?**
Typebot é gratuito, open source e integra nativamente com OpenAI.

**Por que Growth Hacking e não social media tradicional?**
Growth Hacking entrega sistema que cresce sozinho — funil automatizado, dados, otimização contínua. Social media tradicional entrega presença. O cliente precisa de resultado.

---

## ✅ Status do Projeto

### Fase 1 — Estrutura (concluída)
- [x] Landing page publicada no Netlify com botão WhatsApp
- [x] Formulário de captação de leads (Tally → Brevo)
- [x] Sequência de 5 emails automáticos (Brevo)
- [x] 3 produtos configurados na Kiwify
- [x] Chatbot com IA no Instagram Direct (Typebot + GPT-4o mini)
- [x] Webhook Kiwify → Make.com configurado
- [x] Integração Make.com → Brevo funcionando
- [x] Automação de onboarding pós-venda ativada
- [x] Campanha Meta Ads ativa (R$15/dia)
- [x] Campanha Google Ads configurada (aguardando ativação)
- [x] Perfil Google Business criado
- [x] Perfis Workana e 99Freelas completos
- [x] WhatsApp Business configurado
- [x] Dashboard de métricas interativo
- [x] Guia de objeções (5 objeções com respostas)
- [x] Script de abordagem Instagram (5 etapas + 3 modelos)
- [x] Lista de 118 leads extraída e classificada
- [x] Abordagem ativa iniciada

### Em andamento
- [ ] Abordagem diária — 13 Instagram + 6 Workana/99Freelas
- [ ] Primeiro cliente piloto com depoimento em vídeo
- [ ] Teste completo do fluxo de compra (Kiwify → Make → Brevo → Tally)
- [ ] Automação WhatsApp via Make.com

### Fase 2 — Escala (planejada)
- [ ] ERP conectado ao funil completo
- [ ] Relatório automatizado para clientes
- [ ] Expansão para outros nichos (odontologia, imobiliário)
- [ ] Contratação de assistente operacional
- [ ] Dashboard com Google Analytics integrado

---

## 📁 Estrutura do Repositório

```
fluxia-business/
│
├── landing-page/
│   └── index.html                          # Landing page com botão WhatsApp
│
├── emails/
│   └── emails-brevo-fluxia.html            # 5 emails da sequência automática
│
├── automacoes/
│   └── FLUXIA_BUSINESS_AUTOMACAO.md        # Documentação técnica do onboarding
│
├── dashboard/
│   └── fluxia-dashboard.html               # Dashboard de métricas interativo
│
├── materiais-vendas/
│   ├── guia-objecoes-fluxia.docx           # 5 objeções com respostas prontas
│   └── script-instagram-fluxia.docx        # Script de abordagem em 5 etapas
│
├── prospecção/
│   └── lista_leads_fluxia.xlsx             # 118 leads classificados SP
│
├── posts/
│   ├── post2-case-clinica.html
│   ├── post3-dica-valor.html
│   ├── post4-prova-social.html
│   ├── post5-como-funciona.html
│   ├── post6-oferta-lancamento.html
│   ├── reels-post2-frames.html
│   └── thumbnail-antes-depois.html
│
├── identidade-visual/
│   ├── perfil-instagram-fluxia.svg
│   ├── banner-linkedin-v2.html
│   └── imagem-produto-fluxia-business.svg
│
├── planejamento/
│   └── calendario-maio-2026.md             # 19 posts planejados
│
└── README.md
```

---

## 👩‍💻 Sobre a Autora

Desenvolvido por **Tacianne Braz** como projeto prático aplicado durante estudos em Data Science, Analytics e Inteligência Artificial.

Este projeto demonstra na prática:
- Growth Hacking aplicado a negócios locais
- Integração de múltiplas APIs e plataformas no-code/low-code
- Automação de funil de vendas completo
- Aplicação de LLMs em produto real
- Construção e execução de estratégia de prospecção ativa
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

*Última atualização: abril 2026*
