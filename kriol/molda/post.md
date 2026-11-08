# Kriol: temporários acima de 1 MiB

Planned: 2026-11-20 08:30 Luxembourg (LinkedIn)

## Text: LinkedIn

Mais uma correção minha no Kriol, a linguagem de programação em crioulo de Cabo Verde.

O Kriol tem um limite de 1 MiB para o que vai para a pilha. Só que esse limite só se aplicava a variáveis locais, parâmetros e arrays devolvidos. Duas coisas escapavam: uma função que devolve uma molda maior do que o limite, e um literal usado como temporário, como g = [1; 1000000]; dentro de uma função.

Qualquer uma punha vários MiB num só frame, e o programa morria com SIGSEGV em vez de falhar a compilar.

Agora o compilador recusa as duas, com uma mensagem em português que diz quantos bytes ocupa o valor e sugere guardá-lo numa variável declarada fora das funções. Inicializações globais grandes continuam a compilar, porque não usam temporário.

#Kriol #CaboVerde #programming

## Screenshots

- `02-temp-too-large.png`
- `03-return-too-large.png`
- `04-large-global.png`

---

# Kriol: temporários acima de 1 MiB

Planned: 2026-11-20 18:00 Luxembourg (X + Bluesky)

## Text: X

No Kriol, um valor temporário grande ia para a pilha sem limite: g = [1; 1000000]; dentro de uma função, ou uma função que devolve uma molda enorme. O programa morria com SIGSEGV. Agora o compilador recusa acima de 1 MiB.

## Text: Bluesky

No Kriol, um valor temporário grande ia para a pilha sem limite: g = [1; 1000000]; dentro de uma função, ou uma função que devolve uma molda enorme. O programa morria com SIGSEGV. Agora o compilador recusa acima de 1 MiB.

#Kriol #CaboVerde

## Screenshots

- `02-temp-too-large.png`
