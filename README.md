## Projeto de Imersão de Dados Alura

### Contexto
Utilizamos duas bases de dados para entender como os compostos reagem em determinadas células. Há dois tipos de tratamentos, aquele feito com o composto, no qual é utilizado alguma substância ou medicamento e o tratamento com controle que é feito sem a substância ou medicamento.
A primeira base de dados explorada possui os compostos e suas respectivas alterações nas células, na segunda base de dados temos quais foram os mecanismos ativados de acordo com o composto utilizado.

### Plano de Solução
- Passo 1 : Explorei as bases de dados com Pandas, Matplotlib e Seaborn.
- Passo 2 : Verifiquei os 5 compostos mais usados e suas reações.
- Passo 3 : Verifiquei se existe alguma relação dose x tempo.
- Passo 4 : Modelos de Machine Learning com Scikit-learn.

### Hipóteses Assumidas
- Durante o tratamento com controle (sem medicamento) o ideal é não haver células ativas.
- O tratamento feito com duas doses tende a ativar mais mecanismos das células do que aquele feito com uma dose.
- Quanto maior o tempo de efeito do composto, mais mecanismos foram ativados naquela célula.

### Top 5 Insights
- O tratamento com controle não obteve nenhum mecanismo ativado nas células.
- O primeiro composto mais usado 'cacb2b860' fazia parte do tratamento com controle, sendo assim não era um medicamento.
- O uso do segundo composto mais usado '87d714366' apresentou dois mecanismos ativados e o terceiro composto mais usado '9f80f3f77' apresentou um mecanismo ativado.
- Os mecanismos ativados pelo segundo composto foram diferentes do mecanismo ativado pelo terceiro composto.
- Tanto o segundo composto e o terceiro composto não demonstraram uma relação direta entre dose x tempo, portanto, a quantidade de doses tomadas e a quantidade de tempo de efeito do composto não interferiram na quantidade de mecanismos ativados em uma célula, um composto tende a ativar um ou mais mecanismos de células logo na primeira dose ou em 24 horas.

### Próximos Passos
- Analisar os dois últimos compostos mais usados do "Top 5 Compostos Mais Usados".
- Verificar se houve algum composto que ativou mais de 5 mecanismos.
- Treinar outros modelos de Machine Learning.
