# Help-SDK-Runtime

## SDK
Tudo o que é necessário para o desenvolvimento de um app .NET Core.   
Disponibiliza um CLI para criar, compilar, executar e publicar aplicações.

<br>
<br>

![alt text](images/00.png?raw=true=250x250 "Title")  

<https://dotnet.microsoft.com/download>

<br>
<br>

## Runtime 
É o Tempo de Execução, como uma 'Máquina Virtual' que executa os arquivos _.dll_ publicados pelo SDK.  

###### Importante: O SDK já possui seu próprio _Runtime_ para ser utilizado com CLI durante o desenvolvimento.

Ao **hospedar/implantar** o app, tudo o que precisamos para executar a aplicação é o _Runtime_. 

Para implantar uma aplicação usando o IIS por exemplo, instalamos uma outra ferramenta chamada _Hosting Bundle_ (Pacote de Hospedagem):

![alt text](images/01.png?raw=true=250x250 "Title")  


Esta ferramenta possui o _Runtime_ apropriado para executar a aplicação através do IIS.
