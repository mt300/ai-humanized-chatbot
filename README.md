# Chat Bot com IA

Este projeto explora a integração do ChatGPT com o WhatsApp, transformando o chatbot em um assistente virtual capaz de realizar tarefas como falar com clientes, responder a perguntas e muito mais, com um toque humanizado nas conversas.

## 📚 Como funciona

A integração começa com o [wpconnect](https://github.com/wppconnect-team/wppconnect), que estabelece a conexão com o WhatsApp. <br/>
As mensagens recebidas são então processadas pela API do ChatGPT ou Gemini, que gera respostas coerentes e personalizadas.<br/>
Utilizamos um [assistant](https://platform.openai.com/docs/assistants/overview) da OpenAI, que é um do modelo OpenAI que foi pré-configurado com prompts detalhados. </br>
No caso do Gemini usamos um prompt pronto para instruções do modelo. </br>
Esses prompts orientam o assistente sobre como responder de maneira coerente e personalizada, assegurando que as interações não só se mantenham relevantes e engajantes, mas também reflitam uma abordagem humana e natural na conversação.

## 🚀 Como rodar o projeto
1 - Clone o repositorio em uma pasta local
2 - Crie um arquivo .env seguindo o padrao de .env.example e preenchendo com suas informações e chaves API desejadas (Gemini ou OpenAI)
3 - Configurando o bot com os comandos abaixo e siga o passo a passo do terminal 
```
  cd ai-humanized-chatbot
  npm install
  npm run config
```
4 - Rodando o bot
```
  npm run dev
```

### 📌 Prompt do Assistant utilizado para marcar dates

Aqui o prompt que usei para o projeto em questão onde o chatbot deve atender um cliente de uma empresa de desenvolvimento de software.

```
Você é um atendente humanizado e responsavel por falar com os clientes sobre os novos projetos a serem executados pela empresa. Trate-os com educação e extraia o máximo de informações possiveis sobre o projeto. Quando julgar as informações suficientes para montar um orçamento comunique que ja tem as informaçoes necessárias e peça um tempo de 48h para envio do orçamento detalhado do pedido. 
```

