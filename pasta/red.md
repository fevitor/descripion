# Cybersecurity Preparatory School

# Desafio:RED
**Descrição:**
Ao abrir, temos um arquivo PNG para baixarmos, ao abrir, temos essa imagem:
[![red.png](https://i.postimg.cc/c494gbpw/red.png)](https://postimg.cc/9r9jsJFQ)
A primeira vista não parece conter muita coisa, mas ao analisar com o zsteg no webshell, descobrimos uma string codificada em base64.
[![Captura-de-tela-2025-05-08-213043.png](https://i.postimg.cc/qRbZX24b/Captura-de-tela-2025-05-08-213043.png)](https://postimg.cc/G8DQb8BG)
Onde, se colocarmos ele no [cyberchef](https://gchq.github.io/CyberChef/#input=Cg&oenc=65001):

[![Captura-de-tela-2025-05-08-213518.png](https://i.postimg.cc/8cxKxDFL/Captura-de-tela-2025-05-08-213518.png)](https://postimg.cc/N27kr3k0)

teremos a flag:
**picoCTF{r3d_1s_th3_ult1m4t3_cur3_f0r_54dn355_}**

concluindo o desafio.
