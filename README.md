# Programa de cadastro 🎲
 Programa de cadastro de cartão de passagem de ônibus, cadastro de usuário, motorista e ônibus. Para o armazenamento das informações foi utilizado o banco de dados na nuvem Azure SQL, a partir de um programa em Python.
 
 
Linguagem utilizada | Descrição do Projeto | Ferramenta 
---|---|---
<a href="https://www.python.org/">Python</a> e SQL | Programa de cadastro | <a href="https://www.jetbrains.com/pt-br/pycharm/">Pycharm</a> e <a href="https://azure.microsoft.com/pt-br/free/sql-database/search/?&ef_id=Cj0KCQiA_bieBhDSARIsADU4zLfxZCF_8VGj-v2H8f5P1vWTCuhXPxLx-k9QzAK7XukAtyTHZRJ7PksaArgiEALw_wcB:G:s&OCID=AIDcmmzmnb0182_SEM_Cj0KCQiA_bieBhDSARIsADU4zLfxZCF_8VGj-v2H8f5P1vWTCuhXPxLx-k9QzAK7XukAtyTHZRJ7PksaArgiEALw_wcB:G:s&gclid=Cj0KCQiA_bieBhDSARIsADU4zLfxZCF_8VGj-v2H8f5P1vWTCuhXPxLx-k9QzAK7XukAtyTHZRJ7PksaArgiEALw_wcB">Azure SQL</a> 


Para atingir o objetivo de guardar os dados inseridos pelo usuário que alimenta o banco de dados, o primeiro passo foi criar um schema dentro do banco com um `CREATE SCHEMA`. Após isso, usando um `CREATE TABLE` foram criadas 4 tabelas: 

* usuário;

 <img width="194" alt="tabelaUsuario" src="https://user-images.githubusercontent.com/98350733/214062979-c47451f1-203e-4318-81ba-4cdbbfb4dbc0.png">
 
* cartão;

 <img width="275" alt="tabelaCartao" src="https://user-images.githubusercontent.com/98350733/214062965-f942c550-997a-4016-a871-aa1b790a1966.png">

* onibus;

 <img width="265" alt="TabelaOnibus" src="https://user-images.githubusercontent.com/98350733/214062975-248c6ffa-1acf-4218-b3eb-6ff5e4240136.png">

* motorista

 <img width="272" alt="tabelaMotorista" src="https://user-images.githubusercontent.com/98350733/214062973-c4847ee9-8dff-4607-bf16-9be7427f904d.png">
 

Como o programa foi desenvolvido no <a href="https://www.jetbrains.com/pt-br/pycharm/">Pycharm</a>, foi necessário fazer a conexão com o banco de dados importando a biblioteca <a href="https://learn.microsoft.com/pt-br/sql/connect/python/pyodbc/step-3-proof-of-concept-connecting-to-sql-using-pyodbc?view=sql-server-ver16">pyodbc</a>.

Neste projeto, foi utilizado o conceito de <a href="https://realpython.com/python3-object-oriented-programming/">Programação orientada a objetos</a>. Sendo assim, foram criadas classes com seus atributos privados. Portanto, foi necessário utilizar <a href="https://realpython.com/python-getter-setter/">métodos setters e getters's</a>.


- [x] Ao executar o `__main__`, o menu aparece conforme a tela abaixo:


 <img width="454" alt="main" src="https://user-images.githubusercontent.com/98350733/214067939-addd82d6-a256-4e17-90b8-e2a5f379e2ad.png">
 
 - [x] Caso o usuário digite letra, espaço ou enter, a mensagem que aparece é a seguinte:
 
 
  <img width="449" alt="erro" src="https://user-images.githubusercontent.com/98350733/214068338-144a99f4-8eaf-4b58-978a-afb4f221f7a8.png">
  
  
 - [x] Escolhendo a opção número 1, cadastra-se o usuário:
 
 
  <img width="515" alt="cadastroUsuario" src="https://user-images.githubusercontent.com/98350733/214069069-ce3d463c-1b14-489f-99af-78d808dad4f5.png">
  
  
 - [x] Finalizando o cadastro do usuário, o programa questiona se quer continuar ou não. No exemplo abaixo, o responsável cadastra apenas um usuário e responde não ao questionamento, fazendo com que a interface volte ao menu inicial:


  <img width="539" alt="cadastroTeste" src="https://user-images.githubusercontent.com/98350733/214069896-0ecfd77f-3308-4298-82d6-0b8aa4347364.png">
  
  
- [x] O mesmo acontece com o restante dos cadastros;     
     

- [x] No exemplo abaixo, o responsável vizualiza os cadastros usuários registrados no banco de dados, escolhendo a opção 5:


 <img width="416" alt="vizualizaUsuario" src="https://user-images.githubusercontent.com/98350733/214071431-efffdbfb-d361-4123-a362-bc032181b3af.png">
 <img width="451" alt="vizualizaTeste" src="https://user-images.githubusercontent.com/98350733/214071478-c9df7680-8882-4b85-8732-c06207c9476f.png">
 
 
- [x] Por fim, o programa exibe a lista do que foi cadastrado e abaixo apresenta o menu. No exemplo, o responsável escolhe a opção 9 que finaliza o programa:


 <img width="439" alt="fimPrograma" src="https://user-images.githubusercontent.com/98350733/214072394-ba451add-7709-4a28-ad8d-210605dd9e55.png">
