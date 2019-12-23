---
id: pool-de-arbitrage
title: Poolde Arbitraje
sidebar_label: Pool de Arbitraje
---

## Visión General

Junto con los <a href="/docs/seth-pool" class="link">incentivos de la pool de liquidez ETH/sETH</a>, el contrato de arbitraje está diseñado para reforzar la paridad ETH/sETH, asegurando a los traders acceso on ramp y off ramp limpio y económico entre el colateral y los sintéticos.
El contrato es externo a la pool de liquidez de Uniswap, pero enruta y realiza transacciones a través de la misma. Cuando la relación sETH a ETH cae por debajo de 0.99, los usuarios pueden enviar ETH al contrato, el cual convertirá primero ETH a sETH y después sETH a SNX. El modelo de producto constante de Uniswap fuerza a que el precio de sETH se eleve cuando la demanda relativa es alta, por lo que esta transacción múltiple sirve para reforzar la paridad.

Puede leer más sobre el contrato de arbitraje aquí: <a href="https://blog.synthetix.io/our-new-seth-snx-arb-contract-is-now-live/" class="link" target="_blank">Our new ETH-SNX arb contract is now live!</a>

## Pasos Básicos

- Diríjase a <a href="https://etherscan.io/dapp/0xa6b5e74466edc95d0b6e65c5cbfca0a676d893a4#writeContract" class="link" target="_blank">Etherscan Dapp</a>

- Conecte su navegador Web3 (vértice superior derecho)
- Click en "contract address" (vértice superior izquierdo) y asegúrese que el contrato tenga un balance positivo en SNX. Cada semana se depositan nuevos tokens en el contrato, pero a veces las reservas se consumen antes. Regrese a la Dapp
- Click `arbSynthRate` (#13) e ingrese la cantidad de ETH a enviar
- Confirme la transacción       

## Cálculo de Incentivos
Synthetix asigna 5% de la infalción semanal al contrato de arbitraje. A partir deNOviembre 2019, se distribuyen 72.000 SNX semanales, pero esta cantidad disminuirá gradualmente según la agenda de inflación progresa. Una vez el contrato se vacía, no es recargado con nuevos tokens hasta la siguiente semana.