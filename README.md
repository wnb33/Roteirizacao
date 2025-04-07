# Roteirização
Aplicativo para Rotas de Chamados de Serviços Públicos e Privados

# Otimização de Rota utilizando Teoria dos grafos

# Teoria dos Grafos

A teoria dos grafos ou de grafos é um ramo da matemática que estuda as relações entre os objetos de um determinado conjunto. Para tal são utilizadas estruturas chamadas de grafos G(V, E), Onde V é é um conjunto não vazio de objetos denominados vértices (ou nós) e E (do inglês edges - arestas) é um subconjunto de pares não ordenados de V.

Dependendo da aplicação, arestas podem ou não ter direção, pode ser permitido ou não arestas ligarem um vértice a ele próprio e vértices e/ou arestas podem ter um peso (numérico) associado. Se as arestas têm um sentido associado (indicado por uma seta na representação gráfica) temos um dígrafo (grafo orientado). Um grafo com um único vértice e sem arestas é conhecido como grafo trivial.

Estruturas que podem ser representadas por grafos estão em toda parte e muitos problemas de interesse prático podem ser formulados como questões sobre certos grafos. Por exemplo, a estrutura de ligações da Wikipédia pode ser representada por um dígrafo: os vértices são os artigos da Wikipédia e existe uma aresta do artigo A para o artigo B se e somente se A contém um link para B. Dígrafos são também usados para representar máquinas de estado finito. O desenvolvimento de algoritmos para manipular grafos é um tema importante da ciência da computação.

![Image](https://github.com/user-attachments/assets/b93dea42-4dee-482c-b6b0-993ee57c51cb)

# Algoritimo de Dijkstra

O algoritmo de Dijkstra encontra um caminho mais curto de um vértice de origem s para todos os outros vértices. Calcularemos, para cada vértice v, o peso de um caminho mais curto da origem até v, que denotaremos por . 
Agora, essa notação pressupõe que temos uma variável de instância para cada vértice. Não precisamos armazenar pesos de caminho mais curto como variáveis de instância. Por exemplo, podemos usar um mapa, mapeando cada vértice para seu menor peso de caminho. Mas para 
entender o algoritmo, usaremos . Também acompanharemos o ponteiro traseiro em cada caminho mais curto. A nomenclatura padrão para um ponteiro de fundo em um caminho mais curto é um predecessor e, portanto, denotaremos o predecessor do vértice v em um caminho mais curto
da fonte por . Tal como acontece com os ponteiros traseiros no BFS, os predecessores em caminhos mais curtos formam uma árvore direcionada, com arestas apontando para caminhos em direção à fonte.v.distdistv.distv.pred

Gosto de pensar no algoritmo de Dijkstra como uma simulação de envio de executores sobre o grafo, começando no vértice de origem s. Idealmente, a simulação funciona da seguinte maneira, embora vejamos que o algoritmo de Dijkstra funciona de maneira um pouco diferente.
Ele começa enviando executores do vértice de origem para todos os vértices adjacentes. A primeira vez que um corredor chega a qualquer vértice, os corredores imediatamente deixam esse vértice, indo para todos os seus vértices adjacentes.



