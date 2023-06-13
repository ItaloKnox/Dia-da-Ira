# Dia-da-Ira

Patch com a tradução em português da visual novel Dies Irae ~ Amantes Amentes ~, feito para a versão Steam.

Além de adicionar a tradução, esta patch restaura o cursor original do jogo, a música original de menu e a cor original de texto lido.

Inicialmente, pretendo inserir no script trechos do jogo que traduzi durante os anos de 2017 a 2019. Essas traduções podem ser encontradas no site da Knox.
Posteriormente, continuarei a traduzir os extras e algumas cenas aleatórias.

# Instalação

Adquira a versão Steam do jogo, oficialmente ou não.
Baixe o patch, que consiste num arquivo "malie.ini" e uma pasta "data".
Coloque ambos na pasta do jogo e exclua o arquivo data3.dat.

Dentro do arquivo .ini estão instruções para a restauração da música e cor.
Dentro da pasta "data" estão todos os arquivos do data3.dat que você deletou, junto ao arquivo do cursor e o script traduzido.

É necessário ter o conteúdo do data3.dat descompilado na pasta "data" pois não há como inserir coisas dentro dele, mas por sorte a engine reconhece os arquivos mesmo fora dele, desde que eles existam na pasta "data" e o ".dat" correspondente tenha sido deletado.


# Tradução

Para traduzir, é necessário extrair o arquivo exec.dat de dentro do data3.dat, localizado na pasta system.
Tendo extraído, utilize o programa StringTool.exe, feito por marcussacana, para converter o script em exec.txt.
Para compilar, utilize novamente o programa StringTool.exe.

É importante que tanto o exec.dat quanto o exec.txt tenham o mesmo número de linhas e estejam na mesma pasta.
Caso o número de linhas não seja igual, o programa não irá compilar.

O script de Dies Irae possuem uma peculiaridade: cada palavra em itálico ou sobrescrita (ruby) obrigatoriamente exige estar separada em uma nova linha. 
Por causa disso, devido as diferenças gramaticais é muito difícil utilizar o script japonês e manter o exato número de linhas, assim sendo é recomendado o uso do script em inglês.
Devido a limitação do número de linhas, você não pode remover itálicos e sobrescritos, tampouco pode adicionar novas itálicos ou sobrescritos, fazendo com que seja refém da suposta tradução em inglês.
O script em inglês possuem um total de 98463 linhas, enquanto o script japonês possuí 118965 linhas.

Para traduzir, é recomendado utilizar o japonês como base e depois copiar as linhas para a versão em inglês, pois a suposta tradução, em muitos momentos assemelhasse a uma fanfic, com toda a narração de 1º pessoa reescrita em 3º pessoa, com exceção do protagonista.

# Observações

Até o momento, não é possível traduzir as escolhas nem mudar o nome dos personagens da caixa de texto. Não faço ideia de como fazer isso.
Os nomes na caixa e na tradução podem variar, pois a tradução segue a grafia oficial, enquanto a suposta tradução em inglês mudou boa parte deles.
No menu de volume das vozes, os nomes aparecem em japonês para remover os nomes errôneos do inglês. Infelizmente não é possível fazer o mesmo em todas as imagens porque isso me obrigaria a abrir todos os .dat.

Além disso, o vídeo de abertura permanece também sem tradução, pois não é possível inseri-lo sem abrir o data1.dat
Meu objetivo é fornecer apenas um script traduzido, não disponibilizar o jogo inteiro para download. Ao abrir os demais .dat, o patch ficaria com cerca de 7GB e mais de 100 mil arquivos.
Para compensar a falta do vídeo traduzido, será disponibilizado um vídeo à parte com a tradução. Se esta tradução for finalizada, eu farei um patch completo abrindo o .dat. 

Outro problema desta versão é que o texto é justificado à esquerda, o que gera um kerning ruim e atrapalha a leitura.
Infelizmente não há solução para isso.
