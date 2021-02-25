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
