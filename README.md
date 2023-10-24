# Calculadora de Frete

Este é um programa em C# desenvolvido por Danilo Couto para calcular custos de frete com base no preço do pedido e no peso. Ele oferece quatro funções principais, cada uma com um propósito específico:

1. `calculateShippingPrice`: Calcula o custo de frete com base no preço do pedido.
2. `calculateShippingWeight`: Calcula o custo de frete com base no peso dos itens.
3. `calculateShipping`: Calcula o custo de frete final considerando tanto o preço do pedido quanto o peso, com um desconto para custos mais altos.
4. `calculateShippingFromArray`: Calcula o custo de frete final para um array de preços de itens e um array de pesos.

## Informações do Desenvolvedor

- **Desenvolvedor**: Danilo Couto
- **E-mail**: dansantos45@hotmail.com
- **LinkedIn**: [LinkedIn de Danilo Couto](https://www.linkedin.com/in/danilocoutopsantos/)

## Estrutura do Código

O código está organizado em uma classe chamada `ShippingCalculator` dentro do namespace `ShippingCalculator`. Ela contém quatro métodos para calcular diferentes aspectos dos custos de frete:

1. `calculateShippingPrice`: Calcula o custo de frete com base no preço do pedido.
2. `calculateShippingWeight`: Calcula o custo de frete com base no peso dos itens.
3. `calculateShipping`: Calcula o custo de frete final combinando o preço do pedido e o peso.
4. `calculateShippingFromArray`: Calcula o custo de frete final para arrays de preços de itens e pesos.

## Uso

Você pode utilizar este programa para calcular os custos de frete para os seus pedidos. Aqui está como você pode usar cada uma das funções fornecidas:

1. **`calculateShippingPrice`**

   ```csharp
   var calculadora = new ShippingCalculator();
   double precoPedido = 100.0; // Substitua pelo preço do pedido real
   double custoFrete = calculadora.calculateShippingPrice(precoPedido);
   ```

2. **`calculateShippingWeight`**

   ```csharp
   var calculadora = new ShippingCalculator();
   double peso = 3.0; // Substitua pelo peso real do item
   double custoPesoFrete = calculadora.calculateShippingWeight(peso);
   ```

3. **`calculateShipping`**

   ```csharp
   var calculadora = new ShippingCalculator();
   double precoPedido = 100.0; // Substitua pelo preço do pedido real
   double peso = 3.0; // Substitua pelo peso real do item
   double freteFinal = calculadora.calculateShipping(precoPedido, peso);
   ```

4. **`calculateShippingFromArray`**

   ```csharp
   var calculadora = new ShippingCalculator();
   double[] precosItens = { 40, 70, 140, 250 }; // Substitua pelos preços reais dos itens
   double[] pesosItens = { 1, 2, 5, 9 }; // Substitua pelos pesos reais dos itens
   double freteFinal = calculadora.calculateShippingFromArray(precosItens, pesosItens);
   ```

## Testes

O programa inclui um conjunto de testes unitários para garantir a correção dos cálculos de frete. Esses testes utilizam o framework de testes Xunit e abrangem diferentes aspectos dos cálculos de frete. Cada categoria de teste corresponde a uma função específica.

- **Categoria de Teste 1:** Testes para `calculateShippingPrice`
- **Categoria de Teste 2:** Testes para `calculateShippingWeight`
- **Categoria de Teste 3:** Testes para `calculateShipping`
- **Categoria de Teste 4:** Testes para `calculateShippingFromArray`

Você pode executar esses testes para verificar se os cálculos de frete do programa estão funcionando conforme o esperado.

Sinta-se à vontade para incorporar esta calculadora de frete em seus projetos em C# para lidar com cálculos de custos de frete de forma eficiente. Se encontrar algum problema ou precisar de mais assistência, entre em contato com o desenvolvedor Danilo Couto através do e-mail ou do perfil do LinkedIn fornecidos.
