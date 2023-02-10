# ExemploRabbitMQ
##Sistemas Distribuidos

## Executando o projeto

### Se quiser rodar o código do EMISSOR:
1- Abra o arquivo pom.xml
2- Altere o nome do arquivo que se encontra no <mainClass>
3- Salve
4- Execute o comando: 
    ```bash
    mvn compile assembly:single
    ```
5- Altere o nome do arquivo .jar. Ex: Emissor.jar
6- Execute o comando:
 ```bash
    java -jar target/Emissor5.jar
```
7- Cada vez que o código do emissor for rodado, vai ser emitida a mensagem informada no código


### Se quiser rodar o código do RECEPTOR:
1- Abra o arquivo pom.xml
2- Altere o nome do arquivo que se encontra no <mainClass>
3- Salve
4- Execute o comando: 
    ```bash
    mvn compile assembly:single
    ```
5- Altere o nome do arquivo .jar. Ex: Receptor.jar
6- Em uma aba diferente execute o comando:
 ```bash
    java -jar target/ReceptorEmissor.jar
```
7- Cada vez que o código do receptor for rodado, será aberto um terminal que ficará escutando o que está sendo enfileirado no RabbitMQ
