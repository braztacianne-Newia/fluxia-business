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
- 145 visualizações de página a R$0,29 por visita
- Público dominante: mulheres 18-34 anos (70%)
- Melhor plataforma: Instagram (resultados superiores ao Facebook)

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
- Rodapé com contato da Fluxia
- Link personalizado por cliente

### 11. Google Sheets — Banco de Dados *(novo — maio 2026)*
- Planilha pública conectada aos dashboards
- Colunas: Cliente | Leads | Conversão | CPL | Faturamento | Agendamentos
- 4 clientes piloto configurados
- Integração Make.com ativa

### 12. Automação de Prospecção com IA *(novo — maio 2026)*
Pipeline completo e automatizado de prospecção de clientes no Instagram.

```
Apify extrai perfis do Instagram por nicho e região
        ↓
Make.com recebe os dados via API
        ↓
Iterator processa cada perfil individualmente
        ↓
Google Sheets Search verifica duplicados automaticamente
        ↓
OpenAI GPT-4o mini gera mensagem personalizada por perfil
        ↓
Google Sheets recebe: @, nome, seguidores, bio, mensagem pronta, status
        ↓
Operador revisa em segundos e envia
```

**Campos automatizados por perfil:**
- Username
- Nome completo
- Seguidores
- Biografia
- Categoria do negócio
- Link de contato
- URL do perfil
- Mensagem personalizada gerada por IA
- Status (Pendente/Enviado/Respondeu/Interessada)
- Data de envio
- Resposta
- Próxima ação

**Tecnologias:** Apify Instagram Scraper + Make.com + OpenAI GPT-4o mini + Google Sheets

### 13. Presença Digital e Perfis Freelancer
- Instagram: @fluxia_business
- LinkedIn: Fluxia Business
- Google Business criado e otimizado ✅
- Perfil Workana: 100% completo e ativo
- **99Freelas Pro:** assinatura ativa — múltiplas propostas enviadas ✅
- WhatsApp Business: (11) 95292-8873 ✅

### 14. Lista de Prospecção *(atualizada — maio 2026)*
- 118 contatos extraídos via Instant Data Scraper do Google Maps
- Novos lotes extraídos via Apify Instagram Scraper
- Segmento: salões de beleza, barbearias e clínicas de estética em São Paulo
- Classificação em Modelo A (presença digital) e Modelo B (sem presença)
- Abordagens ativas via Instagram com mensagens geradas por IA
- Controle em Google Sheets com status, resposta e próxima ação
- Meta: 15 contatos por dia no Instagram + propostas diárias nas plataformas freelancer

### 15. Materiais de Vendas
- **Guia de Objeções** — 5 objeções com respostas e dicas
- **Script de Abordagem Instagram** — 5 etapas + 3 modelos personalizados
- **Texto padrão de abordagem** — adaptável por perfil, gerado por IA, sem soar genérico

### 16. Propostas Freelancer Enviadas *(atualizado — maio 2026)*
- **Automação atendimento comercial CHATCENTER** — Make + Sheets — R$1.900
- **Agente IA via respond.io** — loja de automóveis Portugal — R$750
- **Agente IA atendimento ao cliente** — Typebot + GPT — R$1.200
- **Landing page Google Maps** — HTML responsivo — R$320
- **Automação Hotmart** — Make + Drive + Sheets — R$1.600

---

## 🛠️ Stack Tecnológica

| Categoria | Ferramenta | Função |
|-----------|------------|--------|
| Frontend | HTML/CSS puro | Landing page e dashboards |
| Hospedagem | Netlify | Deploy gratuito |
| Formulário leads | Tally.so | Captação de leads |
| Automação | Make.com | Integração entre ferramentas |
| Email | Brevo | Sequência automática + onboarding |
| Chatbot | Typebot | Fluxo conversacional |
| IA | OpenAI GPT-4o mini | Respostas e geração de mensagens |
| Pagamento | Kiwify | Checkout e gestão de produtos |
| Social | Meta Business Suite | Automação e agendamento |
| Tráfego pago | Meta Ads | Campanha ativa R$15/dia |
| Tráfego pago | Google Ads | Configurado — aguardando ativação |
| Presença local | Google Business | Perfil da empresa |
| Banco de dados | Google Sheets | KPIs e prospecção |
| Prospecção IA | Apify | Extração de perfis Instagram |
| Geração texto | OpenAI API | Mensagens personalizadas por perfil |
| Freelancer | Workana Pro | Prospecção de clientes |
| Freelancer | 99Freelas Pro | Prospecção + propostas |
| WhatsApp | WhatsApp Business | Atendimento e prospecção |
| Prospecção Maps | Instant Data Scraper | Extração de leads Google Maps |
| Versionamento | GitHub | Documentação e portfólio |

---

## 🔄 Arquitetura Completa do Sistema

