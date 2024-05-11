**IA Assistente de Compras de Supermercado - Multimodal**

**Descrição**
  Este projeto implementa um Assistente de Compras de Supermercado inteligente utilizando a API do Google Gemini. A ferramenta coleta informações do usuário sobre suas necessidades de compra, incluindo número de pessoas, duração da compra, restrições alimentares, hábitos alimentares e alergias. Com base nesses dados, o sistema gera uma lista de compras personalizada, organizada por categorias e com quantidades especificadas, otimizada para evitar desperdícios.

**Funcionalidades**
  Coleta de dados do usuário através de widgets interativos no Google Colab.
  Geração de listas de compras personalizadas considerando:
  - Número de pessoas na família
  - Duração da compra (mensal, quinzenal, semanal)
  - Restrições alimentares (sem glúten, sem lactose, vegetariano, vegano)
  - Refeições feitas em casa (café da manhã, almoço, jantar)
  - Alergias a alimentos específicos
  - Opção de analisar uma imagem da despensa ou geladeira do usuário para evitar a inclusão de itens já existentes no estoque.
  - Formatação da lista de compras em Markdown para melhor visualização.

**Dependências**
  - ipywidgets
  - google.generativeai
  - pathlib
  - textwrap
  - PIL
  - google.colab (para upload de arquivos e secrets)

**Como Usar**
  Configurar a API Key do Google Gemini:
  Vá em "Editar -> Configurações do Notebook" e adicione sua chave da API do Google Gemini como uma Secret com o nome GOOGLE_API_KEY.
  
  **Executar o Notebook:**
    Execute todas as células do notebook.
    Responder às Perguntas:
    O sistema exibirá widgets interativos para coletar as informações do usuário.
    Upload da Imagem (opcional):
    Se desejar, faça o upload de uma imagem da sua despensa ou geladeira.
    Gerar a Lista:
    Clique no botão "Gerar Lista".
    Visualizar a Lista:
    A lista de compras personalizada será exibida em formato Markdown.
    Exemplo de Uso
  # Respostas do Usuário
    num_pessoas = 2
    duracao = "Compra da semana"
    restricoes = ["Sem glúten", "Vegetariano"]
    refeicoes = ["Café da manhã", "Jantar"]
    alergia = "Amendoim"
  
  
  # (O código gera o prompt e envia para o Gemini)
    Use code with caution.
    Observações
    Certifique-se de ter as bibliotecas necessárias instaladas.
    A qualidade da lista de compras gerada depende da precisão e completude das informações fornecidas pelo usuário.
    

**Autor**
Enrico Lopes Marques

**Contato**
enrico.l.marques@gmail.com
