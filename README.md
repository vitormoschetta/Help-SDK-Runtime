# Help-SDK-Runtime

## SDK
O Kit de Desenvolvimento de Software (SDK) é tudo o que é necessário para o desenvolvimento de um app .NET Core.   
Ele disponibiliza um CLI para criar, compilar, executar e publicar aplicações.  
Página oficial de download:  

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

![alt text](images/02.png?raw=true=250x250 "Title") 


Esta ferramenta possui o _Runtime_ apropriado para executar a aplicação através do IIS.

<br>
<br>

## Aplicação Auto-contida
Existe a opção de publicar uma aplicação .NET Core para um SO específico que já inclui o _Runtime_. Ou seja, não é necessário instalar o _Runtime_ separado no _Server_.

Abaixo listamos alguns comandos:  

###### Publicação padrão (depende de instalação separada do _Runtime_ no Server):
```
dotnet publish
```


###### Publicação Auto-contida:
```
dotnet publish --runtime win10-x64 --self-contained true
```

No comando acima especificamos  o _identificador de tempo de execução_(RID), ou seja, que nossa aplicação deverá rodar em um Servidor Windows 10 com processador X64, e que deve incluir o _Runtime_.

No link abaixo podemos obter a lista de comandos para outras arquiteturas e SOs (Windows, Mac e Linux):

<https://docs.microsoft.com/pt-br/dotnet/core/rid-catalog>
