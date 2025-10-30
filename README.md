# AWS WorkFlows Step Function
☁️ AWS Bootcamp Code Girls 2025


## Objetivos ##
Este repositório tem como objetivo consolidar meus conhecimentos em workflows automatizados com AWS Step Functions e organizar anotações e insights adquiridos durante meu estudo e a prática.

## Step Function ##

O Step Functions é um serviço de fluxo de trabalho visual que ajuda os desenvolvedores a usar os produtos da AWS para desenvolver aplicações distribuídas, automatizar processos, orquestrar microsserviços e criar pipelines de dados e machine learning (ML).

O Step Functions é baseado em máquinas de estado e tarefas. No Step Functions, as máquinas de estado são chamadas de fluxos de trabalho, que são uma série de etapas orientadas a eventos. Cada etapa no fluxo de trabalho é chamada de estado. Por exemplo, um estado de tarefa representa uma unidade de trabalho que outro AWS serviço executa, como chamar outro AWS service (Serviço da AWS) ou API. As instâncias de fluxos de trabalho em andamento que executam tarefas são chamadas de execuções no Step Functions.

Obs: Não esquecer de usar a calculadora antes de começar qualquer projeto no Step Function.

**Casos de Uso** 

Automatize os processos de extração, transformação e carregamento (ETL) -
Garanta que diversos trabalhos de ETL de execução prolongada sejam executados em ordem e concluídos com êxito, sem a necessidade de orquestração manual.

Orquestre workloads paralelas de grande escala -
Repita e processe grandes conjuntos de dados, como logs de segurança, dados de transações ou arquivos de imagem e vídeo.

Orquestre microsserviços - 
Combine diversas funções do AWS Lambda em aplicações e microsserviços responsivos sem servidor.

Automatize funções de segurança e TI - 
Crie fluxos de trabalho automatizados, incluindo etapas de aprovação manual, como resposta a incidentes de segurança.

1. Realizando validações no Step Function
   
2. Criando e executando Lambda no Step Function

   

## Exemplo de Workflow ##

1. Workflow para Aprovação de Pedido de Compra

  
   <img src="./images/AWS WorkFlows Aprovação de Pedido de Compra.svg" width="600" />
   

## Dicionário ##

+ O que é validação?

  É o processo de garantir que os dados e decisões dentro de um fluxo de trabalho estejam corretos antes de avançar para a próxima etapa. Ela pode ocorrer de várias formas:

- Validação de entrada: Verifica se os dados recebidos estão completos e corretos.

- Validação condicional: Usa estados de decisão (Choice State) para direcionar o fluxo com base em regras.

- Validação de saída: Confere se os resultados de uma etapa estão no formato esperado.

- Validação com Lambda: Executa verificações mais complexas, como regras de negócio ou consultas externas.

- Validação estrutural: Usa ferramentas da AWS para verificar erros no design do fluxo antes da execução.

- Essa validação torna os workflows mais seguros, confiáveis e alinhados com os objetivos da aplicação.

  
+ O que é CloudFoundation?

É um conjunto de conceitos, práticas e treinamentos que ensinam os fundamentos da nuvem AWS.
Ajuda a step function com:

- Ensina como usar IAM para controlar acesso às máquinas de estado;
- Mostra como monitorar execuções com CloudWatch Logs e Metrics;
- Explica como conectar Lambda, DynamoDB, SNS, SQS e outros serviços;
- Ajuda a entender limites, custos e escalabilidade;
- Promove boas práticas de design de workflows desacoplados e resilientes;
  
Isso é importante para evitar erros como permissões mal configuradas (IAM), falta de visibilidade sobre falhas (sem CloudWatch), fluxos acoplados demais, difíceis de escalar ou manter, uso ieficiente de recursos, gerando custos desnecessários. Dessa forma é possível criar worflows robustos, seguros e otimizados com Step Function.

## Referências ##

https://aws.amazon.com/pt/step-functions/

https://medium.com/@as1987137/starting-aws-step-functions-dbe3ce456acc

https://docs.aws.amazon.com/pt_br/step-functions/latest/dg/welcome.html

https://calculator.aws/#/createCalculator/StepFunctions



