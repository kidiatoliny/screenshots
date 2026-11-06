# Kriol: ligação limpa no macOS

Planned: 2026-11-12 18:00 Luxembourg (X + Bluesky)

## Text: X

Mais uma no Kriol: no macOS, cada compilação imprimia umas 21 linhas de avisos do clang e do ld, com o executável certo. O -no-pie não serve no macOS, onde o PIE é obrigatório, e a libgc vinha feita para outra versão do macOS. Agora sai limpa.

## Text: Bluesky

Mais uma no Kriol: no macOS, cada compilação imprimia umas 21 linhas de avisos do clang e do ld, com o executável certo. O -no-pie não serve no macOS, onde o PIE é obrigatório, e a libgc vinha feita para outra versão do macOS. Agora sai limpa.

#Kriol #CaboVerde

## Screenshots

- `05-clean-link.png`

---

# Kriol: ligação limpa no macOS

Planned: 2026-11-17 08:30 Luxembourg (LinkedIn)

## Text: LinkedIn

Mais uma contribuição para o Kriol, a linguagem de programação em crioulo de Cabo Verde.

No macOS arm64, cada compilação imprimia umas 21 linhas de avisos: um do clang e um do ld por cada objeto da libgc. O executável estava certo, mas o ruído era tudo o que se via de uma compilação que funcionava.

Eram duas causas. O -no-pie ia para todos os alvos que não são Windows, mas no macOS o PIE é obrigatório, por isso o clang dizia que o argumento não servia. E a libgc é compilada com a versão de macOS do compilador do build, enquanto a ligação não pedia nenhuma e ficava com a do clang que estivesse no PATH.

Agora o configure guarda a versão com que a libgc foi feita e a ligação pede essa mesma. A versão do SDK não serve: num Mac onde o compilador assume 27, o xcrun diz 27.2.

#Kriol #CaboVerde #macOS

## Screenshots

- `05-clean-link.png`
