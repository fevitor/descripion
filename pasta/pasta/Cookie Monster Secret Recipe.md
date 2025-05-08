# Cybersecurity Preparatory School



# Desafio:Cookie Monster Secret Recipe
Neste desafio, você assume o papel de um analista cibernético encarregado de localizar uma receita secreta que está oculta em algum lugar dentro do site do Cookie Monster. A proposta simula uma tarefa de exploração web típica de CTFs ou auditorias de segurança básica. 
Temos como objetivo Localizar a receita secreta escondida no site, aplicando técnicas de information gathering, file enumeration e source code inspection. Ao encontrar o conteúdo correto (texto, flag, link ou arquivo), apresentárei como prova da descoberta.
- Localizar a receita secreta escondida no site
- -apresentárei a flag como prova da descoberta.

# descrição do problema:
O desafio apresenta o seguinte texto "O Monstro dos Come-Come escondeu sua receita secreta de biscoitos em algum lugar do seu site. Como um aspirante a detetive de biscoitos, sua missão é desvendar esse segredo delicioso. Você consegue enganar o Monstro dos Come-Come e encontrar a receita escondida?
Você pode acessar o Cookie Monster **aqui** e boa sorte"
com o "aqui" em negrito nos levando um site com o seguinte endereço:http://verbal-sleep.picoctf.net:49480/
[![Captura-de-Tela-13.png](https://i.postimg.cc/VL8RCSWj/Captura-de-Tela-13.png)](https://postimg.cc/vD0fRZjB) site ao clicar no link

# solução 
Apos acessar o site, logo de cara ispecionei ele com as ferramentas de desenvolvedor,e indo em cookies onde achei ele,porém criptografado em [base64](https://pt.wikipedia.org/wiki/Base64)


[![Captura-de-tela-2025-05-08-184107.png](https://i.postimg.cc/BbGVbmvF/Captura-de-tela-2025-05-08-184107.png)](https://postimg.cc/KkJNsrBc)
cookie criptografado

Apos achar o cokkie, eu o descriptografei no [webshell](https://webshell.picoctf.org/) dando como resultado a flag
**picoCTF{c00k1e_m0nster_l0ves_c00kies_AC8FCD75}**
concluindo assim o desafio.
