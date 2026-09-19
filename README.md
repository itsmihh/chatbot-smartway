# Chatbot SmartWay - Bibi (Assistente Virtual)

Este repositório contém a implementação de um chatbot especialista e não-alucinatório baseado na API do Google Gemini (`google-genai`). O projeto foi desenvolvido como uma solução de atendimento automatizado para o aplicativo **SmartWay**, um assistente de mobilidade urbana.

## Sobre o Projeto
A assistente virtual **Bibi** foi programada com uma **Base de Conhecimento Fechada (System Instruction)**, garantindo que ela responda apenas a informações oficiais do projeto e recuse perguntas fora do seu escopo.

###  Funcionalidades Principais
* **Apresentação e Identidade:** Apresenta-se como Bibi, assistente do SmartWay.
* **Respostas Baseadas em Contexto:** Fornece detalhes sobre o aplicativo (onboarding, mobilidade, regras) e suas tecnologias (React Native, Java, PostgreSQL).
* **Bloqueio de Alucinação:** Responde exatamente *"Desculpe, não possuo informações sobre esse assunto."* caso a dúvida não esteja na base.
* **Controle de Sessão e Resumo Automático:** Limita a conversa a exatas **3 interações**, gerando um resumo consolidado das dúvidas ao final da 3ª resposta e encerrando o atendimento.

### Configuração
Para executar o chatbot, é necessário configurar uma chave de API do Google Gemini.

Por questões de segurança, a chave de API não é armazenada diretamente no código ou no repositório. O projeto utiliza o **Google Colab Secrets** para armazenar a chave durante a execução.

* **Configurar a chave no Google Colab**
No Google Colab, acesse o menu de Secrets e adicione uma nova chave com o seguinte nome:

GOOGLE_API_KEY

O valor deve ser preenchido com a chave de API do Google Gemini.

* **Arquivo env.example**
O repositório contém o arquivo env.example apenas como referência dos parâmetros necessários para a configuração:

GOOGLE_API_KEY=

O arquivo não possui o valor real da chave por questões de segurança.

* **Execução**
Após configurar a chave no Google Colab, execute as células do notebook na ordem apresentada. O chatbot utilizará a chave armazenada nos Secrets para realizar as requisições à API do Google Gemini.

