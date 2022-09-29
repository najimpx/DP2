# DP2



307 - Sticks

Enunciado
Com um input de quantos “sticks” terá de ser processado iremos descobrir como juntar esses de forma a formar “sticks” de tamanho igual com menor tamanho possível

Hipótese 1: Dar um Sort nos sticks e verificar se o maior é formado com os outros sticks, senão maior mais menor, senão maior com segundo menor.
          Falha ( não leva em conta as somas irregulares e pouco eficiente)
          
Hipótese 2: Dar um Sort nos sticks e verificar se o maior é formado com os outros sticks, senão maior mais menor, senão maior com segundo menor.
          Tira maior da Lista.
          Soma de menor até menor+segundoMenor + terceiroMenor+... = Maior
          Se igual
                    tira da lista menor+segundoMenor + terceiroMenor+...
                    faz denovo por RECURSAO
                    quartoMenor+quintoMenor+.... = Maior
                              Senao achar RECURSAO acaba
          menor+terceiroMenor+..... = Maior
          Se não achar
                    objetivo Maior+Menor
                              Tira Maior e menor da lista
                               Soma de menor até segundoMenor + terceiroMenor+... = Maior+Menor
                               
BREAK de eficiencia
1 2 3 4 5 6
// pega do maior para menor
Se: menor + segundoMenor > Maior ( 2 + 5)
  break;
Senao:
  continue;

