# Fluxia Business — Agência de Automação com IA

> Projeto real de automação de processos para pequenos negócios usando Inteligência Artificial, desenvolvido do zero em menos de 30 dias.

---

## 📌 Sobre o Projeto

A **Fluxia Business** é uma agência de automação com IA criada para resolver um problema real: pequenos negócios perdem em média **48 horas por mês** em tarefas repetitivas que podem ser automatizadas.

Este repositório documenta toda a arquitetura técnica e as decisões de projeto tomadas para construir um **funil de vendas 100% automatizado**, desde a captação do lead até o pagamento e entrega — sem intervenção humana.

**Site ao vivo:** [fluxiabusiness.netlify.app](https://fluxiabusiness.netlify.app)
**Instagram:** [@fluxia_business](https://instagram.com/fluxia_business)
**LinkedIn:** [Fluxia Business](https://linkedin.com/company/fluxia-business)

---

## 🚀 O que foi construído

### 1. Landing Page
- HTML/CSS puro, responsivo, sem frameworks
- Design editorial com identidade visual consistente
- 3 pacotes de preço — Starter R$997, Pro R$2.500, Full R$4.500
- Formulário de captação integrado via Tally.so
- Hospedagem gratuita via **Netlify**

### 2. Funil de Captação Automático
- Formulário de leads via **Tally.so**
- Integração Tally → Brevo via **Make.com** (webhook)
- Sequência de 5 emails automáticos em 7 dias
- Gatilho: lead entra na lista → emails disparam sozinhos

### 3. Sequência de Email Marketing
- 5 emails configurados no **Brevo**
- Personalização com variáveis dinâmicas (`{{ contact.FIRSTNAME }}`, `{{ contact.SEGMENTO }}`, `{{ contact.DOR }}`)
- Delays configurados: 0, 1, 3, 5 e 7 dias
- Email 5 com link direto para pagamento via Kiwify

### 4. Produto e Pagamento
- 3 produtos configurados na **Kiwify**
  - Starter: R$ 997 (1 automação)
  - Pro: R$ 2.500 (3 automações)
  - Full: R$ 4.500 (5 automações + suporte estendido)
- Checkout com cartão, boleto e Pix
- Recorrência mensal: R$ 500–800/mês

### 5. Chatbot com IA — Instagram Direct
- Fluxo conversacional construído no **Typebot**
- Integração com **OpenAI GPT-4o mini** via API
- 4 fluxos principais:
  - Serviços — apresentação completa
  - Preços — 3 pacotes com valores
  - Falar com a equipe — redirecionamento para landing page
  - Outros assuntos — resposta livre com IA
- Resposta automática configurada no **Meta Business Suite**
- Link do Typebot enviado automaticamente no primeiro contato

### 6. Onboarding Automático Pós-Venda
- Webhook da Kiwify → Make.com
- Email automático com link do formulário de briefing
- Formulário de briefing personalizado no **Tally.so**:
  - Nome e segmento do negócio
  - 5 serviços principais
  - Diferencial competitivo
  - Cliente ideal
  - Tom de comunicação
  - Materiais visuais

### 7. Presença Digital
- Instagram: [@fluxia_business](https://instagram.com/fluxia_business)
- LinkedIn: [Fluxia Business](https://linkedin.com/company/fluxia-business)
- Calendário de conteúdo — 19 posts planejados para abril/maio 2026
- Posts criados em HTML com design consistente e identidade visual
- Reels com roteiros prontos para CapCut

---

## 🛠️ Stack Tecnológica

| Categoria | Ferramenta | Função |
|---|---|---|
| Frontend | HTML/CSS puro | Landing page |
| Hospedagem | Netlify | Deploy gratuito |
| Formulário leads | Tally.so | Captação de leads |
| Formulário briefing | Tally.so | Onboarding de clientes |
| Automação | Make.com | Integração entre ferramentas |
| Email | Brevo | Sequência automática de emails |
| Chatbot | Typebot | Fluxo conversacional Instagram Direct |
| IA | OpenAI GPT-4o mini | Respostas inteligentes no chatbot |
| Pagamento | Kiwify | Checkout e gestão de produtos |
| Social | Meta Business Suite | Automação de respostas e agendamento |
| Versionamento | GitHub | Documentação e portfólio |

---

## 🔄 Arquitetura Completa do Sistema

```
CAPTAÇÃO
Visitante → Landing Page (Netlify)
         → Formulário (Tally.so)
         → Make.com [webhook]
         → Lista de contatos (Brevo)
         → Workflow automático → 5 emails em 7 dias
         → Email 5: Proposta + Link de pagamento (Kiwify)

VENDA
Cliente paga (Kiwify)
         → Webhook → Make.com
         → Email automático com link do briefing
         → Cliente preenche briefing (Tally.so)
         → Produção e entrega em 7 dias

ATENDIMENTO
Mensagem no Instagram Direct
         → Auto reply (Meta Business Suite)
         → Link do Typebot
         → Chatbot com IA (Typebot + GPT-4o mini)
         → Qualificação → Redirecionamento para landing page
```

---

## 📊 Projeção de Resultados

| Período | Visitantes/mês | Leads | Clientes | Receita estimada |
|---|---|---|---|---|
| Mês 1 | ~400 | ~40 | 0–1 | R$ 0–997 |
| Mês 3 | ~800 | ~160 | 2–3 | R$ 2k–3k |
| Mês 6 | ~1.200 | ~240 | 4–6 | R$ 4k–6k |
| Mês 12 | ~2.000+ | ~400+ | 8–12 | R$ 8k–15k |

---

## 💡 Decisões Técnicas

### Por que HTML puro em vez de React ou Next.js?
Performance é crítica para páginas de conversão. HTML/CSS puro carrega mais rápido, sem dependências, e é trivial de hospedar gratuitamente.

### Por que Make.com em vez de Zapier?
1.000 operações gratuitas por mês vs 100 do Zapier. Para o volume inicial, Make é suficiente e gratuito.

### Por que Brevo em vez de Mailchimp?
Automações completas no plano gratuito. Mailchimp restringe automações para planos pagos.

### Por que Kiwify em vez de Hotmart?
Interface mais simples, checkout mais limpo e taxa similar (~9,99% por venda).

### Por que GPT-4o mini em vez de GPT-4o?
Custo ~10x menor com qualidade suficiente para atendimento conversacional. Para o volume inicial, a economia é significativa.

### Por que Typebot em vez de ManyChat?
Typebot é gratuito, open source e integra nativamente com OpenAI. ManyChat cobra por contatos.

---

## 📁 Estrutura do Repositório

```
fluxia-business/
│
├── landing-page/
│   └── landing-fluxia-v3.html     # Landing page completa com 3 pacotes
│
├── emails/
│   └── emails-brevo-fluxia.html   # 5 emails da sequência automática
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
│   └── calendario-maio-2026.md    # 19 posts planejados
│
└── README.md
```

---

## 👩‍💻 Sobre a Autora

Desenvolvido por **Tacianne Braz** como projeto prático aplicado durante estudos em **Data Science, Analytics e Inteligência Artificial**.

Este projeto demonstra na prática:
- Integração de múltiplas APIs e plataformas
- Automação de processos com ferramentas no-code/low-code
- Aplicação de LLMs (Large Language Models) em produto real
- Construção de funil de vendas orientado a dados
- Design e desenvolvimento frontend
- Arquitetura de sistemas de atendimento automatizado
- Estratégia de conteúdo e marketing digital

---

## 📬 Contato

- **Site:** [fluxiabusiness.netlify.app](https://fluxiabusiness.netlify.app)
- **Instagram:** [@fluxia_business](https://instagram.com/fluxia_business)
- **LinkedIn:** [Fluxia Business](https://linkedin.com/company/fluxia-business)
