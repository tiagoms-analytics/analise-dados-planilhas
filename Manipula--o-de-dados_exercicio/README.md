# Google Sheet
# Manipulação_De_Dados_Exercício

O exercício propõe uma série de manipulações e análises em uma planilha do Google Sheets com os seguintes requisitos:

### 1. Manipulação de Dados

1. Altere todos os tipos de dados de acordo com cada coluna.

2. Confira as estatísticas da coluna para conhecer mais os dados.


### Página: 'estatística'

1. Crie uma nova aba chamada **estatística**.

2. Na página de estatística, calcule as seguintes operações em relação ao preço: soma, mínimo, máximo, média, mediana e moda.

### 3. Página: 'mercado_acoes'

1. Crie três colunas novas: `dia`, `mês` e `ano`.
2. Extraia essas informações a partir da coluna `data`.

### 4. Página 'cliente'

1. Crie uma nova aba chamada **cliente**.

2. Na página de “cliente", deixe uma célula para digitar o e-mail do cliente e após digitar o e-mail de qualquer cliente em baixo irá aparecer 3 informações:

- A contagem de quantas operações de compra e venda do cliente fez

- A soma de quantas operações de compra e venda o cliente fez

- A mídia de quantas operações de compra e venda o cliente fez

3.  Na página de “cliente”, após digitar o e-mail de qualquer cliente ao lado, é preciso aparecer uma das mensagens abaixo, de acordo com as operações:

- Se o cliente fez mais de 20 operações, então mostre a mensagem “Perfil Agressivo”,

- Se fez entre 5 a 19 operações, então mostre a mensagem “Perfil Moderado”

- Se fez entre 0 e 4 operações “Perfil Conservador”


## Fórmulas Utilizadas

  
  #### Página estatística

  - SOMA(mercado_acoes!F:F)
  - =MÍNIMO(mercado_acoes!F:F)
  - =MÁXIMO(mercado_acoes!F:F)
  - =MÉDIA(mercado_acoes!F:F)
  - =MED(mercado_acoes!F:F)
  - =MODO(mercado_acoes!F:F)
 
  
  #### Página cliente

   - =SE(E2 < 5; "Perfil Conservador"; SE(E2 > 20; "Perfil Agressivo"; "Perfil Moderado"))
   - =CONT.SES(mercado_acoes!C:C; A2; mercado_acoes!D:D; "venda")
   - =CONT.SES(mercado_acoes!C:C; A2; mercado_acoes!D:D; "compra")
   - =SOMA(C2:D2)
   - =MÉDIA(C2:D2)
    
   ## Observações

   - Verifique que os nomes das abas estejam exatamente como nas fórmulas (mercado_acoes, estatística, cliente).
   - As fórmulas são dinâmicas e funcionam para listas com dados em expansão.
   - Lembre-se de configurar os formatos corretos de data para que as extrações de dia, mês e ano funcionem corretamente.
      
