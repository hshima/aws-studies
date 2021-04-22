# Modulo 1 - Introdução ao Amazon Web Services
## Objetivos
1. Listar os benefícios da AWS
2. Descrever as diferenças entre serviços de entrega sob demanda (on-demand services) e desenvolvimento em nuvem (cloud deployment)
3. Listar o modelo de precificação pré-paga

___

## Introdução ao modelo modelo cliente-servidor (client-server)
Para prover as solicitações de terminais, é solicitado a um servidor que determinada mensagem/tarefa seja realizada ao requisitante, uma vez que a requisição seja válida.

```text
Analogia: 

Ao realizar um pedido a um balconista, o cliente informa o que quer pedir (requisição) e paga (critério de validação).
O atendente (servidor), verifica se o valor recebido está certo (servidor valida a requisição) e emite a ordem de preparo/compra e, quando disponível, a entrega ao cliente ou a quem ele determinar (retorno da requisição).
```

Para realizar os serviços de servidor, o serviço Amazon Elastic Computing Cloud (Amazon EC2) disponibiliza uma instância de servidor virtual.

### Conceito chave: Pagar apenas pelo que se usa
Entretanto, a visão de cliente-servidor é muito limitada pois não compreende a complexidade dos serviços que podem utilizados, como pagar apenas pelo tempo de serviço que está sendo usado de fato, como em um custo fixo.
```text
Analogia:

Pensando em um empregado que contrata um serviço de entrega de comida por aplicativo, não faz sentido pagar pelo mês inteiro (CLT) ou mesmo por dia quando a demanda varia durante o mês.
Um serviço por aplicativo funciona sob demanda, cobrando por transação.
```
Os servidores on-premisses fixam os custos de servidores comprometendo o potencional de margem. A Amazon formata os serviços para que cada recurso seja acionado de acordo com a necessidade do negócio, aumentando ou reduzindo a quantidade de recursos.

## Cloud Computing
Computação em nuvem é o serviço de entrega ou devolução de recursos computacionais sob demanda pela internet, com precificação pre-paga.

Essa característica é a diferenciação que a AWS provê ao seu negócio, pois o "trabalho duro" (heavy lifting) de disponibilização de recursos passam a ser responsabilidade da Amazon, ajustando a estrutura para permitir que os recursos computacionais sejam entregues conforme a necessidade sem necessidade de adições contratuais e condições intrincadas.

### Modelos de desenvolvimento (deployment) para computação em nuvem
Ao contratar os recursos computacionais, é importante considerar os fatores de negócio para a escolha da precificação adequada dos recursos.
A AWS disponibiliza três modelos de nuvem:
- Cloud-based deployment
  - A aplicação roda totalmente na nuvem
  - Migração de aplicações existentes para a nuvem
  - Desenvolva e entregue uma nova aplicação na nuvem
- On-premisses deployment - também conhecida como *private cloud* 
  - Posicionar recursos usando virtualização e ferramentas de gestão de recursos
  - Aumentar o aproveitamento de recursos através de gestão de da aplicação e tecnologias de virtualização
- Hybrid deployment
  - Conecte recursos de nuvem a infra-estrutura on-premises
  - Integre recursos de nuvem com aplicações legadas

## Benefícios da computação em nuvem
- Substitua custos fixos por custos variáveis

    Remova a necessidade de planejamento para investir em hardware, espaço e contratos de data-centeres.

    A definição de custo variável significa que se pagará apenas pelo que consumir.

    Substituindo investimentos pesados por recursos após utiliza-los, passa o custo apenas aos recursos que foram consumidos no período.
- Corte de custos em execução e manutenção de data centeres

    Remover a necessidade de manutenção e gestão de dispositivos e equipamentos, resultando no consumo de tempo e dinheiro.

    O investimento em nuvem permite focar menos em tais tarefas e mais nas aplicações e clientes.
- Pare de tentar adivinhar a capacidade a ser contratada
    
    Elimina a necessidade de adivinhar a capacidade necessária de infra estrutura antes de se iniciar uma aplicação. É possível iniciar quantas intâncias de serviços necessárias e devolvê-las assim que não forem mais necessárias.

