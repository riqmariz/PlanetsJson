# PlanetsJson
Só um lugar para guardar um arquivo de um jogo, no qual será lido em tempo de jogo para modificar
alguns comportamentos sem precisar gerar diferentes builds

obs: utilizar ponto no lugar de vírgula ao escrever números decimais

Explicação:

"zoomMin": é o valor minimo que o usuario pode dar zoomIn

"zoomMax": é o valor maximo que o usuario pode dar num zoomOut

"Sensibilidade": é o valor da sensibilidade do movimento de pinça (quanto maior, mais rapido chega ao zoom máximo ao fazer o movimento) (atualmente 0.01, esse número não deve ser muito grande, recomendo testes ao mexer nesta variável)

"constantPixel": É uma constante que Aumenta/Diminui a escala do mapa, multiplica as coordenadas x,y para afastar ou juntar os planetas em relação a tela.

PlanetsJsons: É o conjunto de planetas (não precisa mexer aqui)

"id": É o identificador do planeta para poder carregar as informações. Planeta (A1, ...,A7,B1, ... , B12. manter padrão de A1, até B12, por favor. Usar CAPS)

"planetName": É o nome do planeta que aparecerá no jogo. Por exemplo, ao por "planetName":Zorgon. O planeta com o Identificador correspondente, na verdade, aparecerá como: Zorgon, apesar de por debaixo dos panos ser utilizado o identificador para referenciar o planeta.

"orbit": Número equivalente a orbita do planeta (que no caso talvez nem precise mexer, mas to colocando aqui)

"altura": é a altura da resolução do planeta, caso queira mudar o tamanho dos planetas. (atualmente é 180(altura)x180(largura))

"largura": é a largura da resolução do planeta, caso queira mudar o tamanho dos planetas. (atualmente é 180(altura)x180(largura))

"x": posição x do planeta (se necessário usar decimal)

"y": posição y do planeta (se necessário usar decimal)

"ep": chance de evento positivo do planeta (número entre 0 e 1)

"en": chance de evento negativo do planeta (número entre 0 e 1)

"n": chance de não acontecer evento (neutro) (número entre 0 e 1)
lembrar que as chances devem ser complementares, ep+en+n = 1.


Considerações:

Cálculo de distância em UA entre os planetas está sendo feito como a distância entre dois pontos arredondando para baixo (se é a distancia é igual é 4,7, então arredonda para 4,5, se é 4,3 arredonda para 4...)

Caso tenha dúvida se editou errado o JSON, Sempre modifique apenas as coisas após o ":", mas pode verificar também nesse link: https://jsonformatter.curiousconcept.com/
