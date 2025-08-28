# 📧 Bots de Email – Automação de Relatórios de Vendas

Projeto em **Python** para automatizar o envio de emails personalizados para vendedores, com base em suas vendas e metas. Utiliza **pandas** para manipulação de dados e **smtplib** para envio de emails.

---

## 🗂 Estrutura do Projeto

O projeto contém os seguintes arquivos:

- `.gitignore` – arquivos e pastas ignorados pelo Git  
- `app.py` – script principal que processa dados e envia emails  
- `vendas.xlsx` – planilha com dados de vendas  
- `LICENSE` – licença do projeto  
- `README.md` – este arquivo  
- `requirements.txt` – dependências do projeto  

---

## 🛠 Tecnologias Utilizadas

- Python – Linguagem principal do projeto  
- pandas – Para leitura e manipulação de arquivos Excel  
- smtplib – Envio de emails via SMTP  
- email.mime – Formatação de emails HTML  
- dotenv – Gerenciamento de variáveis de ambiente  

---

## ⚡ Funcionalidades

- Ler dados de vendas a partir de uma planilha Excel  
- Calcular se cada vendedor atingiu ou não a meta  
- Gerar emails HTML personalizados para cada situação:  
  - Parabéns por atingir a meta  
  - Incentivo para melhorar resultados  
- Enviar emails automaticamente via Gmail ou outro servidor SMTP  

---

## Como Instalar

1. Clone o repositório:  

```
git clone <URL_DO_REPOSITORIO>
cd bots_email

```

2. Crie um ambiente virtual (opcional, mas recomendado):  

```
python -m venv venv
venv\Scripts\activate # Windows
source venv/bin/activate # Linux / Mac
```

3. Instale as dependências:  

```
pip install -r requirements.txt
```

4. Configure suas variáveis de ambiente no arquivo `.env`:  

```
EMAIL_USER=seu_email@gmail.com
EMAIL_PASSWORD=sua_senha_de_app
```

> ⚠️ Recomenda-se usar **senha de app** para contas Gmail.

5. Execute o bot:  

```
python app.py

```

---

## 📝 Observações

- Certifique-se de que a planilha `vendas.xlsx` contém as colunas: `Vendedor`, `Email`, `Periodo`, `Meta`, `Venda`  
- O script envia emails para todos os registros na planilha, gerando mensagens personalizadas  

---

## Licença

Este projeto está sob a **MIT License** – veja `LICENSE` para detalhes.
