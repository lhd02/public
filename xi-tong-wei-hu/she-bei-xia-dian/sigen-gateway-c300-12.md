# Sigen Gateway (C600, C1200, C600-B, C1200-B)

<figure><img src="../../.gitbook/assets/SGA1IN00169-下.png" alt="" width="375"><figcaption></figcaption></figure>

{% include "../../.gitbook/includes/warning.md" %}

<mark style="color:orange;">The Gateway should be disconnected in the following order:</mark>

1. <mark style="color:orange;">Turn off the frame circuit breaker QA3 (connecting to a backup load).</mark>
2. <mark style="color:orange;">Turn off the frame circuit breaker QA2 (connecting to a diesel generator/Smart Load).</mark>
3. <mark style="color:orange;">After shutting down the inverter on the phone, turn off breakers (connecting to inverters).</mark>
   * <mark style="color:orange;">C600 : turn off 2QF1\~2QF30 (miniature circuit breaker)</mark>
   * <mark style="color:orange;">C1200: turn off 2QF1\~2QF50 (miniature circuit breaker)</mark>
   * <mark style="color:orange;">C600-B: turn off 2QF1\~2QF10 (molded case circuit breaker)</mark>
   * <mark style="color:orange;">C1200-B: turn off 2QF1\~2QF20 (molded case circuit breaker)</mark>
4. <mark style="color:orange;">Turn off the frame circuit breaker (connecting to the power grid) QA1.</mark>
5. <mark style="color:orange;">Turn off the surge protective device switch 1QF2, 1QF4 and 1QF6.</mark>
6. <mark style="color:orange;">Turn off the PCB board secondary control switch 1QF1, 1QF3, 1QF5, turn off the secondary control switch of frame circuit breaker 1QF7, 1QF8, 1QF9, 1QF10.</mark>
