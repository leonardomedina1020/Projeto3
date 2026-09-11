# Especificação: Sistema de Cálculo de Frete

## Requisitos Funcionais

- **RF-01 (Event-Driven):** WHEN o usuário calcular o frete e o carrinho atingir o limite regional, THE SYSTEM SHALL zerar o frete.

- **RF-02 (Event-Driven):** WHEN o usuário requisitar o valor do frete, THE SYSTEM SHALL apresentar o valor.

## Regras de Negócio e Exceções

- **RB-01 (State-Driven):** WHILE a região for "Norte", THE SYSTEM SHALL considerar R$ 300,00 como valor limite. Para as demais regiões, o limite é R$ 200,00.

- **RB-02 (Unwanted Behavior):** IF o valor for menor ou igual a R$ 0,00, THEN THE SYSTEM SHALL exibir a mensagem de erro "Valor de carrinho inválido".

- **RB-03 (Unwanted Behavior):** IF a região informada for inválida, THE SYSTEM SHALL exibir a mensagem de erro "Região inválida".

- **RB-04 (State-Driven):** WHILE a região de destino for "Norte", THE SYSTEM SHALL aplicar a tarifa correspondente à região norte.
