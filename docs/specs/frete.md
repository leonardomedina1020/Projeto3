RF-01: WHEN o usuário calcular o frete e o carrinho atingir o limite regional, THE SYSTEM SHALL zerar o frete.

RB-01: WHILE a região for 'Norte', o limite é R$ 300,00. Demais regiões: R$ 200,00.

RB-02: IF valor <= 0, THEN exibir erro 'Valor de carrinho inválido'.

RF-01: WHEN o usuário requisitar o valor do frete, THE SYSTEM SHALL apresentar o valor.

RB-03: IF a região informada for inválida, THE SYSTEM SHALL exibir 'Região inválida'.

RB-04: WHILE a região de destino for "Norte", THE SYSTEM SHALL aplicar a tarifa correspondente à região norte.

