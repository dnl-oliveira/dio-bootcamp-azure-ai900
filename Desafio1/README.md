# Bootcamp Microsoft Azure AI Fundamentals - AI900

# Criando um Modelo de Previsão no Azure

Desafio de projeto do modulo de Introdução ao Aprendizado de Máquina - Trabalhando com Machine Learning na Prática no Azure ML.

## Pré-requisitos

- Uma conta do Microsoft Azure
- Conhecimentos básicos sobre machine learning e Azure

## Passo 1: Configuração do Ambiente

1. Acesse o portal do Azure em [portal.azure.com](https://portal.azure.com).
2. Faça login com suas credenciais do Azure.
3. Dentro do portal azure, clique em Criar Recurso
4. Na tela aberta utilize a barra de pesquisa e digite Azure Machine Learning, no recurso clique no botão criar
5. Preencha os dados solicitados na tela como Grupo de recursos, nome, região, após preencher clique em criar e aguade o termino do deploy.
6. Quando terminar acesse a pagina do recurso, nessa página terá um botão para Ir para o estudio.

## Passo 2: Configurando Modelos e Conjunto de Dados

1. No [Azure Machine Learning Studio](https://ml.azure.com/?azure-portal=true), acesse a página ML automatizado
2. Crie um novo trabalho de ML automatizado com as seguintes configurações, usando Next para avançar pela interface do usuário

### Configurações básicas:

**Nome do trabalho**: mslearn-bike-automl
**Novo nome do experimento**: mslearn-bike-rental
**Descrição** : Aprendizado de máquina automatizado para previsão de aluguel de bicicletas
**Marcadores** : nenhum

### Tipo de tarefa e dados:

* Selecione o tipo de tarefa : Regressão
* Selecionar conjunto de dados : crie um novo conjunto de dados com as seguintes configurações:
    * Tipo de dados :
    * Nome : aluguel de bicicletas
    * Descrição : dados históricos de aluguel de bicicletas
    * Tipo : Tabular
* Fonte de dados :
    * Selecione Dos arquivos da web
* URL da Web :
    * URL da Web :https://aka.ms/bike-rentals
    * Ignorar validação de dados : não selecionar
* Configurações :
    * Formato de arquivo : Delimitado
    * Delimitador : Vírgula
    * Codificação : UTF-8
    * Cabeçalhos de coluna : apenas o primeiro arquivo possui cabeçalhos
    * Pular linhas : Nenhum
    * O conjunto de dados contém dados multilinhas : não selecione
* Esquema :
    * Incluir todas as colunas exceto Caminho
    * Revise os tipos detectados automaticamente

3. Clique em criar, quando a criação for concluida, selecione o conjunto de dados de aluguel de bicicletas para continuar a enviar o trabalho de ML automatizado

## Passo 3: Criando o Modelo de Previsão

1. Siga as etapas detalhadas na documentação para criar um modelo de previsão no Azure.
2. Certifique-se de entender os conceitos apresentados durante o processo.

## Passo 4: Avaliação e Implantação do Modelo

1. Após criar o modelo, avalie sua eficácia usando conjuntos de dados de teste.
2. Se necessário, ajuste e refine o modelo para obter melhores resultados.
3. Depois de satisfeito com o desempenho do modelo, proceda para implantá-lo em produção.

## Passo 5: Monitoramento e Manutenção

1. Uma vez implantado, monitore regularmente o desempenho do modelo.
2. Faça ajustes conforme necessário para garantir que o modelo permaneça preciso e eficiente.
3. Mantenha-se atualizado com as práticas recomendadas de machine learning e Azure para garantir a segurança e confiabilidade do seu modelo.

## Conclusão

Passo a passo baseado no lab [Explore o Machine Learning Automatizado no Azure Machine Learning](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)

Para mais informações e recursos adicionais, consulte a documentação oficial do Azure e a plataforma de aprendizado da Microsoft.