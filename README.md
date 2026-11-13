# Trena → Planta

App web (Chrome no Android) que conecta na trena a laser **Huepar S120-G-BT** por Bluetooth e organiza o levantamento em **Lote → Área → Cômodo → Porta/Janela**. Cada leitura da trena cai direto na medida selecionada (linha verde) e o app avança sozinho para a próxima.

- Sem conta, sem servidor: os dados ficam no celular até você tocar em **☰ → Enviar ao GitHub**.
- O envio grava `dados/levantamento.json` e `dados/levantamento.md` no repositório **privado** `levantamento-casa`.
- Protocolo BLE: serviço `0xAE30`, comando em `0xAE01`, leituras em `0xAE02` (documentação independente em s120.supported.systems).

Se uma leitura não aparecer, abra **☰ → Ver log da trena**, copie e mande para o Claude.
