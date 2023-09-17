# Dia-da-Ira

Patch com a tradução em português da visual novel Dies Irae ~ Amantes Amentes ~, compatível com a versão inglesa DX package e a versão japonesa em HD -Animation Anniversary-. Possivelmente funcional com a versão Steam (não testado), já a versão japonesa pode não reproduzir algumas vozes (a conferir)

Além de adicionar a tradução, este patch restaura o cursor original do jogo, a música original de menu e a cor original de texto lido, o título original dos capítulos III e VI, nomes oficiais que aparecem entre os capítulos e 4 arquivos de voz faltantes por incompetência da versão inglesa.
Há a possibilidade de trocar a abertura do jogo pela versão de switch, pegando o arquivo na pasta vídeo e substituindo.

Inicialmente, pretendo inserir no script trechos do jogo que traduzi durante os anos de 2017 a 2019.
Posteriormente, continuarei a traduzir o restante.

# Progresso
- Introdução - 1/1 legenda
- Prólogo - 1/1 capítulo
- Rota comum - 6/6 capítulos
- Rota da Kasumi - 1/7 capítulos
- Rota da Kei - 0/7 capítulos
- Rota da Marie - 0/7 capítulos
- Rota da Rea - 4/7 capítulos
- Other Story - 5/5  capítulos

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
- Coloque os quatro arquivos de áudio na pasta equivalente.
# Explicação de como o Patch funciona.

Dentro do arquivo .ini estão instruções para a restauração da música de menu e cor do texto lido, em conformidade com a versão original japonesa.
Dentro da pasta "data" estão todos os arquivos dos data1.dat e data3.dat que você extraiu. Nela você colocará os arquivos do patch também.
A decompilação dos data.dat faz-se necessária pois não há como inserir os arquivos da tradução dentro deles nem criar um novo para substituir, por isso seu conteúdo precisa estar aberto. 


# Tradução

Para traduzir, é necessário extrair o arquivo exec.dat de dentro do data3.dat, localizado na pasta system.
Tendo extraído, utilize o programa StringTool.exe, feito por marcussacana, para converter o script em exec.txt.
Para compilar, utilize novamente o programa StringTool.exe.

É importante que tanto o exec.dat quanto o exec.txt tenham o mesmo número de linhas e estejam na mesma pasta.
Caso o número de linhas não seja igual, o programa não irá compilar.

O script de Dies Irae, da forma como é extraído pelo StringTool, possuí uma peculiaridade: cada palavra em itálico ou sobrescrita (ruby) obrigatoriamente exige estar separada em uma nova linha. 
Devido a diferença no número de linhas, é mais cômodo o uso do script em inglês como base.

Também por causa dessa limitação do número de linhas, você não pode remover itálicos e sobrescritos (embora possa ignorar), tampouco pode adicionar novos itálicos ou sobrescritos, fazendo com que seja refém da suposta tradução em inglês.
O script em inglês possuí um total de 98465 linhas, enquanto o script japonês possuí 118965 linhas. Ao todo são 59812 linhas de texto em si, sendo 53851 linhas únicas.

Para traduzir, é recomendado utilizar o japonês como base, pois a suposta tradução, em muitos momentos assemelhasse a uma fanfic - muitas linhas ignorando parte do japonês ou acrescentando frases que simplesmente não existem, repleto de palavrões incondizentes, engrandecimento da narração e uso de expressões e figuras de linguagem que não combinam com a personalidade dos personagens. Inconsistências na alternância de narração de 1º e 3º pessoa e diversas adaptações idiotas, incluindo linhas que parecem terem sido escritas por crianças de 12 anos. Não há preocupação com uma fidelidade 1:1 para com o texto japonês (seja na pontuação ou estrutura das frases); muitas liberdades "artísticas" que não possuem espaço no campo da tradução profissional.

# Observações

- Até o momento, não é possível traduzir as escolhas nem mudar o nome dos personagens da caixa de texto. O StringTool não extrai esta parte do script, embora o MalieVM supostamente consegue (eu que não consigo utilizá-lo).
- Os nomes na caixa e na tradução podem variar, pois a tradução segue a grafia oficial, enquanto a suposta tradução em inglês mudou boa parte deles.
- Outro problema desta versão é que o texto é justificado, o que gera um kerning ruim e atrapalha a leitura. Infelizmente não há solução para isso.
- Caso queira mudar a fonte do jogo, pegue outra fonte .otf (qualquer fonte, na verdade, basta mudar a extensão para .otf) e coloque na pasta "data/font" renomeando ela com o nome da antic.
- Entre a versão DX, a versão Steam e a versão japonesa de Aniversário, recomenda-se a primeira, embora a versão japonesa tenha a possibilidade de alterar a resolução entre 16:9 e 4:3. A versão Steam simplesmente não foi testada, mas deve funcionar se a estrutura de arquivos for a mesma.
- Extraindo o conteúdo da versão de Switch, aparenta ter um .exe para a criação de novos .dat. Com ele, talvez seja possível criar um só com os arquivos da tradução, evitando ter que extrair as coisas com o GARbro, porém só testarei isso se a tradução foi concluída.
- Possivelmente por questões de incompetência, algumas poucas linhas do japonês não existem na suposta tradução em inglês. Restaurá-las é impossível na maioria das vezes pois implicaria em adicionar novas linhas no script, mas fazendo isso a compilação quebra.
- Há interesse na versão Acta Est Fabula (+18), embora a estrutura dos arquivos na versão inglesa impossibilite a criação de um patch nos mesmos moldes. É possível para a versão japonesa, já que são dois jogos separados, não uma "DLC" que apenas acrescenta um .exe e um novo .dat com o conteúdo adicional.