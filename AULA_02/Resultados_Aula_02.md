PASSO 1: Compreensão e Execução

1- "Porque o total de soluções avaliadas é exatamente 32?"
Porque são 5 itens e apenas 2 possibilidades para cada (levar ou não levar) - 2x2x2x2x2 = 32
2-"O que aconteceria se eu colocasse 15 itens?"
Seriam avaliadas 32768 possibilidades (2^15 - 2x2x2x2x2x2x2x2x2x2x2x2x2x2x2 = 32768)
3-"Vocês conseguem imaginar um preblema da vida real parecido com esse?"
A quantidade de produtos comprados no super mercado (Compara ou não comprar) com a restrição do meu dinheiro


PASSO 2: Execução código pronto

Total de solucoes avaliadas: 32
Tempo de execucao: 0.000792 segundos
Melhor valor encontrado: 9
Combinacao otima (0=nao leva, 1=leva): (1, 1, 0, 1, 1)

Itens escolhidos:
 - Livro (peso: 2 , valor: 3 )
 - Fone (peso: 1 , valor: 2 )
 - Carregador (peso: 1 , valor: 3 )
 - Chocolate (peso: 1 , valor: 1 )


PASSO 3: Execução código semi-pronto



PASSO 4: Execução do zero


LAB3_AULA2

# 19. Codigo completo (com a funcao calcular_gap inovadora e o loop funcionando). - / Arquivo .ipynb no repositório
# 20. Valor do gap médio obtido. - Gap médio: 0.39%
# 21. Resposta: "A heuristica gulosa e boa o suficiente para este problema? Em quais situacoes voce usaria ela e em quais preferiria gastar mais tempo para achar o otimo?" - Levando em consideração que os resultados obtidos são mínimos em todos os casos, consideramos a Heuristica boa para o problema. O problema poderia ser replicado em situações como: viagens de barco com limite de pessoas e uma qujantidade elevada de pessoas para transpostar por exemplo e esse já é um otimo exemplo de situação em que seria de extrema importancia gastar mais tempo para achar o "ótimo"

LAB4_AULA2

Resultados: 
Numero de tarefas: 12
Tamanho do espaco de busca (2^n): 4096

Solucao aleatoria gerada: (0, 0, 1, 0, 0, 0, 0, 0, 1, 0, 0, 0)

Tarefas selecionadas:
 - Refatorar service de apolices (horas: 12, valor: 6)
 - Testes automatizados modulo X (horas: 8, valor: 6)

Valor total (funcao objetivo): 12
Horas totais utilizadas: 20 / 40
Solucao factivel (respeita restricao de horas)? Sim

CONSIDERAÇÕES:

Sobre a Atividade 1 (força bruta): o resultado de 32 soluções avaliadas pra 5 itens já deixa claro o problema central: o espaço de busca é $2^n$, então crescimento é exponencial, não linear. Com 15 itens já seriam 32.768 combinações, e com 30 itens passaria de 1 bilhão. Isso é o tipo de coisa que só "clica" de verdade quando a gente vê o número saltando — na teoria parece abstrato, mas rodando o código dá pra sentir o motivo pelo qual força bruta é inviável assim que o problema cresce um pouco.

Sobre a Atividade 3 (heurística gulosa): o gap médio de 0,39% foi surpreendentemente bom, a maioria das 20 instâncias bateu o ótimo exatamente. Mas os casos com gap de 2,1% e 4,2% mostram onde a gulosa falha: ela decide "item por item" olhando só a densidade valor/peso, sem enxergar que talvez sobrar um pouco de capacidade "desperdiçada" no fim. Isso é uma lição prática sobre heurísticas em geral, elas não erram porque são "burras", erram porque tomam decisões locais sem revisão global. Pra mim isso reforça que decidir usar heurística ou método exato não é uma escolha binária de "bom vs. ruim", é uma escolha de trade-off: quanto essa margem de erro (o gap) importa pro problema real, versus quanto tempo/recurso computacional eu tenho pra rodar o método exato.

Sobre a Atividade 4 (modelagem do problema real): o que mais me chamou atenção foi perceber que um problema do meu dia a dia de trabalho (escolher quais tarefas atacar numa sprint) é literalmente a mesma estrutura matemática da mochila — isso é uma virada de chave interessante: parar de ver "problema da mochila" como um exercício acadêmico isolado e passar a reconhecer o padrão em decisões reais (alocação de recursos com restrição de capacidade + maximização de valor aparece em logística, escalonamento, orçamento, etc). E a classificação como NP-difícil também ajuda a justificar, na prática, por que times de produto usam heurísticas informais (tipo "prioriza por valor/esforço") em vez de tentar calcular o ótimo exato toda sprint — sem saber, várias pessoas já fazem uma versão manual da heurística gulosa no dia a dia.

Juntando as três: o fio condutor é a relação entre tamanho do espaço de busca, custo computacional de garantir o ótimo e qualidade aceitável de uma solução aproximada. A força bruta prova que o ótimo existe e é encontrável em instâncias pequenas; a heurística mostra que abrir mão de garantia de otimalidade pode ser um preço baixo (gap menor que 1% na média); e o problema real mostra que essa tensão não é só teórica, ela aparece em decisões concretas de prioridade que eu (ou qualquer time) toma toda semana. Se eu fosse resumir o aprendizado da aula inteira, diria que a parte mais importante não foi implementar os algoritmos, foi entender quando vale a pena gastar tempo computacional buscando o ótimo, e quando uma resposta "boa o suficiente, rápido" já resolve o problema real.

