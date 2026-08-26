==================================================
ALGORITMO GENÉTICO PASSO A PASSO
==================================================

População inicial: [[0, 1, 0, 1, 1], [0, 0, 1, 1, 0], [0, 1, 0, 0, 1], [0, 1, 0, 0, 1], [1, 1, 0, 1, 1], [0, 0, 1, 0, 0]]

==================== GERAÇÃO 0 ====================

Avaliação dos indivíduos:
  [0, 1, 0, 1, 1] → x=11 → f(x)=121
  [0, 0, 1, 1, 0] → x= 6 → f(x)= 36
  [0, 1, 0, 0, 1] → x= 9 → f(x)= 81
  [0, 1, 0, 0, 1] → x= 9 → f(x)= 81
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [0, 0, 1, 0, 0] → x= 4 → f(x)= 16

 Melhor: x = 27 → f(x) = 729

==================== GERAÇÃO 1 ====================

Avaliação dos indivíduos:
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 0, 0, 1, 0] → x=18 → f(x)=324
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [0, 1, 0, 0, 1] → x= 9 → f(x)= 81
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 0, 1, 1] → x=27 → f(x)=729

 Melhor: x = 27 → f(x) = 729

==================== GERAÇÃO 2 ====================

Avaliação dos indivíduos:
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 0, 0, 1, 1] → x=19 → f(x)=361

 Melhor: x = 27 → f(x) = 729

==================== GERAÇÃO 3 ====================

Avaliação dos indivíduos:
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 0, 0, 1] → x=25 → f(x)=625
  [1, 0, 0, 1, 0] → x=18 → f(x)=324
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 0, 1, 1] → x=27 → f(x)=729

 Melhor: x = 27 → f(x) = 729

==================== GERAÇÃO 4 ====================

Avaliação dos indivíduos:
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [0, 1, 0, 1, 0] → x=10 → f(x)=100
  [1, 0, 1, 0, 1] → x=21 → f(x)=441
  [1, 1, 1, 1, 0] → x=30 → f(x)=900
  [1, 0, 0, 0, 1] → x=17 → f(x)=289
  [1, 1, 0, 1, 1] → x=27 → f(x)=729

 Melhor: x = 30 → f(x) = 900

==================== GERAÇÃO 5 ====================

Avaliação dos indivíduos:
  [1, 1, 1, 1, 0] → x=30 → f(x)=900
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 1, 1, 1] → x=31 → f(x)=961
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 1, 1, 0] → x=30 → f(x)=900
  [1, 1, 0, 1, 1] → x=27 → f(x)=729

 Melhor: x = 31 → f(x) = 961

==================== GERAÇÃO 6 ====================

Avaliação dos indivíduos:
  [1, 1, 1, 1, 1] → x=31 → f(x)=961
  [1, 1, 1, 1, 1] → x=31 → f(x)=961
  [1, 1, 0, 1, 0] → x=26 → f(x)=676
  [1, 1, 0, 1, 0] → x=26 → f(x)=676
  [1, 1, 1, 1, 1] → x=31 → f(x)=961
  [1, 1, 0, 1, 0] → x=26 → f(x)=676

 Melhor: x = 31 → f(x) = 961

==================== GERAÇÃO 7 ====================

Avaliação dos indivíduos:
  [1, 1, 1, 1, 1] → x=31 → f(x)=961
  [1, 1, 1, 1, 0] → x=30 → f(x)=900
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 1, 0, 1, 1] → x=27 → f(x)=729
  [1, 0, 0, 1, 0] → x=18 → f(x)=324
  [0, 1, 0, 1, 0] → x=10 → f(x)=100

 Melhor: x = 31 → f(x) = 961

==================================================
RESULTADO FINAL
==================================================

Melhor indivíduo: [1, 1, 1, 1, 1]
x = 31
f(x) = 961

Ótimo global: x = 31, f(x) = 961
Erro: 0





-----

Professor, tendo em vista a sua explicacao sobre a margem de populacao, tanto quanto quanto o numero de POP como este:
POP_SIZE = 6
BITS = 5
GERACOES = 8
TAXA_MUTACAO = 0.1

se tem como entendido que, de geracao em geracao, dependendo das variveis colocadas, a solucao otima ou heuristca podem ser encontradas mais rapidamente.
e como eu perguntei durante a aula, a quantidade de taxa de mutacao tem que ser baixa e a 


RESULTADOS LAB2:

==================================================
ONEMAX - AG com 10 indivíduos, 100 gerações
==================================================
Geração   0: Melhor = 13/20, Média = 9.70
Geração  10: Melhor = 18/20, Média = 16.10
Geração  20: Melhor = 19/20, Média = 16.80
Geração  30: Melhor = 16/20, Média = 14.60
Geração  40: Melhor = 18/20, Média = 14.40
Geração  50: Melhor = 16/20, Média = 14.90
Geração  60: Melhor = 18/20, Média = 15.00
Geração  70: Melhor = 18/20, Média = 15.80
Geração  80: Melhor = 16/20, Média = 14.30
Geração  90: Melhor = 17/20, Média = 14.40

 MELHOR FITNESS: 17/20
   Ótimo = 20 (todos os bits são 1)

lab_02 explicacoes

