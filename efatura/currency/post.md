# efatura: invoices in foreign currency

Planned: X 15/12 18:00, Bluesky 15/12 18:00, LinkedIn 15/12 08:30 (Europe/Luxembourg)

## Text: X

No meu pacote efatura para Node, uma fatura em euros ou dólares fica certa: os valores fiscais do DFE ficam sempre em CVE. O prepareInvoiceToCve() converte com a cotação de compra do BCV e guarda o valor original e a prova da conversão.

## Text: Bluesky

No meu pacote efatura para Node, os valores fiscais do DFE ficam sempre em CVE. O prepareInvoiceToCve() converte uma fatura em euros com a cotação de compra do BCV e guarda o valor original e a prova da conversão.

#NodeJS #TypeScript

## Text: LinkedIn

Faturar em euros em Cabo Verde tem um detalhe: no DFE, os valores fiscais ficam sempre em escudos.

No efatura, o meu pacote Node para a faturação eletrónica de Cabo Verde, o prepareInvoiceToCve() trata disso. Recebe a fatura na moeda de origem, vai buscar a cotação de compra do BCV e devolve uma única fatura em CVE com o valor original a pagar e a prova da conversão.

O BCV é um fornecedor de rede, por isso também há fornecedores fixos e por callback, regras de data e de precisão, e um exemplo offline testado. Está tudo no guia de conversão de moeda.

Quem fatura em moeda estrangeira, como resolve isto hoje?

#NodeJS #TypeScript #CaboVerde

## Screenshots

- `efatura/currency/01-eur-to-cve.png`
