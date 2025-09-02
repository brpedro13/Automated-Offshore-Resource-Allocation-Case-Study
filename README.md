# Case Study: Automação de Alocação de Recursos Offshore com Python

> Este repositório descreve uma ferramenta de automação que desenvolvi na MODEC para otimizar a alocação de colaboradores em plataformas offshore, prevenindo proativamente o risco de downtime operacional.

---

### 🏆 **Resultados-Chave em Destaque**

| Métrica | Impacto Gerado |
| :--- | :--- |
| ⚙️ **Prevenção de Risco** | Sistema de alerta proativo para **evitar downtime** resultante da falta de pessoal |
| 📧 **Comunicação Automatizada** | **100%** de automação no envio de relatórios de lacunas para fornecedores |
| 🕒 **Redução de Erro Humano** | Eliminação de erros manuais na coleta e análise de dados de demanda |

---

## Problema de Negócio

O processo de garantir que todas as vagas de trabalho nas plataformas offshore estivessem preenchidas era crítico e complexo. A verificação da demanda de colaboradores era feita manualmente em um portal online, um processo lento e suscetível a erros humanos. A comunicação com os fornecedores para preencher as lacunas era reativa, o que criava um risco constante de equipes embarcarem com pessoal faltando, resultando em potencial **downtime operacional** e atrasos em projetos.

## 💡 Minha Solução

Desenvolvi uma **ferramenta de automação ponta-a-ponta em Python** que criou um pipeline de dados autônomo. O script foi projetado para:

1.  **Extrair os Dados:** Realizar web scraping diário no portal interno para coletar as necessidades de pessoal.
2.  **Analisar e Identificar Lacunas:** Processar e estruturar os dados coletados, comparando a demanda com a alocação existente para identificar com precisão onde e quais profissionais estavam faltando.
3.  **Gerar e Enviar Alertas:** Criar automaticamente relatórios claros em formato `.csv` detalhando as lacunas e enviá-los por e-mail para os fornecedores responsáveis, garantindo que a informação chegasse à pessoa certa no tempo certo.

## 🛠️ Arquitetura e Tecnologias

- **Linguagem:** Python
- **Web Scraping:** `Requests` (para requisições HTTP) e `Selenium` (para automação de navegador e extração de dados de páginas dinâmicas).
- **Processamento de Dados:** `Pandas` (para estruturação, limpeza e análise dos dados).
- **Envio de E-mails:** `SMTPLIB` e `email` (bibliotecas padrão do Python para automação de e-mails).

## ✨ Principais Funcionalidades Implementadas

- **Módulo de Coleta de Dados:** Um scraper robusto, capaz de navegar no portal e extrair as tabelas de demanda de forma consistente.
- **Módulo de Análise de Lacunas:** Lógica de negócio para comparar a demanda vs. a oferta de profissionais por especialidade e plataforma.
- **Módulo de Geração de Relatórios:** Criação dinâmica de arquivos `.csv`, formatados para fácil leitura no Excel, contendo apenas as informações críticas sobre as vagas em aberto.
- **Módulo de Alerta Automatizado:** Um serviço de e-mail que anexa o relatório e envia um alerta padronizado para uma lista de distribuição de fornecedores.

> *Nota: Por se tratar de um projeto interno e proprietário da MODEC, o código-fonte não pode ser compartilhado publicamente. Este repositório serve como uma documentação detalhada da arquitetura do projeto, dos desafios enfrentados e, principalmente, do valor gerado para o negócio.*
