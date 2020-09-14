---
id: reclamando-ganancias
title: Reclamando Ganancias
sidebar_label: Reclamando Ganancias
---

## Pasos Básicos
- Las ganancias son calculadas y habilitadas una vez cada semana, específicamente los Miércoles.
- Use <a class="link" target="_blank" href="https://beta.mintr.synthetix.io/">Mintr</a> para navegar a la sección de Reclamación (`Claim`).
- Asegúrese de que su ratio de colateralización (`C-RATIO`) es suficiente para reclamar: es requerido un 600%, pero si está en un rango del 1% (sobre 594%, por ejemplo), no tendrá problemas para realizar su petición. En caso contrario, usted tendrá que <a href="/docs/buying-snx" class="link"> comprar más SNX</a> o <a href="/docs/transferring-snx#burning-susd" class="link">quemar sUSD</a> para restablecer su `C-RATIO`.
- Presione `Claim Now` para cobrar su ganancia semanal, tanto en sUSD como en SNX.
- Usted debe realizar al menos una reclamación cada dos semanas. De no hacerlo, sus ganancias serán devueltas al fondo de recompensas común al término de dicho plazo.
- Los SNX reclamados como ganancia son mantenidos en custodia (`escrowed`) por un año. Usted no podrá transferirlos o venderlos durante ese periódo.


## Gestionando la Deuda
Su `C-RATIO` puede cambiar sin la acción directa de usted. Puede encontrar aquí una <a href="https://help.synthetix.io/hc/en-us/articles/360023174973-Why-does-my-total-sUSD-debt-fluctuate-over-time-" target="_blank" class="link">explicación detallada</a> sobre los motivos que pueden provocar la fluctuación de la deuda global en el tiempo. Básicamente, la deuda global - y su parte en términos de proporción - aumentará si los comerciantes que operan en la Plataforma de Intercambio de Synthetix son rentables en general y disminuirá en caso contrario.

Para Noviembre de 2019, la gran mayoría de operadores en Synthetix están "largos" en `sETH` y `sBTC`, synthetic, ether y bitcoin. En una sección llamada `Synths Distribution` que puede consultar a través del <a href="https://dashboard.synthetix.io/" class="link" target="_blank">Synthetix Dashboard</a> usted tendrá acceso a los datos actualizados relativos al posicionamiento de los operadores. 

Una estrategia común para mantener el `C-RATIO` relativamente estable es usar el sUSD que ha sido "acuñado" por usted para reflejar el posicionamiento global de los operadores. Su deuda será incrementada si el portafolio tiene un buen desempeño, pero su valor sintético aumentará a un ritmo constante, protegiendo su `C-RATIO`.

Si un participante (staker) "imprime" sUSD y no los intercambia, está efectivamente "vendiendo en corto" el portafolio global, porque queda expuesto a un crecimiento en la deuda global sin un incremento potencial del sintético en cartera (synth holdings). No hay nada malo con esta forma de posicionamiento frente al mercado, pero algunos participantes inexpertos no han caído en la cuenta de los riesgos que esto podría implicar.

<a href="https://www.delphidigital.io/research" target="_blank" class="link">Delphi Research</a> reúne una serie de ejemplos detallados sobre las mecánicas del sistema de deuda en su reporte sobre SNX (Acceso a través de pago). Puede ver uno a continuación:

<img src="assets/debt-example.png" width="50%">


## ¿Cómo son calculadas las ganancias?
Existen dos componentes que son utilizados como recompensa: sUSD y SNX.

Cuando un operador ejecuta una transacción en la Plataforma de Intercambio de Synthetix, paga una comisión del 0.3%. Estas comisiones son distribuidas de manera proporcional entre todos los participantes (stakers).

Mientras más sUSD usted haya "acuñado", mayor será la proporción de comisiones que reciba.

Las ganancias globales distribuidas en SNX están determinadas por el calendario de inflación del token. En Noviembre de 2019, el 90% de la inflación semanal es asignada a las recompensas por participación (staking). Si desea consultar con más detalle la política monetaria de Synthetix puede hacerlo <a class="link" target="_blank" href="https://blog.synthetix.io/synthetix-monetary-policy-changes/">aquí</a>. 

Si usted se encuentra por debajo del `C-RATIO` necesario no será penalizado, solo no tendrá permitido reclamar sus ganancias.

Su proporción de deuda global es calculada basada en una captura (`snapshot`) de la red tomada cada Miércoles aproximadamente a las 09:00 UTC.

## Calculando Rendimientos
Los rendimientos son una función del volumen de la Plataforma de Intercambio de Synthetix, el calendario de inflación actual y la proporción individual de participación (staking) con respecto a la deuda global emitida. <a href="https://www.stakingrewards.com/asset/synthetix-network-token" class="link" target="_blank">Staking Rewards</a> brinda una aproximación del rendimiento estimado para SNX, sin embargo, puede no incluir el valor de los rendimientos para sUSD.