- Beneficie-se da economia em escala

    Utilizando a computação em nuvem, é possível alcançar um custo variável mais baixo que você mesmo conseguiria por conta própria.
- Ganhe velocidade e agilidade

    A flexibilidade da nuvem permite que seja mais fácil desenvolver e entregar aplicações, em comparação com recursos de data-centers (precisam ser comprados, entregues, instalados, configurados, etc...).
- Atenda ao mundo todo em minutos

    A distribuição global da AWS permite que suas aplicações sejam entregues e alcançadas em todo o mundo com a menor latência.

# Módulo 2
## Objetivos
1. Descrever os benefícios dos níveis básicos da Amazon EC2
2. Identificar os diferentes tiops de instâncias EC2
3. Diferenciar entre as diversas opções de faturamento para Amazon EC2
4. Listar os benefícios da Amazon EC2 Auto Scaling
5. Listar os benefícios do Elastic Load Balancing
   1. Exemplificar casos de uso para o Elastic Load Balancing
6. Listar as diferenças entre o Amazon Simple Notification Service (Amazon SN) e Amazon Simple Queue Service (Amazon SQS)
7. Listar demais opções de computação AWS
___

### Amazon Elastic Compute Cloud (Amazon EC2)
Provê capacidade computacional redimensionável e segurana nuvem com Aamazon EC2

|Antes|Depois|
|---|---|
|Investimento financeiro em hardware e infraestrutura|Provisão e lançamento de reqursos em minutos|
|Espera até que a entrega seja realizada pelos fornecedores|Pare de usar quando tiver finalizado de rodar a carga de trabalho|
|Aguardar a instalação físca nos data-centers|Pague apenas por provisionamentos em uso, não quando parados ou finalizados|
|Configurar todos os equipamentos|Economize ao utilizar apenas a capacidade que precisa ou requer|
___
#### Lançamento de instância
Dispare uma instância. Comece por selecionar um template com configuração básica para sua instância.

Essas configurações incluem sistema operacional, servidor de aplicações ou aplicações. Também é possível configurações específicas de hardware para sua instância.

Configurações de segurança para controlar o tráfego de rede para seu serivodr também são especificadas nesse momento.
___
#### Conecte

Conecte-se à instância. É possível se conectar com a instância de diversas formas. Aplicações podem conectar de formas diversas e múltiplas. Usuários também podem acessar através de login e por outro terminal.

#### Use
Após conexão, é possível utilizar comandos como instalação de softwares, incrementar armazenamento, copias e oranizar arquivos e mais.

### Tipos de instâncias EC2
- Instâncias de uso genérico: Provê um equilíbrio de recursos entre recursos computacionais, memória e rede
  
  Podem ser usados como:
  - Servidores de aplicação
  - Servidores de jogos
  - Backend para aplicações de negócios
  - Pequenas e médias bases de dados
  - Etc...

- Instâncias otimizadas para computação (Compute optimized instances):

  Ideais para aplicações que desempenham bem processadores de alta performance. Assim como instâncias de propósitos genéricos, é possível utilizar para cargas de trabalho tais como web, aplicações e servidores de jogos.

  Entretanto, são ideais para servidores web de alta performance, servidores de aplicações de computação intensiva e servidores dedicados de jogos. Também é possível utilizar a Instâncias de computação otimizada para processar conjuntos de blocos de trabalho que requerem processamento de diversas transções em um mesmo grupo.

- Instâncias otimizadas para memória:

  São projetadas para entregas rápidas de cargas de trabalho que processem grandes datasets em memória.

  Instâncias otimizadas permitem a execução de cargas de trabalho que exigem altas necessidades de memória e performance.

- Instâncias de computação acelerada

  São instâncias que empregam aceleração de hardware, ou coprocessadores, para executar algumas funções de forma mais eficientemente que executadas em CPU (computação de pontos flutuantes, aceleração gráfica e pareamento de data patterns).

  São ideais para trabalhos como aplicações gráficas, streaming de jogos e aplicações de streaming.

