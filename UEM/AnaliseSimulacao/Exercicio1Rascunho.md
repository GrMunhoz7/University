model - ela acabou criando pq n dava p usar o vrtherm
pode ter 3 models
ou 1 model com todas as informações
flowsheet chama os models
outer(vem de fora) NComp (numero de elementos)
## parametros aqui(?)
## Flowsheet
### device
reator as reatormodelo
### SET 
vai colocar alguns valores aqui
area da base do reator
aqui onde fica os valores dos parametros
### especify
altura que fica variando
acho q é onde ficar as variaveis
### Initial
precisa de condições iniciais quando t=0 para conseguir diminuir a ordem de liberdade la
### Equations
balanço de massa global 
balanço molar de A
balanço molar de B
balanço de energia (?)
sla mais oq se precisar
### options
timestep = 0.1
timeend = 500
timeunit = 's'
## optmization
