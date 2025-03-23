# Microsservice User 

### Reference Documentation

* [Objetivos](#Objetivos)

* [Grooming](#Grooming)

* [Sistema](#Sistema)

* [Ações](#Ações)

* [Cenarios](#Cenarios)

* [Banco de Dados](#BancoDeDados)

* [Estrutura de Packages ](#Estrutura de Packages)


## Objetivos

Abordar os conteudos : Ecossistema Spring, Java ,  MVC e outros Design Pattern's na prática.

## Grooming

Criar Usuario salvando no PostgreSQl e enviando Email para usuario. 





##### Sistema

                    Microservice User

    Linguagem                  Java 18

    Dependencia                Maven 

    Banco de Dados             PostgreSQL
    
    BROKER                     Rabbit MQ , Cloud AMQP 

    Envio de Email             SMTP Gmail    

    Teste                      Postman             
    

#### Ecossistema Spring 
    
    Servidor                 Spring Boot , Spring Web 

    Banco de dados           Spring Data 

    Autenticação             Spring Validation 

    Mensageria               Spring AMQP

    Envio Email              Spring MAIL                




###### Ações

    
    Criar usuario no Postman           

    POST
    
    Url = http://localhost:8081/users

    Body =
        {
          "name": "Layon Carvalho",
          "email": "layon.silveira@gmail.com"
        }

###### Cenarios

      1. Criar usuario na base PostgreSQL;
      2. Enviar Email com mensagem;  


#### Banco de Dados


        Create database user;			
			--DROP DATABASE user;
    
        CREATE TABLE TB_User(
        user_id PRIMARY KEY,
        name string,
        email string ) 

#### Estrutura de Packages
        
        controllers: 
            UserController 
        
        dtos:
            UserRecordDto
        
        models:
            UserModel

        repositories: 
            UserRepository

        services: 
            UserService 
    



 