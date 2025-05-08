# Cybersecurity Preparatory School

# Desafio:Flag hunters
**Descrição:** 
O programa contém uma letra de música com versos e um refrão oculto. O objetivo é fazer com que o refrão seja impresso durante a execução.

O código fornecido define uma letra de música com versos e um refrão oculto. A função **reader** é responsável por controlar o fluxo de execução, permitindo que o programa "cante" os versos e revele o refrão quando acionado.

🧠 Compreendendo o Fluxo
- O programa começa a execução a partir do marcador [VERSE1] e quando encontra a palavra-chave REFRAIN, ele altera o fluxo para o trecho do refrão.
- A interação com o usuário ocorre quando o programa solicita uma entrada para o "CROWD".Após alguns testes, percebo que o comando que eu digitei se repete.
 Desde o inicio, é possivel ver o comando 
**flag = open('flag.txt', 'r').read()**
que mostra que a flag só sera entregue quando o codigo secreto for inserido
[![Captura-de-tela-2025-05-08-200112.png](https://i.postimg.cc/pddbtWGF/Captura-de-tela-2025-05-08-200112.png)](https://postimg.cc/18bYGQZm)

**Solução**
apos analisar o codigo, percebi na parte do "refrão", se colocada a palavra certa, ele fornecerá a chave, senão ele repetira o refrão, e este **secret_intro** é o verso que contém nossa bandeira

[![Captura-de-tela-2025-05-08-201156.png](https://i.postimg.cc/65HfmBvS/Captura-de-tela-2025-05-08-201156.png)](https://postimg.cc/KRMTKSQr)

No código, vemos que o *secret_introverse* é adicionado ao topo do *song_flag_hunter*, no entanto, o leitor começa a ler a partir do [VERSE1], para isso precisamos que ele exiba todos os versos.
Sabemos que o script aceita entrada do usuário, e essa entrada não é higienizada e podemos usar o comando "RETURN" para forçar o leitor a ler qualquer linha específica, Como sabemos que o verso que tem nossa bandeira começa logo no começo, precisamos passar o "RETURN 0 "para o script. No entanto, se fizermos isso, o script simplesmente nos retornará o eco, tratando ele apenas como uma string. Para garantir que o script interprete o "RETURN 0" como um comando em vez de uma string, precisamos ajustar nossa entrada e em vez de usar apenas "RETURN 0", usaremos "some_string;RETURN 0".
dessa forma, revelando a flag escondida

[![Captura-de-tela-2025-05-08-203345.png](https://i.postimg.cc/rmJfyxDy/Captura-de-tela-2025-05-08-203345.png)](https://postimg.cc/G84FqBP6)

sendo ela: 
**picoCTF{70637h3r_f0r3v3r_ac197d12}**
concluindo assim, o desafio.
