<div align="center">

# 📊 Calculadora de Impostos — CLT vs. PJ

**Simulador Financeiro e Tributário Interativo para Profissionais e Prestadores de Serviços**

[![Vercel Deploy](https://img.shields.io/badge/Vercel-Online-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://calculadora-impostos-3gft.vercel.app/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)

<p align="center">
  <a href="#-sobre-o-projeto">Sobre</a> •
  <a href="#-demonstração-em-produção">Demonstração</a> •
  <a href="#-funcionalidades-e-regras-de-negócio">Regras de Cálculo</a> •
  <a href="#-tecnologias-utilizadas">Tecnologias</a> •
  <a href="#-como-executar-localmente">Execução</a> •
  <a href="#-autor-e-contato">Contato</a>
</p>

</div>

---

## 📌 Sobre o Projeto

A **Calculadora de Impostos CLT vs. PJ** é uma aplicação web interativa projetada para comparar, de forma transparente e imediata, a rentabilidade líquida e a carga tributária entre o regime de contratação **CLT (Consolidação das Leis do Trabalho)** e a prestação de serviços como **Pessoa Jurídica (PJ)**.

O sistema foi concebido para auxiliar desenvolvedores, consultores e demais profissionais do mercado na análise financeira de propostas de trabalho, transições de carreira e planejamento tributário.

---

## 🌐 Demonstração em Produção

A aplicação está publicada e disponível para uso imediato na **Vercel**:

👉 **[Acessar Calculadora ao Vivo (calculadora-impostos-3gft.vercel.app)](https://calculadora-impostos-3gft.vercel.app/)**

---

## ⚙️ Funcionalidades e Regras de Negócio

### 1. Simulação Completa no Regime CLT
A partir do **Salário Bruto Mensal** e do **Número de Dependentes**, o motor de cálculo aplica automaticamente as alíquotas oficiais:

| Encargo / Benefício | Regra Aplicada no Sistema |
| :--- | :--- |
| **FGTS (8%)** | Cálculo informativo do depósito patronal equivalente a `8%` sobre o salário bruto. |
| **INSS Progressivo** | Cálculo por faixas salariais progressivas (`7,5%`, `9%`, `12%` e `14%`), respeitando o teto de contribuição previdenciária (`R$ 7.786,02`). |
| **IRRF Progressivo** | Base de cálculo ajustada (`Salário Bruto - INSS - Dedução de R$ 189,59 por dependente`) com aplicação das faixas de isenção até `27,5%` e parcela a deduzir. |
| **Salário Líquido** | Resultado final apurado (`Salário Bruto - INSS - IRRF`) formatado no padrão monetário brasileiro (`BRL`). |

### 2. Simulação no Regime Pessoa Jurídica (PJ)
Permite alternar entre os dois principais enquadramentos tributários para prestação de serviços:

| Regime Tributário | Metodologia de Cálculo |
| :--- | :--- |
| **Simples Nacional (Anexo III)** | Aplicação da alíquota inicial de `6%` sobre o faturamento bruto mensal, exibindo o total de impostos pagos e o lucro líquido. |
| **Lucro Presumido (Simplificado)** | Apuração consolidada de **PIS** (`0,65%`), **COFINS** (`3%`), **ISS** (`5%`), **IRPJ** (`15%` sobre base presumida de `32%`) e **CSLL** (`9%` sobre base presumida de `32%`). |

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 Semântico:** Estruturação acessível de formulários, seletores e painel dinâmico de relatórios.
- **CSS3 Moderno:** Layout limpo, responsivo e focado em legibilidade financeira, com diferenciação visual entre proventos, descontos e saldo líquido.
- **JavaScript (ES6+ Vanilla):** Arquitetura modular de funções puras para cálculos tributários, manipulação de eventos do DOM e formatação internacionalizada via `Intl` / `toLocaleString('pt-BR')`.

---

## 📂 Estrutura do Projeto

```text
calculadora-impostos/
├── index.html          # Interface principal e formulários de entrada (CLT e PJ)
├── style.css           # Estilização responsiva e componentes visuais do relatório
├── script.js           # Motor de cálculo tributário (INSS, IRRF, FGTS, Simples e Lucro Presumido)
└── README.md           # Documentação técnica do projeto
```

---

## 🚀 Como Executar Localmente

1. **Clone este repositório:**
   ```bash
   git clone https://github.com/italoholanda-dev/calculadora-impostos.git
   ```

2. **Acesse o diretório do projeto:**
   ```bash
   cd calculadora-impostos
   ```

3. **Execute no navegador:**
   Abra o arquivo `index.html` diretamente no navegador de sua preferência ou utilize a extensão **Live Server** no VS Code.

---

## 👨‍💻 Autor e Contato

Desenvolvido por **Italo Holanda Neves** — Graduando em Análise e Desenvolvimento de Sistemas (Faculdade de Tecnologia Senac Amazonas) e Desenvolvedor Web no IDESAM.

- 🌐 **Portfólio Oficial:** [portfolio-italo-murex.vercel.app](https://portfolio-italo-murex.vercel.app/)
- 💼 **LinkedIn:** [linkedin.com/in/italo-holanda](https://www.linkedin.com/in/italo-holanda/)
- 🐙 **GitHub:** [github.com/italoholanda-dev](https://github.com/italoholanda-dev)
- 📧 **E-mail:** [italoholanda90@gmail.com](mailto:italoholanda90@gmail.com)

---

<div align="center">
  <sub>© 2026 Italo Holanda Neves. Todos os direitos reservados.</sub>
</div>
