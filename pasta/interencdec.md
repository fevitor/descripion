
# Cybersecurity Preparatory School

# Desafio:interencdec
**Descrição:**
Assim que abrimos, vemos a seguinte descrição "Você consegue entender o verdadeiro significado deste arquivo? Baixe o arquivo aqui", baixando o arquivo e usando o [netcat](https://www.devmedia.com.br/netcat-o-canivete-suico-tcp-ip-revista-infra-magazine-8/26299), recebemos esse codigo,
**YidkM0JxZGtwQlRYdHFhR3g2YUhsZmF6TnFlVGwzWVROclh6ZzVNR3N5TXpjNWZRPT0nCg==**
onde se tentar usar a [base64](https://pt.wikipedia.org/wiki/Base64) no [ciberchef](https://gchq.github.io/CyberChef/#input=d3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrXzg5MGsyMzc5fQo&oenc=65001) obteremos 
**b'd3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrX20wMjEyNzU4fQ=='**
[![Captura-de-tela-2025-05-08-205505.png](https://i.postimg.cc/SKQrTjZw/Captura-de-tela-2025-05-08-205505.png)](https://postimg.cc/YvVYj2B3)

Porém ainda esta codificado, mas se removermos as aspas e o primeiro b e colocando denovo no cyberchef, fica:
**wpjvJAM{jhlzhy_k3jy9wa3k_890k2379}**

[![Captura-de-tela-2025-05-08-205949.png](https://i.postimg.cc/Dwnd08K8/Captura-de-tela-2025-05-08-205949.png)](https://postimg.cc/hfZ734vB)
Onde ele começa a ganhar forma de flag.
agora, se usarmos a cifra de cezar, utilizando de um recurso do proprio cyberchef, chamado de *rote13 brute force* descobrimos a flag.

[![Captura-de-tela-2025-05-08-211226.png](https://i.postimg.cc/hjTfV1Lg/Captura-de-tela-2025-05-08-211226.png)](https://postimg.cc/9RXmhTgN)

descobrimos então que a flag é:
**picoCTF{caesar_d3cr9pt3d_890d2379}**
concluindo então o desafio.




