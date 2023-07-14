# Dia-da-Ira

Patch com a tradução em português da visual novel Dies Irae ~ Amantes Amentes ~, compatível com a versão Steam/DX package e a versão japonesa em HD -Animation Anniversary-.

Além de adicionar a tradução, este patch restaura o cursor original do jogo, a música original de menu e a cor original de texto lido, o título original do capítulo VI e os nomes oficiais que aparecem entre os capítulos.
Há a possibilidade de trocar a abertura do jogo pela versão de switch, pegando o arquivo na pasta vídeo e substituindo.

Inicialmente, pretendo inserir no script trechos do jogo que traduzi durante os anos de 2017 a 2019.
Posteriormente, continuarei a traduzir os extras e algumas cenas aleatórias.

# Progresso

Prólogo - 100%
Rota comum - 5/6 capítulos
Rota da Kasumi - 0/7 capítulos 0%
Rota da Kei - 0/7 capítulos 0%
Rota da Mari - 0/7 capítulos 0%
Rota da Rea - 2/7 capítulos
Other Story - 3/5  capítulos

# Instalação
- Baixe o programa [GARbro](https://github.com/morkt/GARbro/releases/tag/v1.5.44)
- Utilize-o para extrair o conteúdo dos arquivos "data1.dat" e "data3.dat" na versão Steam. Na versão japonesa, apenas o "data1.dat".
- Você obterá uma pasta "data" com várias subpastas.
- Delete "data1.dat" e "data3.dat" se estiver com a versão Steam. Delete apenas "data1.dat" se estiver com a versão japonesa.
- Se abrir normalmente, esta etapa foi um sucesso.

(Esse processo é necessário para que não seja preciso literalmente compartilhar 90% do conteúdo do jogo, em um patch de aproximadamente 8GB e mais de 100 mil arquivos)

- Agora baixe o patch disponível aqui no Github.
- Coloque o arquivo malie.ini na pasta raiz do jogo, substituindo o já existente.
- Pegue o conteúdo da pasta "data" que você baixou com o patch e o distribua nas subpastas correspondentes da sua pasta "data", substituindo os arquivos já existentes.
- Na pasta data/picture/event/dead, delete os .dzi e substitua pelos .png
# Explicação de como o Patch funciona.

Dentro do arquivo .ini estão instruções para a restauração da música de menu e cor do texto lido, em conformidade com a versão original japonesa.
Dentro da pasta "data" estão todos os arquivos dos data1.dat e data3.dat que você extraiu. Nela você colocará os arquivos do patch também.
A decompilação dos data.dat se faz necessária pois não há como inserir os arquivos da tradução dentro deles, por isso seu conteúdo precisa estar aberto.


# Tradução

Para traduzir, é necessário extrair o arquivo exec.dat de dentro do data3.dat, localizado na pasta system.
Tendo extraído, utilize o programa StringTool.exe, feito por marcussacana, para converter o script em exec.txt.
Para compilar, utilize novamente o programa StringTool.exe.

É importante que tanto o exec.dat quanto o exec.txt tenham o mesmo número de linhas e estejam na mesma pasta.
Caso o número de linhas não seja igual, o programa não irá compilar.

O script de Dies Irae possuí uma peculiaridade: cada palavra em itálico ou sobrescrita (ruby) obrigatoriamente exige estar separada em uma nova linha. 
Por causa disso, devido as diferenças gramaticais é muito difícil utilizar o script japonês e manter o exato número de linhas, assim sendo é recomendado o uso do script em inglês.

Devido a limitação do número de linhas, você não pode remover itálicos e sobrescritos(embora possa ignorar), tampouco pode adicionar novos itálicos ou sobrescritos, fazendo com que seja refém da suposta tradução em inglês.
O script em inglês possuí um total de 98465 linhas, enquanto o script japonês possuí 118965 linhas. Ao todo são aproximadamente 60000 linhas de texto.

Para traduzir, é recomendado utilizar o japonês como base e depois copiar as linhas para a versão em inglês, pois a suposta tradução, em muitos momentos assemelhasse a uma fanfic (especialmente as partes traduzidas pelo Steiner, vulgo Ludo - Rota da Marie e Other Story), com toda a narração de 1º pessoa reescrita em 3º pessoa, com exceção do protagonista. Muitas linhas ignorando parte do japonês ou acrescentando frases que não existem.

# Observações

- Até o momento, não é possível traduzir as escolhas nem mudar o nome dos personagens da caixa de texto. Não faço ideia de como fazer isso.
- Os nomes na caixa e na tradução podem variar, pois a tradução segue a grafia oficial, enquanto a suposta tradução em inglês mudou boa parte deles.
- Outro problema desta versão é que o texto é justificado, o que gera um kerning ruim e atrapalha a leitura.
Infelizmente não há solução para isso.
- Entre a versão Steam e a versão japonesa de Aniversário, recomendo a segunda pois ela permite alterar entre 16:9 e 4:3.
- Extraindo o conteúdo da versão de Switch, aparenta ter um .exe para a criação de novos .dat. Com ele, talvez seja possível criar um só com os arquivos da tradução, evitando ter que extrair as coisas com o GARbro, porém só testarei isso se a tradução foi concluída.
- Possivelmente por questões de incompetência, algumas poucas linhas do japonês não existem na suposta tradução em inglês. Restaurá-las é impossível na maioria das vezes pois implicaria em adicionar novas linhas no script, mas fazendo isso a compilação quebra.