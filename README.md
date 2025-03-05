
# 📊 Dashboard RFV - Segmentação de Clientes

Este projeto é uma aplicação desenvolvida em **Streamlit** para análise e segmentação de clientes utilizando a metodologia **RFV** (Recência, Frequência e Valor). O objetivo é classificar os clientes com base em seu comportamento de compras e sugerir ações estratégicas para retenção, fidelização e recuperação de clientes.

## 🌐 Acesse a aplicação online

🔗 [Clique aqui para acessar o Dashboard RFV](https://apprfv.streamlit.app/)

## 🛠️ Tecnologias Utilizadas

- Python 3.11+
- Streamlit
- Pandas
- Numpy
- XlsxWriter

## 📥 Como Funciona

### 📊 O que é RFV?
O conceito de **RFV** é uma técnica de segmentação de clientes baseada em 3 pilares:

| Componente | Descrição |
|---|---|
| Recência (R) | Quantos dias se passaram desde a última compra do cliente |
| Frequência (F) | Quantidade total de compras realizadas pelo cliente no período analisado |
| Valor (V) | Total de dinheiro gasto pelo cliente no período analisado |

## 🚀 Como rodar o projeto localmente

1. Clone o repositório:
    ```bash
    git clone https://github.com/seu-usuario/nome-do-repositorio.git
    ```
2. Crie um ambiente virtual:
    ```bash
    python -m venv venv
    ```
3. Ative o ambiente virtual:
    - Windows:
        ```bash
        venv\Scripts\activate
        ```
    - Mac/Linux:
        ```bash
        source venv/bin/activate
        ```
4. Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```
5. Execute a aplicação:
    ```bash
    streamlit run app_RFV.py
    ```

## 📂 Estrutura do Projeto

```
.
├── app_RFV.py                # Código principal da aplicação Streamlit
├── requirements.txt          # Lista de bibliotecas necessárias
├── README.md                  # Esse arquivo com informações do projeto
├── input/                     # Pasta para armazenar o arquivo de dados (ex: dados.csv)
├── auxiliar/                  # Pasta para armazenar arquivos auxiliares (ex: output RFV)
```

## 📋 Como Usar a Aplicação

### Passo 1: Upload do Arquivo
Na barra lateral da aplicação, selecione seu arquivo de transações no formato CSV ou Excel. O arquivo deve conter pelo menos as seguintes colunas:

| Coluna | Descrição |
|---|---|
| ID_cliente | Identificador único do cliente |
| DiaCompra | Data da compra |
| CodigoCompra | Código da transação |
| ValorTotal | Valor da compra |

### Passo 2: Análise RFV
Após subir o arquivo, o app automaticamente calcula:

- Recência (R)
- Frequência (F)
- Valor (V)

E gera uma tabela RFV completa.

### Passo 3: Segmentação e Ações
Com base nos quartis de cada métrica, os clientes são classificados em grupos de desempenho (A, B, C, D). Esses grupos são então usados para sugerir ações específicas de marketing/CRM.

| RFV Score | Ação Recomendada |
|---|---|
| AAA | Enviar cupons e pedidos de indicação |
| DDD | Cliente perdido (churn) - Sem ação |
| CAA ou DAA | Clientes valiosos em risco - Enviar ofertas especiais |

### Passo 4: Download da Tabela RFV
Você pode baixar a tabela RFV segmentada em Excel diretamente da aplicação.

## 📡 Deploy

### Opções Sugeridas:
- [Streamlit Community Cloud](https://streamlit.io/cloud)
- Heroku
- AWS EC2
- Azure App Service

## 📑 Requisitos

### `requirements.txt` (exemplo)
```
streamlit
pandas
numpy
xlsxwriter
```

## 💡 Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests no repositório.

## 📜 Licença

Esse projeto é livre para uso acadêmico e educacional.

## 🔗 Contato

Caso queira entrar em contato ou tirar dúvidas:

- 📧 Email: seu-email@exemplo.com
- 🔗 LinkedIn: [Seu LinkedIn](https://linkedin.com/in/seu-perfil)

