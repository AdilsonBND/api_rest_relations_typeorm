<h1> Api relations </h1>



<div>
  <img align="right" src="https://github.com/AdilsonBND/api_rest_relations_typeorm/blob/main/RELACIONAMENTOS_DB.png" width="45%"  />
</div>
 
* Api realizada para estudos com bancos de dados relacionais seguindo o esquema ao lado:
* A tabela room corresponde a sala de cursos tendo relacionamento 'um para muitos' com a tabela vídeos, dessa forma a tabela room pode receber varios vídeos mas cada vídeo participa apenas de uma sala, também possui relacionamento 'muitos para muitos' com a tabela Subjects que corresponde as matérias, dessa forma uma matéria pode pertencer a várias salas e um sala pode possuir várias matérias.
* A tabela room-subjects é ternária, existente apenas para estabelecer relacionamento entre as tabelas Room e Subjects.
 
### Instalação

* Após baixar o repositório certifique-se de que tenha dado permissões ao diretório .docker/entrypoints.sh e dentro da pasta do repositório rode o comando:
<pre> docker compose up</pre>

* Para testar as requisições POST e GET pode utilizar-se da extensão do VSCODE chamada "REST CLIENT", tendo no próprio repositório um arquivo de nome 'teste_requisicao.http' onde poderá realizar os teste.
