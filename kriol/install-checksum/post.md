# Kriol: o instalador passa a verificar o SHA256

## Text: X

Mais uma contribuição para o Kriol: o install.sh descarregava o compilador e instalava-o sem verificar nada. Agora compara o SHA256 do arquivo com o SHA256SUMS.txt da mesma release e para antes de extrair se não bater, se faltar a entrada ou se a release não tiver o ficheiro.

## Text: Bluesky

Mais uma contribuição para o Kriol: o install.sh descarregava o compilador e instalava-o sem verificar nada. Agora compara o SHA256 do arquivo com o SHA256SUMS.txt da mesma release e para antes de extrair se não bater, se faltar a entrada ou se a release não tiver o ficheiro.

#Kriol #CaboVerde

## Text: LinkedIn

Esta semana contribuí para o Kriol com coisas que ninguém vê mas que contam: a segurança do caminho por onde o compilador chega ao teu computador.

O install.sh descarregava o arquivo da release e extraía-o sem verificar nada. Um download cortado ou trocado era instalado sem aviso. Agora compara o SHA256 com o SHA256SUMS.txt da mesma release e para antes de extrair se algo não bater.

No CI, as GitHub Actions passam a ser referidas pelo SHA do commit em vez da tag, e os arquivos LLVM e llvm-mingw do build de Windows só são extraídos se o SHA256 for o esperado. O runtime do MinGW é ligado a todos os programas, por isso um arquivo adulterado chegaria ao produto distribuído.

Corrigi também um detalhe curioso: sai(256) terminava com código 0, sucesso, porque o sistema só guarda os 8 bits de baixo do exit status.

O Kriol é uma linguagem de programação baseada no crioulo de Cabo Verde, criada pelo Anaxímeno Brito.

#Kriol #CaboVerde #segurança
