# Chatbot SmartWay - Bibi (Assistente Virtual)

Este repositório contém a implementação de um chatbot especialista e não-alucinatório baseado na API do Google Gemini (`google-genai`). O projeto foi desenvolvido como uma solução de atendimento automatizado para o aplicativo **SmartWay**, um assistente de mobilidade urbana.

## Sobre o Projeto
A assistente virtual **Bibi** foi programada com uma **Base de Conhecimento Fechada (System Instruction)**, garantindo que ela responda apenas a informações oficiais do projeto e recuse perguntas fora do seu escopo.

###  Funcionalidades Principais
* **Apresentação e Identidade:** Apresenta-se como Bibi, assistente do SmartWay.
* **Respostas Baseadas em Contexto:** Fornece detalhes sobre o aplicativo (onboarding, mobilidade, regras) e sua tecnologias (React Native, Java, PostgreSQL).
* **Bloqueio de Alucinação:** Responde exatamente *"Desculpe, não possuo informações sobre esse assunto."* caso a dúvida não esteja na base.
* **Controle de Sessão e Resumo Automático:** Limita a conversa a exatas **3 interações**, gerando um resumo consolidado das dúvidas ao final da 3ª resposta e encerrando o atendimento.


Chatbot desenvolvido para a aula de IA usando Gemini API
