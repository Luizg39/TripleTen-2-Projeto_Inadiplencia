# TripleTen-2-Projeto_Inadiplencia

## Análise do risco de inadimplência dos mutuários

Seu projeto é preparar um relatório para a divisão de empréstimos de um banco. Você precisará descobrir se o estado civil de um cliente e o número de filhos têm impacto sobre se ele deixará de pagar um empréstimo. O banco já tem alguns dados sobre a capacidade de crédito dos clientes.

Seu relatório será considerado ao criar uma pontuação de crédito de um cliente em potencial. A contagem de crédito é usada para avaliar a capacidade de um devedor em potencial de pagar seu empréstimo.

Primeiramente, os dados serão avaliados a procurá de dados ausentes, problemas nas colunas, dados com problemas, dados com o tipo errado, dados duplicados e ausentes. Depois de identificados os problemas, eles serão corrigidos para que a as hipóteses sejam testadas.

Com a tabela pronta para a ánalise serão feitas as perguntas:

    Existe alguma relação entre ter filhos e pagar um empréstimo em dia?
    Existe alguma relação entre o estado civil e o pagamento de um empréstimo no prazo estipulado?
    Existe uma relação entre o nível de renda e o pagamento de um empréstimo no prazo?
    Como as diferentes finalidades do empréstimo afetam o pagamento pontual do empréstimo?


## Conclusão Geral

Inicialmento houve a exploração dos dados, com o objetivo de identificar dados incorretos, ausentes ou disprepantes. Foram identifacados que as colunas days_employed, education e total_income precisavam de correção.

Em relação aos valores ausentes, 2174 observações possuiam valores ausentes representando 10% do dataframe. Não foi identificada uma razão para os valores ausentes. Foi decidido preencher os valores ausentes. Para a correção dos valores negativos foi usado o módulo. Para os valores discrepantes, foram divididos para ficarem na ordem de grandeza dos outros valores. Em relação aos dados duplicados ou incorretos, foram 73 linhas, uma variação de 0,3%.

Foi criado a coluna age_index para categorizar os dados da coluna dob_years. Para categorizar a coluna total_income foi criada a coluna categ_income e para a coluna purpose foi criado a coluna categ_income.

As conclusões em relação as perguntas foram :

Existe uma correlação entre a quantidade de filhos e do pagamento em dia?

    Existe correlação entre ter filhos ou não e o pagamento em dia. O números de filhos não é relevante a taxa de inadimplência

Existe uma correlação entre o status familiar e o pagamento em dia?

    Os indivíduos que nunca foram casados possuem uma propensão maior a inadimplência, entre 9,3 a 9,7%. Os indivíduos que já foram casados possuem uma tendência menor, entre 6,5% e 7,5%.

Existe uma correlação entre o nível de renda e o pagamento em dia?

    O nível de renda não possui uma variação da taxa de inadimplência muito relevante entre elas, com as categorias classe média alta e pobre tendo o mesmo nível de inadimplência.

Como a finalidade do crédito afeta a taxa de inadimplência?

    Os empréstimos com finalidade imobiliária possuem a menor taxa de inadimplência, seguido pelo casamento. Os empréstimos para aquisição de educação superior e carro possuem as maiores taxas de inadimplências.

