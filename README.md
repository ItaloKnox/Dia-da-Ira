# Dia-da-Ira

Patch com a tradução em português da visual novel Dies Irae ~ Amantes Amentes ~, feito para a versão Steam.

Além de adicionar a tradução, esta patch restaura o cursor original do jogo, a música original de menu e a cor original de texto lido.

Inicialmente, pretendo inserir no script trechos do jogo que traduzi durante os anos de 2017 a 2019. Essas traduções podem ser encontradas no site da Knox.
Posteriormente, continuarei a traduzir os extras e algumas cenas aleatórias.

# Instalação e Explicação de como o Patch funciona.
- Caso tenha adquirido o jogo legalmente, abra-o uma primeira vez. Ele exige conexão com a internet na primeira execução.
- Baixe o programa [GARbro](https://github.com/morkt/GARbro/releases/tag/v1.5.44)
- Utilize-o para extrair o conteúdo dos arquivos "data1.dat" e "data2.dat".
- Deixe todo o conteúdo em uma única pasta chamada "data".
- Delete "data1.dat" e "data2.dat" e abra o jogo. Se abrir normalmente, esta etapa foi um sucesso.

(Esse processo é necessário para que não seja preciso literalmente compartilhar 90% do conteúdo do jogo, em um patch de aproximadamente 8GB e mais de 100 mil arquivos)

- Agora baixe o patch disponível futuramente aqui no Github.
- Coloque o arquivo malie.ini na pasta raiz do jogo, substituindo o já existente.
- Pegue o conteúdo da pasta "data" que você baixou com o patch e o distribua nas subpastas correspondentes da sua pasta "data", substituindo os já existentes.

# Explicação de como o Patch funciona.

Dentro do arquivo .ini estão instruções para a restauração da música de menu e cor do texto lido, em conformidade com a versão original japonesa.
Dentro da pasta "data" estão todos os arquivos do data3.dat, que você precisa deletar, junto ao arquivo do cursor e o script traduzido.

É necessário ter o conteúdo do data3.dat descompilado na pasta "data" pois não há como inserir coisas dentro dele, mas por sorte a engine reconhece os arquivos fora dele, desde que eles existam na pasta "data" e o ".dat" correspondente tenha sido deletado.


# Tradução

Para traduzir, é necessário extrair o arquivo exec.dat de dentro do data3.dat, localizado na pasta system.
Tendo extraído, utilize o programa StringTool.exe, feito por marcussacana, para converter o script em exec.txt.
Para compilar, utilize novamente o programa StringTool.exe.

É importante que tanto o exec.dat quanto o exec.txt tenham o mesmo número de linhas e estejam na mesma pasta.
Caso o número de linhas não seja igual, o programa não irá compilar.

O script de Dies Irae possuí uma peculiaridade: cada palavra em itálico ou sobrescrita (ruby) obrigatoriamente exige estar separada em uma nova linha. 
Por causa disso, devido as diferenças gramaticais é muito difícil utilizar o script japonês e manter o exato número de linhas, assim sendo é recomendado o uso do script em inglês.

Devido a limitação do número de linhas, você não pode remover itálicos e sobrescritos, tampouco pode adicionar novos itálicos ou sobrescritos, fazendo com que seja refém da suposta tradução em inglês.
O script em inglês possuí um total de 98463 linhas, enquanto o script japonês possuí 118965 linhas.

Para traduzir, é recomendado utilizar o japonês como base e depois copiar as linhas para a versão em inglês, pois a suposta tradução, em muitos momentos assemelhasse a uma fanfic, com toda a narração de 1º pessoa reescrita em 3º pessoa, com exceção do protagonista.

# Observações

- Até o momento, não é possível traduzir as escolhas nem mudar o nome dos personagens da caixa de texto. Não faço ideia de como fazer isso.
- Os nomes na caixa e na tradução podem variar, pois a tradução segue a grafia oficial, enquanto a suposta tradução em inglês mudou boa parte deles.
- Visando manter a estética original do jogo, a tradução sempre deixa um espaço em branco no início dos parágrafos, bem como ocorre no japonês e foi removido na suposta tradução.
- Ainda visando a fidelidade com o original, a tradução mantém busca preservar a estética da pontuação original.
- Outro problema desta versão é que o texto é justificado à esquerda, o que gera um kerning ruim e atrapalha a leitura.
Infelizmente não há solução para isso.
