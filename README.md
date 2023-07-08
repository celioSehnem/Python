# Leitura de dados metereológicos 

Este trabalho visa explorar com o Python, um arquivo .csv que contém dados meterológicos. 

O arquivo contém informações climáticas diárias do município brasileiro de Porto Alegre, entre os anos 1961 e 2016. O arquivo contém 18.564 registros com os campos: data, precipitação (volume de chuva em milímetros por m²), temperatura máxima (em graus celsius), temperatura mínima (em graus celsius), horas insol, temperatura média (em graus celsius), umidade relativa do ar (% entre 0 e 100) e a velocidade do vento (em m/s). 

Com base nesse conjunto de dados, criei um programa que realiza as seguintes operações:

### 1) Carregamento dos dados em uma variável + transformação dos dados + correção de dados incorretos: 
Criei uma função para a leitura de dados, visto que teria de abrir o arquivo em diversos momentos do programa. A função, por meio do append, salva todos os dados .csv em uma lista, além disso, como originalmente todos estavam em formato de texto, transformei todos os dados em float, com excessão da coluna data, que transfomei em formato de data. Além disso, exclui os número negativos e acima de 100 no campo de precipitação.

### 2) Visualização dos dados carregados do arquivo por meio de inputs do usuário:
O usuário deve informar o período que quer ver, ou seja, deve indicar o mês e ano iniciais, bem como o mês e ano finais que deseja visualizar os dados. Permita também que o usuário informe se quer ver 1) todos os dados, 2) apenas os de precipitação, 3) apenas os de temperatura, ou 4) apenas os de umidade e vento para o período informado. Todos os inputs realizados pelo usuário passaram por uma validação.

### 3) Visualização do dia com maior precipitação

### 4) Média da temperatura mínima de um determinado mês (auge do inverno) nos últimos 11 anos do conjunto de dados (2006 a 2016) + gráfico com as médias do mês selecionado durante esses 11 anos: 
O programa escreve a média da temperatura mínima de um mês informado pelo usuário e a média geral da temperatura mínima para todo o período (11 anos). Ou seja, se o mês informado for 8, o programa exibi a temperatura mínima média do mês de agosto de cada ano (agosto/2006, agosto/2007, ...agosto/2016) e por fim apresenta a média deste período. Por fim o programa exibe um gráfico com as médias do mês selecionado durante 2006 até 2016.
