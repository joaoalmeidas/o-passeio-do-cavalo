# o-passeio-do-cavalo
Exercicio 7.22 do livro Java: Como Programar

(Passeio do cavalo) Um problema interessante para os fãs de xadrez é o problema do Passeio do Cavalo, originalmente proposto pelo
matemático Euler. A peça do cavalo pode mover-se em um tabuleiro vazio e tocar cada um dos 64 quadrados somente uma única vez? Aqui,
estudamos esse intrigante problema em profundidade.
O cavalo só faz movimentos em forma de L (dois espaços em uma direção e um outro em uma direção perpendicular). Portanto, como
mostrado na Figura 7.30, partindo de um quadrado próximo do centro de um tabuleiro de xadrez vazio, o cavalo (rotulado K) pode fazer oito
movimentos diferentes (numerados de 0 a 7).
a) Desenhe um tabuleiro de xadrez oito por oito em uma folha de papel e tente o Passeio do Cavalo manualmente. Coloque um 1 no quadrado inicial, um 2 no segundo quadrado, um 3 no terceiro e assim por diante. Antes de iniciar o passeio, estime até onde você chegará,
lembrando que um passeio completo consiste em 64 movimentos. Até onde você foi? Isso foi próximo de sua estimativa?
b) Agora vamos desenvolver um aplicativo que moverá o cavalo pelo tabuleiro. O tabuleiro é representado por um array bidimensional
oito por oito board. Cada quadrado é inicializado como zero. Descrevemos cada um dos oito possíveis movimentos em termos de
seus componentes vertical e horizontal. Por exemplo, um movimento do tipo 0, como mostrado na Figura 7.30, consiste em mover
dois quadrados horizontalmente para a direita e um quadrado verticalmente para cima. Um movimento do tipo 2 consiste em mover
um quadrado horizontalmente para a esquerda e dois quadrados verticalmente para cima. Movimentos horizontais para a esquerda e
movimentos verticais para cima são indicados com números negativos. Os oitos movimentos podem ser descritos por dois arrays unidimensionais, horizontal e vertical, como segue:

Faça com que as variáveis currentRow e currentColumn indiquem, respectivamente, a linha e a coluna da posição atual
do cavalo. Para fazer um movimento do tipo moveNumber, em que moveNumber está entre 0 e 7, seu aplicativo deve utilizar as
instruções
currentRow += vertical[moveNumber];
currentColumn += horizontal[moveNumber];
Escreva um aplicativo para mover o cavalo pelo tabuleiro. Mantenha um contador que varia de 1 a 64. Registre a última contagem
em cada quadrado para o qual o cavalo se move. Teste cada movimento potencial para ver se o cavalo já visitou esse quadrado. Teste
cada movimento potencial para assegurar que o cavalo não saia fora do tabuleiro. Execute o aplicativo. Quantos movimentos o cavalo
fez?
