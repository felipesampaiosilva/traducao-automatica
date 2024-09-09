# traducao-automatica

1. Ajustando o argumento num_examples na função load_data_nmt: O tamanho dos vocabulários de origem e destino aumenta conforme o número de exemplos utilizados cresce, já que mais palavras são vistas no conjunto de dados. Quando reduzimos o número de exemplos, o vocabulário se torna menor, limitando o modelo a um conjunto mais restrito de palavras, o que pode simplificar o treinamento, mas pode impactar negativamente a generalização.

2. Tokenização em idiomas como chinês e japonês: A tokenização em nível de palavra não é ideal para esses idiomas, pois não há delimitadores claros entre palavras, como espaços. Nesses casos, é melhor usar tokenização em nível de caractere ou técnicas como Byte-Pair Encoding (BPE) ou SentencePiece, que lidam melhor com a segmentação e a estrutura dos idiomas.
