# Fluxia Business — Agência de Automação com IA

> Projeto real de automação de processos para pequenos negócios usando Inteligência Artificial, desenvolvido do zero em menos de 30 dias.

---

## 📌 Sobre o Projeto

A **Fluxia Business** é uma agência de automação com IA criada para resolver um problema real: pequenos negócios perdem em média **48 horas por mês** em tarefas repetitivas que podem ser automatizadas.

Este repositório documenta toda a arquitetura técnica e as decisões de projeto tomadas para construir um **funil de vendas 100% automatizado**, desde a captação do lead até o pagamento — sem intervenção humana.

**Site ao vivo:** [fluxiabusiness.netlify.app](https://fluxiabusiness.netlify.app)

---

## 🚀 O que foi construído

### 1. Landing Page
- HTML/CSS puro, responsivo, sem frameworks
- Design editorial com identidade visual consistente
- Seção de preços com 3 pacotes (Starter, Pro, Full)
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

### 5. Chatbot com IA (Instagram Direct)
- Fluxo conversacional construído no **Typebot**
- Integração com **OpenAI GPT-4o mini** via API
- 4 fluxos: Serviços, Preços, Falar com equipe, Outros assuntos
- Resposta automática configurada no Meta Business Suite

### 6. Presença Digital
- Instagram: [@fluxia_business](https://instagram.com/fluxia_business)
- LinkedIn: [Fluxia Business](https://linkedin.com/company/fluxia-business)
- Calendário de 6 posts criados e programados

---

## 🛠️ Stack Tecnológica

| Categoria | Ferramenta | Função |
|---|---|---|
| Frontend | HTML/CSS puro | Landing page |
| Hospedagem | Netlify | Deploy gratuito |
| Formulário | Tally.so | Captação de leads |
| Automação | Make.com | Integração entre ferramentas |
| Email | Brevo | Sequência automática de emails |
| Chatbot | Typebot | Fluxo conversacional |
| IA | OpenAI GPT-4o mini | Respostas inteligentes |
| Pagamento | Kiwify | Checkout e gestão de produtos |
| Social | Meta Business Suite | Automação de respostas |

---

## 🔄 Arquitetura do Funil

```
Visitante
    ↓
Landing Page (Netlify)
    ↓
Formulário (Tally.so)
    ↓
Make.com [webhook]
    ↓
Lista de contatos (Brevo)
    ↓
Workflow automático → 5 emails em 7 dias
    ↓
Email 5: Proposta + Link de pagamento (Kiwify)
    ↓
Cliente paga → Entrega do serviço
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

## 💡 Aprendizados e Decisões Técnicas

### Por que HTML puro em vez de React ou Next.js?
A landing page foi construída em HTML/CSS puro para maximizar a velocidade de carregamento e simplicidade de deploy. Para uma página de conversão, performance é crítica — cada segundo a mais reduz a taxa de conversão em ~7%.

### Por que Make.com em vez de Zapier?
O Make.com oferece 1.000 operações gratuitas por mês contra 100 do Zapier. Para o volume inicial, Make é suficiente e gratuito.

### Por que Brevo em vez de Mailchimp?
O Brevo permite automações completas no plano gratuito. O Mailchimp restringe automações para planos pagos.

### Por que Kiwify em vez de Hotmart?
Interface mais simples, checkout mais limpo e taxa similar (~9,99% por venda).

### Por que GPT-4o mini em vez de GPT-4o?
Custo ~10x menor com qualidade suficiente para atendimento conversacional básico. Para o volume inicial, a economia é significativa.

---

## 📁 Estrutura do Repositório

```
fluxia-business/
│
├── landing-page/
│   └── index.html          # Landing page completa
│
├── emails/
│   └── sequencia-brevo.html # 5 emails da sequência
│
├── posts/
│   ├── post1-apresentacao.html
│   ├── post2-case-clinica.html
│   ├── post3-dica-valor.html
│   ├── post4-prova-social.html
│   ├── post5-como-funciona.html
│   └── post6-oferta-lancamento.html
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

---

## 📬 Contato

- **Site:** [fluxiabusiness.netlify.app](https://fluxiabusiness.netlify.app)
- **Instagram:** [@fluxia_business](https://instagram.com/fluxia_business)
- **LinkedIn:** [Fluxia Business](https://linkedin.com/company/fluxia-business)
