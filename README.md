# CodeAnalysis-RacingGame
Trabalho realizado por: Dário Ribeiro, a23489

-------------------------------INTRODUÇÃO--------------------------------


Neste trabalho, foi pedido para fazer a análise de um jogo desenvolvido em Monogame, à escolha.

Em particular, foi escolhido o jogo chamado de "RacingGame".

O RacingGame é um jogo de corrida 2D Top-Down, feito em C# e Monogame, com o objetivo de acabar as voltas todas do cicuito em primeiro lugar, como qualquer outro jogo de corrida.

É possível andar para a frente, travar, virar, colidir e andar em slow-motion.

Os controlos são:

Z - Andar para a frente;
S - Travar / andar para trás;
Q - Andar para a esquerda;
D - Andar para a direita;
CAPS-LOCK - Slow-Motion.


------------------------------ANÁLISE DE FICHEIROS / CÓDIGO-------------------------------
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

Estas imagens representam o que contém o ficheiro "Camera.cs", onde todo este código irá manipular completamente a câmara, que neste caso, está centrada no nosso carro (graças à função Update). Este código também permite trocar o zoom e manter o alcance da câmara se a janela onde o jogo se encontra se altera.

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

![image](https://user-images.githubusercontent.com/106490681/235976194-8e75f272-4227-42eb-b427-8e956a961b89.png)

![image](https://user-images.githubusercontent.com/106490681/235976238-ca27a5e3-5eaa-4703-ae79-32f4f7a063b0.png)

A pasta "Game", como o nome indica, contém a lógica por detrás dos carros e dos mapas, interpretando-os como os "entities", já referidos anteriormente.

O código que existe dentro do ficheiro "AIRaceCarEntity.cs" representa os carros adversários, controlados pelo computador, pois este jogo é apenas single-player.

![image](https://user-images.githubusercontent.com/106490681/235977875-266bc277-806d-4721-a1d8-26211a446678.png)

![image](https://user-images.githubusercontent.com/106490681/235977920-4cbedf44-e11d-49cf-bc4c-e9a928714c6f.png)

![image](https://user-images.githubusercontent.com/106490681/235978583-db6299b1-9733-499e-bb55-b6c7252f0cc8.png)

![image](https://user-images.githubusercontent.com/106490681/235978617-c335fdab-d70d-4acc-a750-8243f430c57f.png)


O código que existe dentro do ficheiro "MapEntity.cs" representa a entidade "Map", e este código contém métodos para renderizar o mapa, e verificar as colisões com o mesmo.

![image](https://user-images.githubusercontent.com/106490681/235978756-9062aced-8a4b-480a-b5bf-3cb0a169a8f3.png)

![image](https://user-images.githubusercontent.com/106490681/235978848-540fcf21-5abf-4b68-8918-aa739402d753.png)

![image](https://user-images.githubusercontent.com/106490681/235978918-c5b99172-2d6c-4f11-8ba4-9d5d7a6d3fa3.png)

![image](https://user-images.githubusercontent.com/106490681/235978950-3a92ef02-e6b7-40bb-a1de-8f430a91d512.png)


O código que existe dentro do ficheiro "PlayerRaceCarEntity.cs" representa a entidade "RaceCarEntity", mas especificada para o jogador. 
Ele verifica o input do carro do jogador, e mantém registo dos seus tempos de volta.

![image](https://user-images.githubusercontent.com/106490681/235980096-66e55b6a-1f24-45b0-945c-9a689a0e46ee.png)

![image](https://user-images.githubusercontent.com/106490681/235980129-1e80cc70-c8ed-46ad-b1f0-de76a6e80bce.png)

O código que existe dentro do ficheiro "RaceCarEntity.cs" representa a "entidade-mãe" da entidade do carro do computador, e do carro do jogador. Apenas contém toda a lógica necessária para o carro se movimentar, e a informação necessária em relação ao piloto em particular, como as voltas que já completou.

![image](https://user-images.githubusercontent.com/106490681/235980979-d2e95ceb-b3cf-4ec2-b378-1a00a61535d9.png)

![image](https://user-images.githubusercontent.com/106490681/235981018-e3ac491c-257e-43c0-b763-49681c0b805c.png)

![image](https://user-images.githubusercontent.com/106490681/235981042-b8af304d-118c-40f8-99ba-a09493b1edf4.png)

![image](https://user-images.githubusercontent.com/106490681/235981065-fd2af8a5-9497-4379-ab25-ef2e50c05943.png)

![image](https://user-images.githubusercontent.com/106490681/235981128-9371f63a-717a-41e7-9b6f-5a1e200e3914.png)



O ficheiro "Level.cs" contém o código necessário para o nível ser criado no ecrã, através do ficheiro .xml que o desenvolvedor deste jogo utilizou.

![image](https://user-images.githubusercontent.com/106490681/235983018-c72f9fcc-0313-4345-89c6-fedd8fbe8eb8.png)

![image](https://user-images.githubusercontent.com/106490681/235983056-78dc4827-76fa-4698-b650-7269868bbd80.png)

![image](https://user-images.githubusercontent.com/106490681/235983084-b3373dbc-b732-4812-b127-e2f779ddcebb.png)

![image](https://user-images.githubusercontent.com/106490681/235983151-6de8234b-e7c9-4457-b307-7490abf5aea1.png)

![image](https://user-images.githubusercontent.com/106490681/235983183-958262d5-0013-4002-9282-0f2eacb89803.png)

![image](https://user-images.githubusercontent.com/106490681/235983200-92dd3689-5ee3-407b-a6c0-d0cb1a3de1c4.png)

---SCENES---

![image](https://user-images.githubusercontent.com/106490681/235985705-495f1666-b752-4088-8d60-ae947e599e52.png)

Dentro desta pasta, existem os ficheiros necessários para carregar o mapa, e para detetar colisões ("GameScene.cs" e "SATDemoScene.cs", respetivamente).

No ficheiro "GameScene.cs", observamos:

![image](https://user-images.githubusercontent.com/106490681/235983975-4cf4c9ee-e22a-4d82-b31d-c13916926895.png)

![image](https://user-images.githubusercontent.com/106490681/235984040-2eca956f-7839-45e8-832e-01b8870d8854.png)

![image](https://user-images.githubusercontent.com/106490681/235984160-a939d36b-8ed3-46f8-8cf0-25f6b6baa663.png)

![image](https://user-images.githubusercontent.com/106490681/235984194-ecb263c9-35e1-460c-83c7-1c81aff5d5e4.png)

![image](https://user-images.githubusercontent.com/106490681/235984249-1778e827-ef0c-40f4-a616-f916c1a6acf7.png)

![image](https://user-images.githubusercontent.com/106490681/235984291-6326e4ef-3d0f-4b10-8b71-0a82648f5e7a.png)

Também contém funções para representar o tempo de volta, e representa o nome do jogador, acima do carro, e os nomes dos bots.(Neste caso, os bots apenas estão numerados.)

No ficheiro "SATDemoScene.cs", observamos o sistema de colisões utilizado.
Este sistema é baseado na condição de polígonos convexos se intersetam.

![image](https://user-images.githubusercontent.com/106490681/235984663-c6f28bc2-20c3-4725-b913-0695ee2772b8.png)

![image](https://user-images.githubusercontent.com/106490681/235984686-5fdf6d21-d0dc-41f8-a83d-880758b9a58c.png)

![image](https://user-images.githubusercontent.com/106490681/235984717-e71d154f-3b94-43aa-a416-3deec3bb0650.png)

![image](https://user-images.githubusercontent.com/106490681/235984742-455ac398-86a7-48a5-8eae-fb520ff7a67b.png)

![image](https://user-images.githubusercontent.com/106490681/235984769-e76cf544-9b7d-4b3b-a4e7-9b799c903fb7.png)

---UTILS---

Esta pasta contém código utilitário, e parte da lógica do jogo.

![image](https://user-images.githubusercontent.com/106490681/235985613-8663ce4a-1b2a-4719-b6f8-6bcb639dd9ae.png)

![image](https://user-images.githubusercontent.com/106490681/235986098-bdd407a8-292d-4fe6-b808-71d34e092d3c.png)

![image](https://user-images.githubusercontent.com/106490681/235986221-4f323bd9-9154-4a5a-b874-75315477717d.png)

![image](https://user-images.githubusercontent.com/106490681/235986277-b7cef82b-ae8c-41ef-88dc-7572e432c782.png)

![image](https://user-images.githubusercontent.com/106490681/235986397-4dc2be6a-ab15-4f6b-a2e2-12545f2cd606.png)

Nas imagens acima, podemos observar o código que contém o ficheiro "Assets.cs". Este apenas contém código para gerir a cache e os assets utilizados no jogo.

No ficheiro "InputManager.cs", podemos ver que lá existe apenas o código para gerir inputs de teclado e rato, sendo este ficheiro a mãe. 

Nele, é utilizado a abordagem de "KeyPressed", "KeyReleased", "KeyUp", ou "KeyDown".

![image](https://user-images.githubusercontent.com/106490681/235987922-12468e37-c294-4b68-b7e2-273910b8fa0c.png)

![image](https://user-images.githubusercontent.com/106490681/235987963-174c5f4c-0a51-4221-9353-dee1a88f9659.png)

![image](https://user-images.githubusercontent.com/106490681/235987995-bcb9d0ea-eaca-444b-85ab-6691d1f35193.png)

![image](https://user-images.githubusercontent.com/106490681/235988028-9f719f7f-eb88-4ace-a227-750571c1955c.png)

![image](https://user-images.githubusercontent.com/106490681/235988067-e365c4a2-ad9d-4077-96cd-57671999108c.png)

No ficheiro "MathUtils.cs", existe toda a lógica matemática ligada ao jogo.

![image](https://user-images.githubusercontent.com/106490681/235989711-2edb4a59-a053-45db-b315-d6944524533c.png)

![image](https://user-images.githubusercontent.com/106490681/235989762-116f4b37-b0ed-483a-8aa1-302d1cc5b95c.png)
 
![image](https://user-images.githubusercontent.com/106490681/235990104-1cbcdc7f-012f-4477-9ced-a1356f6b99ec.png)

No ficheiro "SAT.cs", existe a implementação do Separating Axis Theorem (SAT), já explicada anteriormente.

![image](https://user-images.githubusercontent.com/106490681/235990313-3d66d28f-ab12-4948-8fa3-90d2922d0618.png)

![image](https://user-images.githubusercontent.com/106490681/235990352-f15fabb4-fddb-479f-ab06-668ee0747304.png)

![image](https://user-images.githubusercontent.com/106490681/235990421-1ba964b3-b9e1-4724-9530-8fdc45ea4a61.png)

![image](https://user-images.githubusercontent.com/106490681/235990485-93f5b41b-a418-4f2a-b3d3-c537cfe3c958.png)

![image](https://user-images.githubusercontent.com/106490681/235990546-9418663a-5ae8-4f5a-8391-3beced3d3490.png)

![image](https://user-images.githubusercontent.com/106490681/235990672-0f6b12cd-8c7f-4aa0-a326-ed9592cbd265.png)

![image](https://user-images.githubusercontent.com/106490681/235990698-a1ef0077-9f76-4595-9461-80ccfb1ad944.png)

![image](https://user-images.githubusercontent.com/106490681/235990729-ea2bb68c-b0f9-4e38-9570-bfcc20d87b4b.png)

![image](https://user-images.githubusercontent.com/106490681/235990967-097db63a-102d-47e5-9d1f-ffb1997a489b.png)

![image](https://user-images.githubusercontent.com/106490681/235991071-373db83a-abf7-4211-83d9-48575378d1a7.png)

![image](https://user-images.githubusercontent.com/106490681/235991101-29205eaf-60d8-47ca-a56f-75fd0131ce62.png)

![image](https://user-images.githubusercontent.com/106490681/235991116-0e7285be-e826-42f0-b823-979c3e8f4e7f.png)

No ficheiro "SpriteBatchUtils.cs", existe código apenas destinado a debug.

![image](https://user-images.githubusercontent.com/106490681/235991295-f1207e91-0a09-413c-bfae-245b8681d5c3.png)

![image](https://user-images.githubusercontent.com/106490681/235991329-e21b1072-862d-48f7-8373-e63c50543a75.png)

No ficheiro "StringUtils.cs", existe código destinado a nomear as posições de cada carro, em inglês (1st, 2nd, 3rd, 4th, e assim sucessivamente).

![image](https://user-images.githubusercontent.com/106490681/235991556-09500d01-5735-462e-b65f-3479ace413f5.png)

No ficheiro "Tiled.cs", existe código destinado a ler um tileset de formato .xml (convém notar que apenas suporta os dados de colisão de polígonos, devido ao sistema SAT explicado anteriormente).

![image](https://user-images.githubusercontent.com/106490681/235992892-5d952b07-534a-4492-9a3a-d3751b921efa.png)

---GAME.CS---
No ficheiro "Game.cs", existe o código que irá servir para fazer o jogo funcionar, isto é, para conseguir abrir, e colocar tudo o necessário no ecrã e todas as funcionalidades executarem sem problemas. Também existe um modo "slow-motion", que ativa ao carregar na tecla CAPS-LOCK.

![image](https://user-images.githubusercontent.com/106490681/235995113-18c95937-8489-4ccf-bc98-1e733c2bf3e1.png)

![image](https://user-images.githubusercontent.com/106490681/235995175-ded2a2e4-04ed-43c1-9fd3-6b938a699ad3.png)

![image](https://user-images.githubusercontent.com/106490681/235995212-d29df184-ee1e-4e28-9829-d51a2024a825.png)

![image](https://user-images.githubusercontent.com/106490681/235995265-dad68962-3472-44b9-a8d5-010289feb7e2.png)

![image](https://user-images.githubusercontent.com/106490681/235995332-93b4d857-7f4c-49fc-a5b1-8df3c4269767.png)

![image](https://user-images.githubusercontent.com/106490681/235995382-480c2167-1202-40a6-b2bd-833ca8f1dd0e.png)

---RESTO DE FICHEIROS---
O resto dos ficheiros deste jogo apenas contêm conteúdos relacionados com o GitHub, o logótipo do Monogame, um P.S escrito pelo desenvolvedor do jogo, e a função Main, que apenas contém um comando para abrir o jogo.

![image](https://user-images.githubusercontent.com/106490681/235996275-a19c347d-af7f-431a-a5e1-49fa7582fcf0.png)

![image](https://user-images.githubusercontent.com/106490681/235996319-65111435-12bf-4ba0-9f39-28900b914763.png)

![image](https://user-images.githubusercontent.com/106490681/235996355-daf29edd-abb7-4d7d-94d1-0c6783b8f4ac.png)
