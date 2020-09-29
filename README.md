# PlanetsJson
Só um lugar para guardar um arquivo de um jogo, no qual será lido em tempo de jogo para modificar
alguns comportamentos sem precisar gerar diferentes builds

obs: utilizar ponto no lugar de vírgula ao escrever números decimais

Explicação:

"zoomMin": é o valor minimo que o usuario pode dar zoomIn

"zoomMax": é o valor maximo que o usuario pode dar num zoomOut

"Sensibilidade": é o valor da sensibilidade do movimento de pinça (atualmente 0.01, esse número não deve ser muito grande, recomendo testes ao mexer nesta variável)

"constantPixel": É uma constante que Aumenta/Diminui a escala do mapa, multiplica as coordenadas x,y para afastar ou juntar os planetas em relação a tela.

PlanetsJsons: É o conjunto de planetas (não precisa mexer aqui)

"planet": É o nome do Planeta (A1, A2, ... , B12. Não temos tempo para mudar o nome dos planetas, pelo menos não nesse JSON format, exatamente, então manter padrão de A1, até B12, por favor.)

"Orbit": Número equivalente a orbita do planeta (que no caso talvez nem precise mexer, mas to colocando aqui)

"x": posição x do planeta (se necessário usar decimal)

"y": posição y do planeta (se necessário usar decimal)

"ep": chance de evento positivo do planeta (número entre 0 e 1)

"en": chance de evento negativo do planeta (número entre 0 e 1)

"n": chance de não acontecer evento (neutro) (número entre 0 e 1)
lembrar que as chances devem ser complementares, ep+en+n = 1.
