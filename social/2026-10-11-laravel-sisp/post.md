# laravel-sisp: SISP (Vinti4) payments in Laravel

Project: `laravel-sisp` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| X | Sun 11 Oct, 11:00 | `6aca0784b07d37ac976968ce` | |
| Bluesky | Sun 11 Oct, 11:00 | `6aca0787b07d37ac97696971` | |
| LinkedIn | Thu 22 Oct, 08:30 | `6aca09fab07d37ac9769c964` | |

Language: Portuguese (Cabo Verde).

## Images

None.

## Text: X, Bluesky

Quem vende online em Cabo Verde mais cedo ou mais tarde tem de integrar a SISP (Vinti4). O laravel-sisp trata disso no Laravel: pagamentos, callbacks com validação de fingerprint, reembolsos, reconciliação e fatura em PDF.

github.com/akira-io/laravel-sisp

## Text: LinkedIn

Se tens uma loja ou um SaaS em Cabo Verde, mais cedo ou mais tarde vais ter de integrar a SISP (Vinti4).

O laravel-sisp é um pacote open source que trata desse fluxo no Laravel:
- pedidos de pagamento e callbacks, com validação de fingerprint
- cancelamentos, novas tentativas e registo de reembolsos
- transações em modelos Eloquent, com logs de auditoria e reconciliação
- fatura em PDF depois do pagamento aprovado
- ferramentas de sandbox para testar

Instala com composer require akira/laravel-sisp e corre php artisan laravel-sisp:install.

Para quem não usa PHP, também existe o node-sisp, para Node.js.

Se já integraste a SISP noutro stack, conta nos comentários como correu.