```
CAPTAÇÃO PASSIVA
Visitante → Landing Page (Netlify)
         → Formulário (Tally.so) → Make.com → Brevo → 5 emails → Kiwify

CAPTAÇÃO ATIVA AUTOMATIZADA (novo)
Apify extrai perfis Instagram por nicho/região
         → Make.com processa cada perfil
         → Verifica duplicados no Sheets
         → GPT-4o mini gera mensagem personalizada
         → Google Sheets recebe tudo organizado
         → Operador revisa e envia em segundos

CAPTAÇÃO ATIVA MANUAL
Lista 118 contatos (Google Maps SP)
         → Instagram 15/dia
         → Propostas Workana e 99Freelas
         → Meta Ads R$15/dia

VENDA & ONBOARDING
Cliente paga (Kiwify) → Webhook → Make.com → Brevo → Email briefing → Entrega 7 dias

ATENDIMENTO
Instagram Direct → Auto reply → Typebot + GPT-4o mini → Qualificação → Landing page

ACOMPANHAMENTO
Dashboard interno → Todos os clientes → KPIs via Google Sheets
Dashboard cliente → Dados específicos → Resumo executivo automático
```

---

## 📊 Resultados Meta Ads *(maio 2026)*

| Métrica | Resultado |
|---------|-----------|
| Visualizações da página | 145 |
| Custo por visualização | R$0,29 |
| Valor gasto | R$42,76 |
| Público dominante | Mulheres 18-34 (70%) |
| Melhor plataforma | Instagram |

---

## ✅ Status do Projeto

### Fase 1 — Estrutura (em execução)
- [x] Landing page com Growth Hacking
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
- [x] **Automação de prospecção Apify → Make → OpenAI → Sheets (novo)**
- [x] **Geração de mensagens personalizadas por IA por perfil (novo)**
- [x] **Verificação automática de duplicados na prospecção (novo)**
- [x] **5 propostas enviadas nas plataformas freelancer (novo)**

### Em andamento
- [ ] Primeiro cliente pagante com depoimento em vídeo
- [ ] Verificação do Instagram para liberar Direct
- [ ] Conteúdo programado 30 dias no Instagram
- [ ] IA de atendimento treinada para salões
- [ ] Novo criativo Meta Ads com maior retenção

### Fase 2 — Escala (planejada)
- [ ] ERP conectado ao funil completo
- [ ] Relatório automatizado via Make.com
- [ ] Expansão para outros nichos
- [ ] Contratação de assistente operacional

---

## 📁 Estrutura do Repositório

```
fluxia-business/
│
├── index.html                          # Landing page
├── dashboard.html                      # Dashboard interno
├── dashboard-cliente.html              # Dashboard do cliente — template
│
├── automacoes/
│   ├── FLUXIA_BUSINESS_AUTOMACAO.md    # Documentação onboarding
│   └── prospeccao-instagram-make.md    # Documentação automação prospecção (novo)
│
├── prospeccao/
│   ├── lista_leads_fluxia.xlsx         # 118 leads Google Maps
│   └── prospeccao_instagram_fluxia.xlsx # Leads Instagram com mensagens IA (novo)
│
├── materiais-vendas/
│   ├── guia-objecoes-fluxia.docx
│   └── script-instagram-fluxia.docx
│
├── emails/
│   └── emails-brevo-fluxia.html
│
├── posts/
│   └── [posts e reels]
│
├── identidade-visual/
│   └── [logos e banners]
│
└── README.md
```

---

## 💡 Decisões Técnicas

**Por que Apify para extração de perfis?**
Permite buscar perfis Instagram por nicho e localização sem violar os termos de uso. Plano gratuito com $5 de crédito é suficiente para centenas de perfis por mês.

**Por que GPT-4o mini para geração de mensagens?**
Custo mínimo por mensagem (~$0,001), qualidade suficiente para personalização, integra nativamente com Make.com via API.

**Por que verificar duplicados antes de adicionar?**
Evita abordar o mesmo perfil duas vezes e mantém a planilha limpa para controle de status.

**Por que HTML puro em vez de React ou Next.js?**
Performance crítica para páginas de conversão. Carrega mais rápido, sem dependências, hospedagem gratuita.

**Por que Make.com em vez de Zapier?**
1.000 operações gratuitas por mês vs 100 do Zapier.

**Por que Brevo em vez de Mailchimp?**
Automações completas no plano gratuito.

**Por que Kiwify em vez de Hotmart?**
Interface mais simples e checkout mais limpo.

---

## 👩‍💻 Sobre a Autora

Desenvolvido por **Tacianne Braz** como projeto prático aplicado durante estudos em Data Science, Analytics e Inteligência Artificial.

Este projeto demonstra na prática:
- Growth Hacking aplicado a negócios locais
- Pipeline de prospecção automatizado com IA
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
