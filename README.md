# CodeAnalysis-RacingGame
Trabalho realizado por: Dário Ribeiro, a23489

-------------------------------INTRODUÇÃO--------------------------------


Neste trabalho, foi pedido para fazer a análise de um jogo desenvolvido em Monogame, à escolha.
Em particular, foi escolhido o jogo chamado de "RacingGame".

------------------------------ANÁLISE DE FICHEIROS-------------------------------
![image](https://user-images.githubusercontent.com/106490681/235947349-f00b37b7-fbdd-473c-a117-c4bea1fb5763.png)

Ao analisar esta imagem, podemos observar que existem 5 pastas, com nomes:

-Assets;

-Core;

-Game;

-Scenes;

-Utils.

---ASSETS---

A pasta "Assets", como o nome indica, contém as imagens, fontes e sprites que foram utilizadas para o desenvolvimento do jogo, como observado nas seguintes imagens:

![image](https://user-images.githubusercontent.com/106490681/235949899-0e22576f-b4a4-4e03-a495-d6b00a90fe7c.png)
![image](https://user-images.githubusercontent.com/106490681/235950044-e03e2c86-d2de-4a12-8d57-c68e29de33f1.png)
![image](https://user-images.githubusercontent.com/106490681/235950102-04904553-c704-4d5a-bde5-d068f4a90c57.png)
![image](https://user-images.githubusercontent.com/106490681/235950140-70fe6c9c-354f-47ee-bb95-61db424d6d07.png)

---CORE---
A pasta "Core", como o nome indica, contém a lógica para o jogo dar load para o ecrã.
![image](https://user-images.githubusercontent.com/106490681/235955650-2ecf0555-7b31-428a-96f3-30b52eb8b6a7.png)

Nesta imagem, podemos observar o código que está contido no ficheiro "BaseScene.cs", onde esta função mostrada irá encarregar-se de ser uma base para carregar os mapas, e de gerir o input de teclado e de rato.


![image](https://user-images.githubusercontent.com/106490681/235958351-45765e13-536c-4c4d-b8d8-114987ebdcc8.png)

![image](https://user-images.githubusercontent.com/106490681/235958418-7be98076-acb0-4b6d-946e-9efc7cbc22d2.png)

![image](https://user-images.githubusercontent.com/106490681/235958449-56e1a2d5-eccc-4630-b606-11fa0207be77.png)

![image](https://user-images.githubusercontent.com/106490681/235958495-097e9938-e063-41b8-a154-8c54e1657321.png)

![image](https://user-images.githubusercontent.com/106490681/235958521-5f489ed7-383b-4c10-9821-7c91f9a737eb.png)

Estas imagens representam o que contém o ficheiro "Camera.cs", onde todo este código irá manipular completamente a câmara, que neste caso, está centrada no nosso veículo (graças à função Update). Este código também permite trocar o zoom e manter o alcance da câmara se a janela onde o jogo se encontra se altera.

![image](https://user-images.githubusercontent.com/106490681/235961268-202dc23e-4e0d-4c51-9e94-835690c325fd.png)

O código que se encontra na imagem acima, que está dentro do ficheiro "DebugFieldAttribute.cs" é apenas código para facilitar o debugging.

![image](https://user-images.githubusercontent.com/106490681/235961972-be28563c-dbc3-43b1-bf27-a1762d2c9d04.png)

![image](https://user-images.githubusercontent.com/106490681/235962028-77b603ac-299b-436b-b940-9016d50f7cfa.png)

![image](https://user-images.githubusercontent.com/106490681/235962079-58e48212-2224-4819-ad25-25b40f10c147.png)

![image](https://user-images.githubusercontent.com/106490681/235962130-b1c5b1f2-e2d6-48ce-b11b-72d4260bcdaf.png)

![image](https://user-images.githubusercontent.com/106490681/235962204-c09d26db-12e7-4cb7-9f47-2c4e1dbdb460.png)

![image](https://user-images.githubusercontent.com/106490681/235962222-e58b4bc3-ec81-4371-85a7-0bb07704843f.png)

Todas as imagens acima contêm código derivado do ficheiro "Entity.cs", que em geral, serve para gerir entidades do jogo, utilizando queues.

![image](https://user-images.githubusercontent.com/106490681/235963248-ba4072cf-ef66-42d3-8014-0589cb01a6a4.png)

![image](https://user-images.githubusercontent.com/106490681/235963320-969320d6-bc04-4edc-888c-8999b00bdb40.png)

![image](https://user-images.githubusercontent.com/106490681/235963374-b734f716-5d3b-4be1-8fd6-665e03668cae.png)

![image](https://user-images.githubusercontent.com/106490681/235963415-5f7dd55f-3401-4b8d-a698-98c343c9b481.png)

![image](https://user-images.githubusercontent.com/106490681/235963458-46b5dc3e-2c95-4390-93fc-fe339471eb8a.png)

Todas as imagens acima contêm código derivado do ficheiro "GameEntity.cs", que em geral, serve para criar as entidades do jogo, que são geridas pelo código que está no ficheiro "Entity.cs", e cria as tais entidades com várias propriedades e texturas.



























---GAME---
A pasta "Game", como o nome indica, contém a lógica por detrás dos carros e dos mapas.
![image](https://user-images.githubusercontent.com/106490681/235952198-4d63b6cf-dfbe-429d-ad72-91165f1a5fee.png)
O ficheiro "Level.cs" contém o código necessário para o nível ser criado no ecrã
