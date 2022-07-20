# Projeto Final - Bootcamp de Engenharia de Dados How-Bootcamps:
# Previsão de Preço de Moedas e Criptomoedas

## Sobre:
Este repositório tem como finalidade armazenar o projeto final do bootcamp de engenharia de dados da How Bootcamps e auxiliar no versionamento e desenvolvimento do mesmo. No caso, após os diversos conhecimentos adquiridos e aprimorados durante o Bootcamp, tanto relacionados à Engenharia de Dados, tanto relacionados a computação em nuvem (AWS), foi nos dado o desafio de criar um projeto final que envolvesse as tecnologias mostradas durante a trajetória.

## Objetivos:
O objetivo deste projeto é criar um sistema completo em nuvem para previsão do valor de moedas e criptomoedas utilizando técnicas de Aprendizado de Máquina e de Aprendizado Profundo. Além do meu interesse pela área de mercado financeiro, no geral, o objetivo principal desse projeto é aplicar técnicas de alto nível para criação de um modelo que consiga prever os valores das moedas em diferentes intervalos de tempo: diário, semanal e mensal. Dessa forma, o sistema conseguiria gerar um grande valor para o usuário, visto que o mesmo conseguiria ter, pelo menos, uma estimativa do quanto uma moeda se valorizaria ou desvalorizaria, evitando prejuízos e auxiliando-o.

## Métodos utilizados:
<!--ts-->
* Inicialmente, foram mapeados os possíveis projetos que poderiam ser realizados (Brain Storm). Porém, como as outras opções não eram uma aplicação com um uso real, a opção de criar um modelo para realizar predições de preços de criptomoedas prevaleceu.

* Após a escolha do tema, foram mapeados os serviços e ferramentas que seriam utilizadas. No caso, a arquitetura montada e os serviços escolhados serão explicados com mais detalhes na próxima seção.

* Realizar testes utilizando uma API para obter os valores sobre as moedas, visto que esses dados serão ingeridos na nuvem para realizar o treinamento dos modelos.

<!--te-->

## Ferramentas utilizadas:

<!--ts-->
* Amazon S3: Armazenamento dos dados extraídos da API em formato .json.

* Amazon Kinesis: Realizar a ingestão dos dados a todo momento, com um curto período de intervalo entre cada ingestão.

* Amazon SQS: Integração da API e do S3 por meio de filas.

* Amazon Glue: Integração de Dados entre S3 e Athena.

* Amazon Athena: Queries nos dados armazenados no S3.

* Amazon Sagemaker: Treinamento de modelo e deploy de endpoint para realizar inferência.
<!--te-->

## Arquitetura:

