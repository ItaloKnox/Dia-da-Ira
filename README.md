# Dia-da-Ira

Patch com a tradução em português da visual novel Dies Irae ~ Amantes Amentes ~. 
Compatível com a versão inglesa DX package e a versão Steam. Funciona também com a versão japonesa em HD -Animation Anniversary-, embora não recomendada.

Além de adicionar a tradução, este patch restaura o **cursor original**, a **música original de menu**, a **cor original** de texto lido, o **título original** dos capítulos **III e VI**, **nomes oficiais** entre capítulos e **arquivos de voz faltantes ou censurados**.
Existe a possibilidade de trocar a abertura do jogo pela versão de switch, pegando o arquivo na pasta vídeo e substituindo.

# Progresso
- Introdução - 1/1 legenda
- Prólogo - 1/1 capítulo
- Rota comum - 6/6 capítulos
- Rota da Kasumi - 6/7 capítulos
- Rota da Kei - 1/7 capítulos
- Rota da Marie - 0/7 capítulos
- Rota da Rea - 6/7 capítulos
- Other Story - 5/5  capítulos
Ao todo são 59812 linhas de texto em si, sendo 53851 linhas únicas.

# Instalação
- Baixe o programa [GARbro](https://github.com/morkt/GARbro/releases/tag/v1.5.44)
- Utilize-o para extrair o conteúdo dos arquivos ```data1.dat``` e ```data3.dat``` na versão DX. Na versão japonesa, apenas o  ```data1.dat```.
- Você obterá uma pasta ```data``` com várias subpastas.
- Delete ```data1.dat``` e ```data3.dat``` se estiver com a versão DX. Delete apenas ```data1.dat``` se estiver com a versão japonesa.
- Se abrir normalmente, esta etapa foi um sucesso.

(Esse processo é necessário para que não seja preciso literalmente compartilhar 90% do conteúdo do jogo, em um patch de aproximadamente 8GB e mais de 100 mil arquivos)

- Agora baixe o patch disponível [aqui](https://github.com/Monaco-a-Knox/Dia-da-Ira/releases) no Github.
- Coloque o arquivo ```malie.ini``` na pasta raiz do jogo, substituindo o já existente.
- Pegue o conteúdo da pasta ```data``` que você baixou com o patch e o distribua nas subpastas correspondentes da sua pasta ```data```, substituindo os arquivos já existentes.
- Na pasta ```data/picture/event/dead```, delete os .dzi e substitua pelos .png.
- Coloque os arquivos de áudio nas pastas equivalente.

# Explicação de como o Patch funciona.

Dentro do arquivo ```.ini``` estão instruções para a restauração da música de menu e cor do texto lido, em conformidade com a versão original japonesa.
Dentro da pasta "data" estão todos os arquivos dos ```data1.dat``` e ```data3.dat``` que você extraiu. Nela você colocará os arquivos do patch também.
A decompilação dos data.dat faz-se necessária pois não há como inserir os arquivos da tradução dentro deles nem criar um novo para substituir, por isso seu conteúdo precisa estar aberto. 


# Tradução

Para traduzir, é necessário extrair o arquivo ```exec.dat``` de dentro do ```data3.dat```, localizado na pasta ```system```, utilizando o GARbro.
Tendo extraído, utilize o programa StringTool, criado por [marcussacana](https://github.com/marcussacana/SacanaWrapper), para converter o script em exec.txt.
Para compilar, utilize novamente o programa StringTool.exe.
É importante que tanto o ```exec.dat``` quanto o ```exec.txt``` **tenham o mesmo número de linhas e estejam na mesma pasta**.
Caso o número de linhas não seja igual, o programa não irá compilar.

Para traduzir as escolhas e nomes na caixa de texto, utilize Malie_Script_Tool, criado por [Crsky](https://github.com/crskycode/Malie_Script_Tool), para converter o script em ```exec.msg.txt``` e ```exec.str.txt```
Para usá-lo, é necessário compilá-lo com o Visual Studio. O programa possui um bug, então é necessário compilá-lo duas vezes. Uma para criar uma versão específica para decompilar. Em seguida, delete as linhas 19 e 22 em ```Program.cs``` e compile novamente para criar uma versão de compilação.

O script de Dies Irae, da forma como é extraído pelo StringTool, possuí uma peculiaridade: cada palavra em itálico ou sobrescrita (ruby) obrigatoriamente exige estar separada em uma nova linha. 
Devido a diferença no número de linhas, não é recomendado para se trabalhar com o script japonês (embora não seja impossível).
Por causa da limitação do número de linhas, você não pode remover itálicos e rubys (embora possa ignorar), tampouco pode adicionar novos itálicos ou ruby, fazendo com que seja refém do texto.

Extraindo com o Malie_Script_Tool, o problema de itálicos e rubys é corrigido. No entanto, o programa extrai o texto duplicado (apenas a segunda linha importa). O ideal é utilizá-lo apenas para traduções do japonês ou para fazer edições, adicionando itálicos, rubys e quebras de linha.

A tradução inglesa de Dies Irae, embora oficial, é de procedência duvidosa. Muitas linhas "americanizadas", infinitos palavrões desnecessários, frases incompletas, linhas reescritas ao ponto de parecer uma fanfic, inconsistências narrativas entre 1º e 3º pessoa e diversos erros de tradução. Por isso, trabalhar conjuntamente ao script japonês lado a lado torna-se imprescindível.

# Censura

Como você deve saber, a versão japonesa de Amantes Amantes, lançada para computar, é baseada na versão de PSP. Todo eroge lançado para console sofre censura, tanto visual quanto textual, muito além de meramente remover as cenas de sexo.
Sendo assim, acaba por ser **obrigatório usar o script inglês como base para a tradução**, isso porque ele **restaurou** grande parte das linhas originais da versão Acta Est Fabula, tanto as linhas reescrita quanto as linhas que foram removidas.
Contudo, a versão inglesa não restaurou 100% dessas linhas. Tudo o que eu pude restaurar em conformidada ao jogo original, eu restaurei, incluído no patch os respectivos arquivos de voz originais. Infelizmente três linhas (v_ma3009, v_vi0267 e v_sy2162) não podem ser restauradas porque foram removidas. Adicionar qualquer linha extra quebra o atual processo de compilação.

A versão inglesa também optou por não restaurar algumas artes sem censura. Neste patch, pretendo restaurá-las. (No momento, a substituição de imagens está apresentando problema de resolução)

# Observações

- Caso queira mudar a fonte do jogo, pegue outra fonte .otf (qualquer fonte, na verdade, basta mudar a extensão para .otf) e coloque na pasta "data/font" renomeando ela com o nome da antic.
- Extraindo o conteúdo da versão de [Switch](https://github.com/masagrator/DiesIraeScenario), aparenta ter um .exe para a criação de novos .dat. Com ele, talvez seja possível criar um só com os arquivos da tradução, evitando ter que extrair as coisas com o GARbro, porém só testarei isso se a tradução foi concluída.
- Há interesse na versão Acta Est Fabula (+18), porém a estrutura da versão Steam/DX impede a criação de um patch.