# Dia-da-Ira

Patch com a tradução em português da visual novel Dies Irae ~ Amantes Amentes ~, compatível com a versão inglesa DX package e a versão Steam. Funciona também com a versão japonesa em HD -Animation Anniversary-, entretanto alguns arquivos de áudio nela não existem ou são censurados, uma vez que o script da versão inglesa restaurou linhas originais da versão Acta est Fabual, que por sua vez foram censuradas na versão de console de Amantes Amentes, posteriormente portada para computador.

Além de adicionar a tradução, este patch restaura o cursor original do jogo, a música original de menu e a cor original de texto lido, o título original dos capítulos III e VI, nomes oficiais que aparecem entre os capítulos e 5 arquivos de voz faltantes por incompetência da versão inglesa.
Há a possibilidade de trocar a abertura do jogo pela versão de switch, pegando o arquivo na pasta vídeo e substituindo.

Inicialmente, pretendo inserir no script trechos do jogo que traduzi durante os anos de 2017 a 2019.
Posteriormente, continuarei a traduzir o restante.

# Progresso
- Introdução - 1/1 legenda
- Prólogo - 1/1 capítulo
- Rota comum - 6/6 capítulos
- Rota da Kasumi - 4/7 capítulos
- Rota da Kei - 1/7 capítulos
- Rota da Marie - 0/7 capítulos
- Rota da Rea - 6/7 capítulos
- Other Story - 5/5  capítulos

- A ordem adequada para jogar é também a de lançamento: Kasumi e Kei > Marie e Rea | Final 1 > Final 2 (Intercalando com as Other Story conforme são desbloqueadas)
- Kasumi e Kei compartilham boa parcela de texto em seus três primeiros capítulos, entretanto o desenrolar é diferente.
- Marie e Rea compartilham boa parcela de texto em seus dois primeiros capítulos, entretanto o desenrolar é diferente.
- Uma das Other Story compartilha texto com o final da Rea.
- Um dos finais da Rea compartilha texto com o outro final.

Resumindo, tem muito texto repetido, mas justificasse dado o conceito do déjà-vu e presciência.