- Instâncias otimizadas para armazenamento

  São projetadas para cargas de trabalhos que demandam altas taxas de leituras sequenciais e acessos de escrita para  grandes datasets em armazenamento local. Exemplos: file system distribuídos, aplicações de warehousing, sistemas OLTP (Online Transaction Processing) de alta frequência.

  Em computação, a medida de performance de um dispositivo de armazenamento é IOPS (Inpu/Outpu Per Second). Storage optimized instances são desenvolvidas para entregar dezenas de milhares de IOPS randomicamente distribuídos papra aplicações, em baixa latência.

## Amazon EC2 Pricing - precificação

- On-demand - Sob demanda

  Ideais para usos em trabalhoes de curtos períodos e irregulares que não podem ser interrompidos.

  Não há pagamento antecipado ou contrato pré requerido.

  O trabalho não é interrompido até que você encerre e será cobrado apenas pelo tempo de computação consumido.

  Não são recomendados para para cargas de trabalho que durem mais de um ano, pois é possível alcançar economias maiores com Reserved Instances.

- Amazon EC2 Savings Plans

  A AWS oferece Saving Plans (planos de economia) para diversos serviços computacionais, incluindo o EC2.

  Esses planos permitem reduzir o custo de computação ao contratos de 1 ou 3 anos, podendo alcançar economias de até 72%, em comparação com o plano on-demand.

  Após consumir a fraquia do Saving Plan, os custos passam a ser os mesmos do plano on-demand.

  Mais adiante, nesse curso, será visitada a ferramenta AWS Cost Explorer. Essa ferramenta permite visualizar, compreender e gerir seu custo e consumo na AWS no decorrer do tempo.
  
  Essa ferramenta permite analisar seu padrão de consumo Amazon EC2 em janelas de 7, 30 ou 60 dias. Também sugere recomendações customizadas para Savings plans. As recomendações estimam quanto poderia ser economizado em seu custo mensal de AWS EC2, com base no consumo prévio e comprometimento contratual de horas e um planejamento de 1 ou 3 anos.

- Reserved Instances - Instâncias Reservadas

  São descontos de faturamento aplicados ao uso de instâncias On-demand. É possível adquirir Standard Instances e Convertible Instances por período de 1 ou 3 anos e Scheduled Instances pelo período de 1 ano. As maiores economias estão nos planos de 3 anos.

  Ao final do período de uma Reserved Instance, é possível continuar utilizando os serviços sem interrupção, entretanto, o faturamento ocorrerá com base no plano On-demand até que uma das condições abaixo sejam confirmadas:
    - A instância seja finalizada (terminated)
    - Seja adquirida uma nova Resered Instance que coincida com os atributos da instância (Tipo de instância, região, tenancy - arrendamento e plataforma).

- Spot Instances

  São ideais para cargas de trabalho que sejam flexíveis quanto a períodos de execução ou que podem suportar interrupções.

  Esses recursos são instâncias EC2 ociosas, por isso, permitem descontos de até 90% em relação ao plano on-demand.

  Exemplo de uso: Existe a necessidade de processar em background uma tarefa secundária. Você requisita uma instância Spot. Se uma instância spot está disponível, a instância é disparada.

  Entretanto, se não existe uma instância EC2 disponível, a solicitação não será iniciada até que exista disponibilidade, podendo demorar algum tempo até que sua instância seja lançada.

  Após iniciada e em processamento, se a disponibilidade não estiver mais disponível ou a demanda por instâncias spot se elevar, sua instância pode ser interrompida.

- Host dedicado

  São servidores físicos com instâncias da disponibilidade Amazon EC2 dedicas exclusivamente ao seu uso.

  É possível utilizar licenças de software por Socket, por Core ou por VM para ajudar a manter compliance de licenças.

  É possível adquirir On-demand Dedicated Hosts e Reservations de Host Dedicado.

  De todas as opções de Amazon EC2 disponíveis, Hosts dedicados são as mais caras.

## Scaling Amazon EC2

