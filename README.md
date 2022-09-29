# DP2



307 - Sticks

Enunciado
Com um input de quantos “sticks” terá de ser processado iremos descobrir como juntar esses de forma a formar “sticks” de tamanho igual com menor tamanho possível

Hipótese 1: Dar um Sort nos sticks e verificar se o maior é formado com os outros sticks, senão maior mais menor, senão maior com segundo menor.
          Falha ( não leva em conta as somas irregulares e pouco eficiente)
          
1 2 3 4 5 6
// pega do maior para menor
Se: menor + segundoMenor > Maior ( 2 + 5)
  break;
Senao:
  continue;

