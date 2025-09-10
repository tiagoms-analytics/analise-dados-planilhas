# Google Sheet
# Análise_De_Dados_Exercício

O exercício propõe uma série de manipulações e análises em uma planilha do Google Sheets com os seguintes requisitos:

### 1. Análise de Dados

1. Normalize os dados da coluna “preco” na página “mercado_acoes”.

2. Crie 2 visualizações de filtro: Filtrar operações de compra e Filtrar operações de venda.


### 2. Página: 'cliente'

1. Na página “cliente”, onde o usuário irá digitar o código do cliente, irá mostrar o nome e email dele.


### 3. Página: 'estatística'

1. Na página “estatística”, acrescente as operações de variância e desvio padrão em relação ao preço.


### 4. Página 'tendencia_temporal'

1. Crie uma nova aba chamada **tendencia_temporal**.

2. Faça a previsão da quantidade de operações do mês 12, considerando o intervalo de valores do mês 1 ao mês 11. Ao lado, subtraia o valor da previsão - o valor real do mês 12 para saber o erro da sua previsão com o valor real.



## Fórmulas Utilizadas

  
  #### Página cliente
  
Comandos para onde o usuário irá digitar o código do cliente, irá mostrar o nome e email dele.
  - =PROCV(B2;mercado_acoes!A:C;2) =PROCV(B2;mercado_acoes!A:C;3)
  - =PROCV(B2;mercado_acoes!A:C;3)
  
  #### Página estatística
  
  Comandos para a Variância e o Desvio Padrão.
   - ==VAR(mercado_acoes!F:F)
   - DESVPAD(mercado_acoes!F:F)

   #### Página tendencia_tempora

Comando para a previsão da quantidade de operações do mês 12, considerando o intervalo de valores do mês 1 ao mês 11. Depois subtraia o valor da previsão - o valor real do mês 12 para saber o erro da sua previsão com o valor real.
  - =PREVISÃO(A13;B2:B12;A2:A12)
  - =C13-B13
   
    
        
