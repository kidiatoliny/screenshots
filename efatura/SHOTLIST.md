# eFatura Cabo Verde for Node: shot list

Source: the Node.js eFatura Cabo Verde package and its playground in ~/playground
How to shoot: the playground running in a browser window or terminal, against the sandbox only, with demo NIFs and amounts

Screens to capture and their status. Build or open it from an up-to-date main, demo data only, window-only `screencapture` on Retina, never cropped or edited. The post that uses a feature's shots goes in that feature's folder as `post.md` (written by Claude).

- [x] `playground/01-issue-invoice.png`: Issuing a demo invoice from the playground in ~/playground (TEST environment, demo NIF and amounts).
- [x] `playground/02-response.png`: The validation result or generated DFE XML for that invoice.

## Batch 12/12 - 25/12

- [ ] `currency/01-eur-to-cve.png`: the efatura playground (Fastify example or a small script in ~/playground) calling prepareInvoiceToCve() on a demo invoice in EUR, showing the resulting CVE invoice, the original payable amount and the conversion evidence (rate, date, source). Use a fixed provider if the BCV network call isn't reachable, and say so in the commit. Demo data only. NEEDED BY Mon 14/12 20:00
