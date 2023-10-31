Matheus Seabra Mazucato
Tayler Henrique


Esse código é um script escrito em C# para Unity, uma plataforma de desenvolvimento de jogos. Vou explicar o que cada parte do código faz:
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/ef64ee2a-0e60-4a1a-9b62-6ca980b70615)<br>
Essas linhas são declarações de namespaces. Elas importam bibliotecas que o código usará. Neste caso, você está usando bibliotecas do Unity para lidar com objetos 3D e física.<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/68659b68-1ea0-49e3-a9a0-d401bc7f69ce)<br>
Aqui é definida a classe Controlador, que herda de MonoBehaviour. No Unity, os scripts que controlam objetos do jogo devem herdar de MonoBehaviour.<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/6949cb28-ee33-4335-9506-1f778278979d)<br>
Uma variável privada chamada rb é declarada para armazenar uma referência a um componente Rigidbody. O Rigidbody é usado para simular a física de um objeto no jogo, como colisões e movimento.<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/2211ecba-ba62-4bc8-bd3f-cd7db1841faa)<br>
Esta é uma função chamada awake(). No entanto, deveria ser Awake() com "A" maiúsculo, para ser reconhecida pelo Unity. A função Awake() é chamada quando o objeto ao qual o script está anexado é inicializado. Aqui, estamos inicializando a variável rb obtendo uma referência ao componente Rigidbody do objeto.<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/71fba924-c0ca-4e02-b6e1-fd738800befa)<br>
Aqui, o código está pegando o componente Rigidbody do objeto ao qual o script está anexado e atribuindo à variável rb.<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/c673cbd5-053e-4f82-8964-9d90834ed493)<br>
Esta é outra função, OnCollisionEnter(). Ela é chamada automaticamente pelo Unity quando o objeto colide com outro objeto. A função recebe um parâmetro Collision que contém informações sobre a colisão.<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/35743fb0-9f7c-4da8-97a0-4d887c6ef802)<br>
O código verifica a tag do objeto com o qual ocorreu a colisão usando uma instrução switch. As tags são usadas para identificar objetos no Unity.<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/5c4fab17-1f13-4099-b254-74ba26c3f655)<br>
Se a tag do objeto colidido for "Vermelho", o objeto é destruído usando Destroy(). Isso remove o objeto da cena.<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/0964e7ce-f5f1-48f2-a780-c27accb8fb61)<br>
Se a tag do objeto colidido for "Azul", é aplicada uma força ao objeto com um vetor Vector3.back multiplicado por 3000. Isso empurra o objeto para trás.<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/2f8bb616-e409-4a68-8ed0-aa56b520e21b)<br>
Se a tag do objeto colidido for "Verde", uma mensagem é impressa no console usando print().<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/d9ac3159-c17f-46b1-a9a8-da3bb7821657)<br>

eu e minha dupla fizemos uma cena simples apenas para entender como funcionava os tipos de colisores, fizemos alguns retangulos onde cada um deles faz um tipo de colisão diferente sendo assim o verde empurra vermelho quebra e o azul repele. Fizemos um codigo de movimentação e um codigo que faz a camera seguir o personagem<br>
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/97186404-76b6-43f4-acb0-a626f9a8ef01)
![image](https://github.com/MatheusSeabra/Unity-colision/assets/101134295/e077dc1e-405c-40f4-9d56-20e19e00ec15)<br>

os colisores mais utilizados foi Static Collider e o RigidBody Collider<br>



https://github.com/MatheusSeabra/Unity-colision/assets/101134295/9897a022-db59-4249-bbf7-fc22e58b03ca


