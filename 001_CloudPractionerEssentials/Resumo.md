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