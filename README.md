# 🧪 clinical-report-engine  
**Automated TLFs (Tables, Listings, Figures) for Phase I–III Clinical Trials**

> Solução em R para automação de relatórios regulatórios — ideal para CROs, bioestatísticos e profissionais de desenvolvimento clínico.

![R](https://img.shields.io/badge/R-4.4+-276DC3?logo=r)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 💡 O que é?

Motor de relatórios clínicos em **R + RMarkdown** que gera automaticamente:

- ✅ **Tabelas** de demografia e distribuição (com `gt`)
- ✅ **Listagens** dos dados brutos
- ✅ **Figuras** de eventos adversos (`ggplot2`)
- ✅ **Análise estatística** (Teste Exato de Fisher)
- ✅ **Validação de dados** antes da geração

Totalmente **reprodutível, auditável e alinhado às boas práticas regulatórias** (ICH E3, CDISC).

---

## 📦 Tecnologias

- **R** (`tidyverse`, `gt`, `rmarkdown`)
- Saída em **Word, HTML ou PDF**
- Dados de exemplo em formato **CSV (compatível com separador `;`)**

---

## ▶️ Como Executar

```r
# 1. Clone o repositório
# 2. Instale dependências
install.packages(c("tidyverse", "gt", "rmarkdown"))

# 3. Gere o relatório
rmarkdown::render("analysis.Rmd", output_format = "word_document")
