# Dia-da-Ira

Patch com a tradução em português da visual novel Dies Irae ~Amantes Amentes~, feito para a versão Steam.

Além de adicionar a tradução, esta patch restaura o cursor original do jogo, a música original de menu e a cor original de texto lido.

# Instalação

Adquira a versão Steam do jogo.
Baixe o patch, que consiste num arquivo "malie.ini" e uma pasta "data".
Coloque ambos na pasta do jogo e exclua o arquivo data3.dat.

Dentro do arquivo .ini estão instruções para a restauração da música e cor.
Dentro da pasta "data" estão todos os arquivos do data3.dat que você deletou, junto ao arquivo do cursos e o script traduzido.

É necessário ter o conteúdo do data3.dat descompilado na pasta "data" pois não é como inserir coisas dentro dele, mas por sorte a engine reconhece os arquivos mesmo fora dele.


# Tradução

Para traduzir, é necessário extrair o arquivo exec.dat de dentro do data3.dat, localizado na pasta system.
Tendo extraído, ultilize o programa StringTool.exe, feito por marcussacana, para converter o script em exec.txt.
Para compilar, utilize novamente o programa StringTool.exe.

É importante que tanto o exec.dat quanto o exec.txt tenham o mesmo número de linhas e estejam na mesma pasta.
Caso o número de linhas não seja igual, o programa não irá compilar.

O script de Dies Irae possuem uma peculiaridade: cada palavra em itálico ou sobrescrita (ruby) obrigatoriamente exige estar separada em uma nova linha. 
Por causa disso, devido as diferenças gramaticais é muito difícil utilizar o script japonês e manter o exato número de linhas, assim sendo é recomendado o uso do script em inglês.
Devido a limitação do número de linhas, você não pode remover itálicos e sobrescritos, tampouco pode adicionar novas itálicos ou sobrescritos, fazendo com que seja refém da suposta tradução em inglês.

Para traduzir, é recomendado utilizar o japonês como base e depois copiar as linhas para a versão em inglês, pois a supostatradução, em muitos momentos assemelhasse a uma fanfic, com toda a narração de 1º pessoa reescrita em 3º pessoa, com exceção do protagonista.

# Observações

Os nomes dos per