# Instalação
- Baixe o programa [GARbro](https://github.com/morkt/GARbro/releases/tag/v1.5.44)
- Utilize-o para extrair o conteúdo dos arquivos "data1.dat" e "data3.dat" na versão DX. Na versão japonesa, apenas o "data1.dat".
- Você obterá uma pasta "data" com várias subpastas.
- Delete "data1.dat" e "data3.dat" se estiver com a versão DX. Delete apenas "data1.dat" se estiver com a versão japonesa.
- Se abrir normalmente, esta etapa foi um sucesso.

(Esse processo é necessário para que não seja preciso literalmente compartilhar 90% do conteúdo do jogo, em um patch de aproximadamente 8GB e mais de 100 mil arquivos)

- Agora baixe o patch disponível aqui no Github.
- Coloque o arquivo malie.ini na pasta raiz do jogo, substituindo o já existente.
- Pegue o conteúdo da pasta "data" que você baixou com o patch e o distribua nas subpastas correspondentes da sua pasta "data", substituindo os arquivos já existentes.
- Na pasta data/picture/event/dead, delete os .dzi e substitua pelos .png.
- Coloque os arquivos de áudio na pasta equivalente.
# Explicação de como o Patch funciona.

Dentro do arquivo .ini estão instruções para a restauração da música de menu e cor do texto lido, em conformidade com a versão original japonesa.
Dentro da pasta "data" estão todos os arquivos dos data1.dat e data3.dat que você extraiu. Nela você colocará os arquivos do patch também.
A decompilação dos data.dat faz-se necessária pois não há como inserir os arquivos da tradução dentro deles nem criar um novo para substituir, por isso seu conteúdo precisa estar aberto. 


# Tradução

Para traduzir, é necessário extrair o arquivo exec.dat de dentro do data3.dat, localizado na pasta system.
Tendo extraído, utilize o programa StringTool, criado por [marcussacana](https://github.com/marcussacana/SacanaWrapper), para converter o script em exec.txt.
Para compilar, utilize novamente o programa StringTool.exe.
É importante que tanto o exec.dat quanto o exec.txt tenham o mesmo número de linhas e estejam na mesma pasta.
Caso o número de linhas não seja igual, o programa não irá compilar.

Para traduzir as escolhas e nomes na caixa de texto, utilize Malie_Script_Tool, criado por [Crsky](https://github.com/crskycode/Malie_Script_Tool), para converter o script em "exec.msg.txt" e "exec.str.txt"
Para usá-lo, é necessário compilá-lo com o Visual Studio. Após obter seus .txt, compile novamente deletando as linhas 19 e 22 em "Program.cs" para que o programa possa criar o novo .dat corretamente.

O script de Dies Irae, da forma como é extraído pelo StringTool, possuí uma peculiaridade: cada palavra em itálico ou sobrescrita (ruby) obrigatoriamente exige estar separada em uma nova linha. 
Devido a diferença no número de linhas, é mais cômodo o uso do script em inglês como base.

Também por causa dessa limitação do número de linhas, você não pode remover itálicos e sobrescritos (embora possa ignorar), tampouco pode adicionar novos itálicos ou sobrescritos, fazendo com que seja refém do texto.
O script em inglês possuí um total de 98479 linhas, enquanto o script japonês possuí 118965 linhas. Ao todo são 59812 linhas de texto em si, sendo 53851 linhas únicas.

Extraindo com o Malie_Script_Tool o problema de itálicos e rubys é corrigido, mas como ele apresenta texto duplicado, o ideal é utilizá-lo apenas após terminar a tradução, para fazer apenas edições.

Para traduzir, é recomendado utilizar o japonês como base, pois a suposta tradução, em muitos momentos assemelhasse a uma fanfic - muitas linhas ignorando parte do japonês ou acrescentando frases que simplesmente não existem, repleto de palavrões incondizentes, engrandecimento da narração e uso de expressões e figuras de linguagem que não combinam com a personalidade dos personagens. Inconsistências na alternância de narração de 1º e 3º pessoa e diversas adaptações idiotas, incluindo linhas que parecem terem sido escritas por crianças de 12 anos. Não há preocupação com uma fidelidade 1:1 para com o texto japonês (seja na pontuação ou estrutura das frases); muitas liberdades "artísticas" que não possuem espaço no campo da tradução profissional. A princípio, a rota da Kei é a pior de todas.
Contudo, embora o japonês deva ser a base, deve-se utilizar o inglês para tradução, uma vez que ele restaurou linhas da versão Acta que foram censuradas no Amantes, logo o script traduzido é mais completo que o script japonês, possuindo textos sem censura e linhas adicionais. Resumindo: trabalhar com ambos lado a lado.

# Observações

- Um problema do jogo é que o texto é justificado, o que gera um kerning ruim e atrapalha a leitura. Infelizmente não há solução para isso.
- Caso queira mudar a fonte do jogo, pegue outra fonte .otf (qualquer fonte, na verdade, basta mudar a extensão para .otf) e coloque na pasta "data/font" renomeando ela com o nome da antic.
- Entre a versão DX, a versão Steam e a versão japonesa de Aniversário, recomenda-se a primeira, embora a versão japonesa tenha a possibilidade de alterar a resolução entre 16:9 e 4:3. A versão Steam simplesmente não foi testada, mas deve funcionar se a estrutura de arquivos for a mesma.
- Extraindo o conteúdo da versão de Switch, aparenta ter um .exe para a criação de novos .dat. Com ele, talvez seja possível criar um só com os arquivos da tradução, evitando ter que extrair as coisas com o GARbro, porém só testarei isso se a tradução foi concluída.
- Há interesse na versão Acta Est Fabula (+18), embora a estrutura dos arquivos na versão inglesa impossibilite a criação de um patch nos mesmos moldes. É possível para a versão japonesa, já que são dois jogos separados, não uma "DLC" que apenas acrescenta um .exe e um novo .dat com o conteúdo adicional.