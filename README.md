## 🚨 Detección de fraude en pagos en línea

Construí un sistema que detecta fraude en pagos en línea a partir de patrones reales de transacciones. Responde a una pregunta simple de negocio: ¿dónde se concentran más los fraudes para reforzar primero? 

En mis datos, los casos se reparten casi 50/50 entre CASH_OUT (50.1%) y TRANSFER (49.9%), pero TRANSFER es ~4.2× más riesgoso por transacción (tasa 0.7688% vs 0.1840%). 

Con un modelo de machine learning optimizado por costo, logro capturar ~85.5% del fraude con una tasa de falsos positivos ~0.052%; además, si un equipo revisa solo el 0.5–1% de operaciones con mayor puntaje, detecta ~89–91% de los casos. 

Recomendación práctica: step-up 2FA y checks de velocidad en TRANSFER (por tasa) y OTP/2FA + revisión prioritaria del top-K en CASH_OUT (por volumen).

> Impacto esperado: menos pérdidas y menos fricción para clientes legítimos, enfocando los controles donde realmente ocurren los intentos de fraude.
