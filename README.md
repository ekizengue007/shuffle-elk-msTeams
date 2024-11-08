![image](https://github.com/user-attachments/assets/363c7705-d6b4-44af-9af8-f92cd49fa47b)# shuffle-elk-msTeams

Diagrama do Projecto
![image](https://github.com/user-attachments/assets/5dc1b9d0-301d-4055-a0b0-0b3b8a71a80e)
1. Passo - Ter os alertas configurados no ELK ;)
2. Realizar as validações abaixo
2.1 Verificar em que index os alertas estão a ser salvos
   Na imagem abaixo, selecionando um dos alertas, podemos observar que os alertas estão na index ".siem-signal-default" ( não precisas pegar o número)
   ![image](https://github.com/user-attachments/assets/c3488e20-ac7b-4813-9c66-c19dc5569295)
4. Pesquisar por cada nodo e organizar conforme a imagem acima ;)
   ![image](https://github.com/user-attachments/assets/4305f946-ca76-43ef-b9af-f2e5286fb8e9)
   ![image](https://github.com/user-attachments/assets/74740a22-bfa1-4c01-8996-7331506f2361)
   ![image](https://github.com/user-attachments/assets/3c22571e-af3f-4aa7-af00-c5a76cf5537d)
5. Vamos começar com o elasticsearch
   Em name: teu nome
   Find Actions: Index search
   Index: Usar a index onde se encontram os alertas : Passo 2.1
   ![image](https://github.com/user-attachments/assets/ffda3985-1b7b-4420-bfba-362414ee3a2c)
   Em autenticaton temos:
   ![image](https://github.com/user-attachments/assets/43938bb8-ba38-4925-bd54-757a2a95e6b3)
   Em headers
   ![image](https://github.com/user-attachments/assets/fa4c22a7-b922-4ae2-8503-95f92274d0a0)
   Em body
   ![image](https://github.com/user-attachments/assets/16eb7db9-2e7c-408c-b6c6-e5d033ba400d)
   ![image](https://github.com/user-attachments/assets/1edb577f-cc7c-426a-a5b1-ac9018303b2d)
   Copiar em body-elastic.json
   Agora vamos em Suffle Tools
   ![image](https://github.com/user-attachments/assets/7a69bf4e-df90-4d25-8c3d-a05767751682)
   Name: Filtro_Lista
   Find Actions : Filter Lister
   ![image](https://github.com/user-attachments/assets/5cc1c546-f6c3-44c4-b17b-0c7b4ae0dab5)
   Another Shuffle Tools
   ![image](https://github.com/user-attachments/assets/89f17697-a3c4-42f4-bc5d-507a7277bcf3)

   Para o MS Teams, recomendo seguir os passos da documentação oficial ;)
   https://github.com/Shuffle/python-apps/tree/master/unsupported/microsoft-teams/1.0.0
   Seguindo os passos presentes na documentação e copiando a nossa webhook url temos
   ![image](https://github.com/user-attachments/assets/433f6dd5-1cbe-47b8-8dc4-8890671f88a1)
   A "message" se encontra em message-teams.json
   
   Por ultimo temos então o schedule
   ![image](https://github.com/user-attachments/assets/d60f8c23-a40b-404b-a47f-4f3f0fa6f752)
   onde 300sec=5 minutos :)
   


   

   




   





   
