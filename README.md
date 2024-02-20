<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="60px" src="https://hermes.dio.me/lab_projects/badges/87d332d0-5198-4a2f-b159-38c8c2976954.png"></a>
    <span> Trabalhando com Machine Learning</span>
</h1>

## Criando modelo de previsão - Passo a passo

Para trabalhar no machine learn é essencial que você possua um workspace e esta é a tarefa inicial, criar o seu workspace para assim poder criar o seu trabalho automatizado.

Depois que nosso worlspace estiver pronto temos que entrar no ML studio para criar um "novo trabalho de ML automatizado", seguindo o passo a passo da documentação do Learning para melhor entendimento e para que tudo dê certo:
![image](https://github.com/MateusCantanhede/TrabalhandoComMachineLearning/assets/19481162/ba9138f6-f2fb-48c3-9b3e-9793406b7e1f)
 

...

## Vamos criar um aprendizado de maquina para a previsão de aluguel de bicicletas:
![image](https://github.com/MateusCantanhede/TrabalhandoComMachineLearning/assets/19481162/114afee4-210f-4be0-a2b8-7ffa65aaaaf1)
 

O tipo de tarefa é regressão e onome de ativo de dados e aluguel de bicicletas, com fonte de dados da WEB.
![image](https://github.com/MateusCantanhede/TrabalhandoComMachineLearning/assets/19481162/3004ca33-c0c5-4490-a986-aeb1f4ff92c0)
 
...

Adocumentação do Learning é bem didática e traz todos os valores e configurações para que o trabalho automatizado seja criado:

![image](https://github.com/MateusCantanhede/TrabalhandoComMachineLearning/assets/19481162/c9f29563-bfbb-49b7-af54-d2aedb98b868)

![image](https://github.com/MateusCantanhede/TrabalhandoComMachineLearning/assets/19481162/ba29c7df-84ae-4b37-94a3-21c08799bb24)


![image](https://github.com/MateusCantanhede/TrabalhandoComMachineLearning/assets/19481162/0946049c-e7dd-4211-8a55-e4838671bb52)

...

Chegando na opção "examinar" basta enviar o seu trabalho de treinamento:
<img align="right" src="https://raw.githubusercontent.com/alexklenio/DIO-Microsoft-Azure-AI-Fundamentals/main/imagens/DP01%20-%20Machine%20Learning/14.png" width=""/> 

...

Após envio seu trabalho irá passar pelo processo de configuração das execuções e após 15 min mais ou menos, podendo o tempo ser menor, ou maior, estará concluído:
![image](https://github.com/MateusCantanhede/TrabalhandoComMachineLearning/assets/19481162/8f7691ff-5092-4efb-8aca-70aac39f536d)


<img align="right" src="https://raw.githubusercontent.com/alexklenio/DIO-Microsoft-Azure-AI-Fundamentals/main/imagens/DP01%20-%20Machine%20Learning/16.png" width=""/> 

...

Pipeline com as etapas do processo de aprendizado e os testes realizados
![image](https://github.com/MateusCantanhede/TrabalhandoComMachineLearning/assets/19481162/08d77298-afeb-44a9-88db-6f00b66c52ea)


## Teste do modelo

Na página do modelo, cliquei na aba "Pontos de extremidade". Também é possível acessar pelo menu lateral em "Pontos de extremidade". Cliquei no ponto correspondente ao modelo gerado. Em seguida, acessei a aba "Testar".

Para o teste, utilizei o json abaixo:

``` JASON
{
  "input_data": {
    "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]
  }
}
```

A previsão gerada foi: 351.95

![image](https://github.com/MateusCantanhede/TrabalhandoComMachineLearning/assets/19481162/b19159ee-6b9a-4fa8-ae33-17d8745b51dd)