explicacao:  " 
question N-1: the answer for the question is the following, at the moment that we raise the mutation probability, the amount of likely improvment, is instantly deleted

question N-2: " when the population is lowered, the amount of "chances" and tries are basically arriving to a low quality, making the code not having a good status

question N-3: "when we raise the number of generations, we are basically incresing the quantity of "varieties" and the good binaries be kept (of course, if the elite number had kept the same, 2)

question N-4: "when we changed the elite to 0, we are saying to the code that we can't stay with the same genetics that were before discovered, neither to know about earlier generations

considerações:

Analisando os dois códigos, entendemos que:
Configuração 1 (pop=30, ger=50, mut=0.02, elite=2) convergiu rápido e ficou estável
Chegou no ótimo (20/20) já na geração 10 e se manteve lá até o fim. Isso mostra uma combinação "equilibrada": população grande o suficiente pra manter diversidade genética, mutação baixa o suficiente pra não destruir bons indivíduos, e elitismo garantindo que o melhor encontrado nunca se perde de uma geração pra outra.

Configuração 2 (pop=10, ger=100, mut=0.1, elite=0), nunca convergiu, mesmo com o dobro de gerações
Aqui o melhor fitness fica oscilando (14 → 17 → 18 → 16 → 19 → 15...) e termina em 15/20, pior que o pico de 19/20 lá na geração 70. Ou seja: o algoritmo achou uma solução quase ótima e depois a perdeu. Isso só é possível porque ELITE=0 — sem elitismo, não existe garantia de que o melhor indivíduo sobreviva à próxima geração; ele pode ser destruído por crossover/mutação e nunca mais reaparecer.

Por que isso aconteceu, parâmetro por parâmetro:

População pequena (10): pouca diversidade genética disponível pro torneio de seleção escolher bons pais; o "pool genético" é raso.
Mutação alta (0.1 vs 0.02): com 20 bits, uma taxa de 10% significa em média 2 bits mutando por indivíduo a cada geração, isso é ruído demais perto do ótimo, os bits corretos ficam sendo "desfeitos" quase tão rápido quanto são encontrados.
Elite=0: essa é provavelmente a causa mais decisiva da instabilidade. Sem preservar o melhor indivíduo, o algoritmo não tem "memória" do progresso, cada geração começa do zero em termos de garantia.
Mais gerações (100 vs 50) não compensou nada disso: rodar o dobro de tempo com parâmetros ruins não substitui parâmetros bem ajustados. Quantidade de iterações ≠ qualidade da busca.

Conclusão geral (juntando com o AG anterior, do f(x)=x²): os dois experimentos reforçam que um Algoritmo Genético é, no fim das contas, um equilíbrio entre exploração (mutação, diversidade populacional, testar coisas novas) e exploração do que já funciona (elitismo, seleção proporcional ao fitness, não perder o que é bom). A Configuração 1 pende pro lado da exploitation e converge rápido; a Configuração 2 exagera na exploration a ponto de o algoritmo "esquecer" boas soluções que já tinha achado. Isso é uma ilustração bem prática de um dos dilemas centrais de computação evolutiva: mutação e diversidade são necessárias pra não ficar preso em ótimo local, mas em excesso e sem elitismo pra ancorar o progresso elas impedem a convergência.


LAB3:

Resultados: ==================================================
OTIMIZANDO f(x) = x * sin(3x)
==================================================
Geração   0: Melhor f(x) = 6.0863 (x = 6.6667)
Geração  10: Melhor f(x) = 8.9019 (x = 8.9020)
Geração  20: Melhor f(x) = 8.9019 (x = 8.9020)
Geração  30: Melhor f(x) = 8.9019 (x = 8.9020)
Geração  40: Melhor f(x) = 8.9019 (x = 8.9020)

Considerações:

Convergência rápida e "travada": o AG achou x ≈ 8,90 (f(x) ≈ 8,90) já na geração 10 e ficou parado ali até a geração 50. Isso indica que o algoritmo caiu num ótimo local forte e não teve estímulo suficiente pra escapar com TAXA_MUT = 0.05 e apenas 8 bits de resolução, depois que a população converge, fica difícil "pular" pra outro pico da função sem uma mutação mais agressiva ou reinício de diversidade.
Resolução dos 8 bits limita a precisão: com 256 valores possíveis discretizando o intervalo [0,10], o "grão" mínimo de x é de ~0,039. Isso é suficiente pra achar um bom pico, mas não garante achar o x exato que maximiza a função é uma limitação da própria representação binária, não do algoritmo em si.
A função tem múltiplos ótimos locais (por ser x·sin(3x), oscila bastante), e não temos garantia de que 8,90 é o máximo global do intervalo só sabemos que é o melhor que essa população específica encontrou. Seria interessante rodar com seeds diferentes pra ver se o AG converge sempre pro mesmo pico ou se varia.
O deslocamento do fitness (+10) foi necessário, mas é um detalhe de implementação que merece nota no relatório: como a função original tem valores negativos, a seleção por roleta (que soma fitnesses diretamente) exigiu esse ajuste. É um lembrete prático de que a escolha do método de seleção impõe restrições sobre como modelar o fitness com seleção por torneio, por exemplo, esse deslocamento nem seria necessário.
