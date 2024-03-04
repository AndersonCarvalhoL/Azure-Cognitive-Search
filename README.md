<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="60px" src="https://hermes.dio.me/lab_projects/badges/619af8f8-d138-4e40-9d48-fec7b318e44d.png"></a>
    <span> 
Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados</span>
</h1>

## Documentação
Material original em inglês:
[Documentação](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)

## Passo 1: Criando recurso do Asure AI Search:     

<img src="img/01.png" width=""/> ...  

## Passo 2: Criando recurso do Azure AI services:      

<img src="img/02.png" width=""/> ... 

## Passo 3: Criando o storage:      

<img src="img/03.png" width=""/> ... 
<img src="img/04.png" width=""/> ... 

## Passo 3: Permitindo acesso anônimo ao Blob:      

Como nosso laboratório é apenas didático,para aprender os princípios da inteligência artificial com o Azure, precisamos permitir o acesso anônimo ao blob para simplificar e facilitar nossas implementações, Após criar o seu Storage, entre no mesmo e navegue até a guia SETTINGS > CONFIGURATION seguindo os passos abaixo:

<img src="img/05.png" width=""/> ... 


## Passo 5: Criando o Container:      

Navegue até a guia DATA STORAGE > CONTAINERS, para criar o contanier dentro do storage e adicionar as pesquisas que seram analisadas pelo AI SERVICE.

<img src="img/06.png" width=""/> ...   
<img src="img/07.png" width=""/> ...  

## Passo 6: Importação e indexação dados para o AI SEARCH:      

Neste ponto você precisa linkar / importar os dados que você inseriu e configurou no seu STORAGE, volte para o AI SEARCH e siga os passos abaixo:

<img src="img/08.png"" width=""/> ... 

Esta é a parte mais importante de todo o processo, assim como o bootcamp fala são muitos passos que que você precisa seguir a risca, achei apenas uma diferença da documentação oficial para o que achei quando configurei o meu.

Ao seguir a [Documentação](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html) você chegará em INDEX DOCUMETS, o qual o gif acima mostra o início do processo, siga os topicos até chegar na sessão 4:

<img src="img/09.png" width=""/> ... 

**4. In the Attach Cognitive Services section, select your Azure AI services resource.**

Note que a instrução manda que selecionemos o recurso AI SERVICE configurado, porém não mostrou nenhum, apenas uma informação dizendo que meu acesso era gratúito e que as configurações são limitadas, não se preocupe e pode passar para o passo 5 . In the Add enrichments section.

Siga todas as configurações terminando no passo 7 . Select the indexer name to see more details.

## Passo 7: Cnsultando o índice:      

Feitas todas as configurações vamos voltar ao AZURE AI SERVICES, entrar no nosso serviço e através do SEARCH EXPLORER testar se tudo foi indexado e se a consulta esta funcionando, utilizando os comandos:

<img src="img/10.png" width=""/> ... 

```
search=*&$count=true    (  verifica se a indexação esta funcionando e mostra os documentos )
```
<img src="img/11.png" width=""/> ... 

```
search=locations:'Chicago' ( Consulta as ocorrencias acontecidas em Chicado )
```
<img src="img/12.png" width=""/> ... 

```
search=sentiment:'negative' ( Consulta as ocorrencias com sentimento negativo )
```
<img src="img/13.png" width=""/> ... 


## Observações finais:      

As ferramentas de inteligência artificial do Azure tornam mais fácil encontrar informações em documentos, pesquisas e depoimentos, agilizando a avaliação da satisfação das empresas com seus produtos e serviços.