# 🤖 Chatbot com a API do Google Gemini

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jvmorva/Chatbot-Gemini/blob/main/Chatbot_Gemini.ipynb)

Este notebook Google Colab demonstra a criação de um chatbot básico utilizando a API do Google Gemini.

## 🔍 Visão Geral

O código configura um ambiente para interagir com a API do Google Gemini, lista os modelos disponíveis, e demonstra como criar e interagir com um chat, incluindo a configuração de instruções do sistema e a recuperação do histórico da conversa.

## 📦 Requisitos

Para executar este código, você precisará de:

- Uma conta Google.
- Uma chave de API do Google Gemini.
>_Dica:_ Uma maneira fácil de conseguir é através do Google AI Studio - basta acessar - https://aistudio.google.com/app/apikey - fazer login com sua conta Google e clicar em "Create API Key").
- A biblioteca `google-genai` instalada.
- A chave de API do Gemini armazenada nos secrets do Google Colab com o nome `GOOGLE_API_KEY`.

## ⚙️ Instalação

1. Instale a biblioteca `google-genai` na versão 1.15.0: `pip install google-genai==1.15.0`
> A versão está congelada para garantir compatibilidade, já que a biblioteca ainda está em constante evolução e pode passar por mudanças frequentes.
2. Configure sua chave de API:
- No Google Colab:
Armazene sua chave de API do Google Gemini nos secrets do Colab.
Vá em “Secrets” (ícone de chave) na barra lateral esquerda, clique em + Novo secret e crie um secret com o nome GOOGLE_API_KEY e o valor da sua chave.
>Se você optou por importar a API KEY do Google AI Studio, basta clicar em “Chaves da API Gemini” e importá-la.

- Em ambiente local: Defina a variável de ambiente `GOOGLE_API_KEY`.

## ▶️ Como usar

1. Execute as células do notebook sequencialmente.
2. A célula que contém o loop `while prompt != "fim":` permitirá que você interaja com o chatbot em tempo real. Digite suas perguntas e pressione Enter.
3. Para encerrar a conversa, digite `fim` e pressione Enter.

## 🔧 Funcionalidades

- Autenticação com a API do Google Gemini.
- Listagem dos modelos Gemini disponíveis.
- Criação de instâncias de chat.
- Envio de mensagens para o chatbot.
- Configuração de instruções do sistema para o chatbot.
- Recuperação e exibição do histórico da conversa.

## 🎨 Personalização

Você pode modificar o modelo Gemini utilizado alterando a variável `modelo`. Além disso, a configuração do chat pode ser ajustada através do `types.GenerateContentConfig` para alterar o comportamento do chatbot.
