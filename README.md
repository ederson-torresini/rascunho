# Livro

O ponto de partida foram os vídeos do Tim Berners-Lee no Ted.com.
Lá, Berners-Lee fala sobre a Internet ser composta de dados, não de páginas.
Se o HTML separa forma de conteúdo, então uma coisa é armazenar o conteúdo e outra é apresentá-lo.
Além disso, as âncoras apontam para os próximos conteúdos. Logo, é um grafo.
Um grafo de possibilidades (árvore etc.) e outro grafo, de caminho já navegado - o histórico.
Assim, há inúmeras formas de apresentar:
- Um livro sequencial: dado, outro dado, e assim por diante.
- Um jogo de caminhos possíveis: escolha sua própria aventura.

O dado, em si, pode-se ter como analogia uma folha dobrada várias vezes.
Tem na capa um identificador genérico (hash), vários idiomas possíveis.
Pode haver o uso de IA para tradução automática, o que deve estar discriminado no idioma em questão.
Ao desdobrar uma vez, o título e palavras-chave.
Outra vez, uma frase de resumo (lide, ler sobre isso em Jornalismo), lembrando como a Wikipedia faz ao passar o mouse por cima de um conceito.
Mais uma vez, um parágrafo de explicação.
De novo, um texto completo.
Por fim, referências para outros dados.
Claro, a qualquer momento pode haver referências (âncoras) para outros dados.

Os servidores dos dados armazenam os dados como blocos.
Tem um índice de blocos, que podem ser acessados individualmente e por nível (definir os níveis previamente).
Exemplo:
- GET /dados/1/capa
onde /dados é o tipo de informação, 1 é o identificador e capa é o nível.
- GET /dados/1/capa/referencias
onde são requisitados os itens capa até referência.

Logo, o servidor pode, inclusive, sugerir os próximos dados a serem acessados:
- O próximo nível do dados.
- Um dado referenciado pelo dado corrente.

O cliente pode, também, solicitar os dados na forma de grafo (ver linguagem do Mermaid).
Ao pedir um grafo de dados, pode criar seu grafo de possibilidades para o usuário.

Cabe ao cliente, portanto, fazer as requisições e apresentar como quiser os dados.
Na forma de livro, pode bem apresentar todos os dados sequencialmente.
Pode também ser um livro interativo, onde o usuário pode expandir os dados conforme desejar, ou mesmo escolher o próximo tópico.
Exemplo: o usuário pode reler um dado, com mais ou menos profundidade, e o livro indicar com "relendo" ou "aprofundando".
Outra opção é um jogo de caminhos possíveis, onde o usuário escolhe o próximo tópico a ser lido.
Nesse caso, ele pode ser recompensado por isso, como em um jogo de RPG.
Por fim, pode ainda apresentar um grafo 3D, onde o usuário pode navegar pelos dados como se fosse um mapa.

Aparecem, assim, três tipos de servidor:
- Dados.
- Grafos: que podem conter outros grafos (ver conceito de playlist do Spotify e PIMs como Obsidian e outros).
- Armazenamento de progresso do usuário - as trilhas.

Será usado o termo grafo para caminho possível e trilha para caminho já navegado.

É preciso, assim, uma linguagem para descrever esses grafos - e trilhas - e seus possíveis caminhos:
- Estruturas de decisão: caminhos possíveis quando escolhas são feitas - ou exercícios são bem ou mal resolvidos.
- Estruturas de repetição: caminhos possíveis quando um dado é relido ou aprofundado.
(ver linguagem ink e Twine)

Os dados podem ser analisados por IAs nesses servidores de progresso, ou mesmo no cliente (ver WebAssembly?).
Podem ser desde sugestões de progresso, ou mesmo construção de novos "livros" ou "jogos" a partir dos dados e trilhas dos usuários.
Ou seja, novos grafos possíveis.

Outra opção são produtores de cursos, que podem criar seus próprios cursos (grafos) a partir dos dados.
Logo, alguns dados são certificados como "oficiais", e outros são "comunitários".
Um curso, por exemplo, pode ter um dado de apresentação, passar por vários dados de conteúdo, e terminar com um dado de avaliação.

Há, assim, vários tipos de dados:
- Conceito: teoria.
- Exemplo: prática.
- Curso: apresentação do professor/tutor/outro.
- Exercício: prática avaliativa - avaliada por professor/tutor/outro ou mesmo IA.

Mais informações podem ser armazenadas. O progresso do usuário pode gerar resultados, como XP e créditos em um sistema de economia.
O sistema de economia pode ser usado para comprar cursos pagos, ou até mesmo para contratar horas de outros usuários: mentorias etc.
