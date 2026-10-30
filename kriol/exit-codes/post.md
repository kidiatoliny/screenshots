# Kriol: sai(256) já não termina com sucesso

## Text: X

No Kriol, sai(256) terminava com código 0, ou seja, sucesso. O sistema só guarda os 8 bits de baixo do exit status, e sai(-1) dava 255. Agora o compilador recusa um código literal fora de 0 a 255, e um código calculado para o programa com erro.

## Text: Bluesky

No Kriol, sai(256) terminava com código 0, ou seja, sucesso. O sistema só guarda os 8 bits de baixo do exit status, e sai(-1) dava 255. Agora o compilador recusa um código literal fora de 0 a 255, e um código calculado para o programa com erro.

#Kriol #CaboVerde
