---
id: trading-como
title: Cómo Hacer Trading Usando Sintéticos
sidebar_label: Cómo Hacer Trading Usando Sintéticos
---

## Accediendo al Ecosistema
Hay tres formas sencillas de adquirir los activos que necesita para operar en la <a href="https://synthetix.exchange/" target="_blank" class="link">Plataforma de Intercambio de Synthetix</a> o <a href="https://synthetix.exchange/" target="_blank" class="link">Synthetix Exchange</a>:
- <a href="/docs/staking-snx-overview" class="link">Bloquee (Stake) SNX</a> y acuñe sUSD
- Use Uniswap para intercambiar ETH por sETH
- Utilice el servicio ubicado en el panel izquierdo de la Plataforma para intercambiar ETH por sUSD

## Ejecutando una Operación (Trade)
La interfaz será actualizada mostrando su balance para cada activo sintético. De momento, hasta Noviembre de 2019 hay ~25 activos soportados, pero hay planes de incluir una cantidad significativamente mayor. Algunos son activos "de posición larga" por protocolo, como sETH y sBTC, aparejados con uno "de posición corta" o "inverso". Algunos son tokens de Ethereum - de nuevo, aparejados con una versión "de posición corta" o "inversa" - y algunos son divisas fiduciarias globales. El equipo ha introducido también cestas de activos sintéticos, con pares "cortos"/"largos" de una cesta de tokens de Casas de Cambio (Exchanges) centralizadas y una cesta de finanzas descentralizadas que pronto estará también disponible.

Los operadores pueden ejecutar una transacción seleccionando un activo de entrada, un activo de salida y una cantidad determinada. Las comisiones por operación son el 0.3% del valor de la transacción.

> Recientemente las comisiones han sido ajustadas a 0.5% en algunas ocasiones, con el objetivo de reducir la rentabilidad de los bots de ejecución anticipada (front-running)

Para las operaciones en las que se intercambian un activo "de posición larga" por un activo "inverso" (por ejemplo, sETH por iBTC), la comisión es duplicada. Un punto de especial importancia, es el hecho de que no hay deslizamientos de precio (slippage). Al momento de la ejecución, el precio al contado (spot price) por cada sETH será el mismo, tanto si está comerciando solo 1 sETH, como si está comerciando 100 sETH. 

La interfaz de usuario de la Plataforma permite al operador escoger entre una variedad de velocidades de transacción. Más allá de la confirmación de la velocidad de transacción, seleccionar un valor de gas más lento o más rápido no afectará a la operación en sí. Sin embargo, si la red está altamente congestionada, la operación podría fallar si el token ya no se encuentra disponible al mismo precio.
