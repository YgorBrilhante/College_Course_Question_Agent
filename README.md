# Agente de dúvidas de curso universitário
## Fui convidado pelo Centro Universitário Católico Salesiano Auxilium para fazer um agente de IA que responde dúvidas pelo WhatsApp sobre o curso de Tecnologia e Desenvolvimento de Sistemas.

### Situação
* Haveria uma feira de profissões onde colégios visitariam a universidade para conhecer cursos e carreiras como forma de incentivo à busca pelo ensino superior. 

### Iniciativa
* Fizemos um Agente de IA para os alunos visitantes interagirem através do WhatsApp e abrirem os olhos para a carreira de desenvolvimento de software que explica e tira dúvidas sobre o curso, vestibular, matérias, atuação profissional, salários e etc!

## Tecnologias:
* n8n 
* EvolutionAPI (WhatsApp)
* Redis
* NocoDB
* OpenAI API
* PGVector (RAG e Fine-Tuning)


### Fluxo Completo
![Fluxo completo](https://github.com/user-attachments/assets/99eb9be0-1897-465c-8f4b-7bc87b61cc51)


### 1ª parte - Recebimento da mensagem por WebHook, verificação de registro do número no NocoDB e verificação do tipo de mensagem
![fluxo 1](https://github.com/user-attachments/assets/0340b38b-2050-47a4-8038-af0492a0a4f0)

### 2ª parte - Processamento de audio e transcrição ou buffer para agrupamento de mensagens de texto picadas
![fluxo 2](https://github.com/user-attachments/assets/e6459729-6ae9-46c0-ae7f-d5a857dfd289)

### 3ª parte - Validação de conteúdo pelo guardrails, processamento pelo AI Agent, envio de resposta por WhatsApp
![fluxo 3](https://github.com/user-attachments/assets/cc0ee438-fcca-4eea-bdf2-5ac895766b30)
