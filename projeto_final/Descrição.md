# Visualizando a Poesia de Belchior
Antonio Carlos Belchior, mais conhecido como Belchior (Sobral, 26 de outubro de 1946 – Santa Cruz do Sul, 30 de abril de 2017), foi um compositor cearense entre os mais notórios do cancioneiro popular brasileiro.  Dono de uma obra de grande densidade e complexidade estético, literária e filosófica, suas ricas composições são objeto de estudo acadêmico e um marco da cultura cearense. Neste trabalho, propomos uma análise de suas letras (apenas as em português) através de técnicas de processamento de linguagem natural [1] e de visualização de dados [2], buscando extrair informações como palavras e expressões com maior relevância, similaridade entre letras e análise de sentimento através da ferramenta LinguaKit [3].

### Descrição dos Dados: como os dados serão obtidos, tamanho, qual o tipo deles, que tipo de limpeza ou manipulação devem ser feitas, etc.
Os dados são em formato HTML que serão extraídos do site Letras (https://www.letras.mus.br/).  Para tanto, será utilizado um web crawler que visitará iterativamente cada página de letras do artista, por álbum, armazenando estas em um arquivo json. Para cada instância, haverá o texto da letra, o título da música e o nome do álbum. Para realizar as diferentes visualizações, serão necessárias etapas de processamento de linguagem natural: normalização, remoção de stopwords, tokenização, detecção de fim de sentença, vetorização de documento, POS-tagging e chunking.  Dependendo da visualização, técnicas diferentes serão aplicadas.

### Perguntas de partida / hipóteses
Quais os termos mais relevantes na obra toda? Quais os termos mais relevantes por álbum? Quais letras possuem maior similaridade? Qual a polaridade de sentimento dominante na obra? E por álbum? Quais são as palavras que mais ocorrem juntas? 

### Referências Bibliográficas
[1]  Bird, Steven, Edward Loper and Ewan Klein (2009), Natural Language Processing with Python. O’Reilly Media Inc.

[2] Munzner, Tamara (2014). Visualization Analysis and Design. A K Peters Visualization Series, CRC Press.

[3] Gamallo, Pablo & Garcia, Marcos. (2017). LinguaKit: A multilingual tool for linguistic analysis and information extraction. Linguamática. 9. 19-28. 10.21814/lm.9.1.243. 
