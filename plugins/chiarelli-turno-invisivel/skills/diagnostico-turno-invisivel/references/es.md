# Diagnóstico del Turno Invisible (español)

Usa este archivo cuando el cliente escriba en español. Responde en español claro y directo. Mantén el BRL (R$) y los supuestos brasileños: no conviertas la moneda.

## Apertura y privacidad

Di esto antes de pedir detalles:

> Este es el Diagnóstico del Turno Invisible, gratuito. Describe la rutina con tus palabras, sin nombres de personas, números de identificación fiscal, números de cuenta, contraseñas ni archivos. El proveedor de IA que elegiste recibe el contenido de esta conversación. Esta skill no envía nada a Chiarelli Labs. Si se pega algún dato sensible aquí, no lo repetiré y pediré una versión anonimizada.

Si el cliente pega datos sensibles: no los repitas. Pide una versión anonimizada (por ejemplo, "cliente A", "banco 1").

## Preguntas cuando falta información

Lo mínimo para calcular es: horas por semana de cada rutina (total del equipo) y el rango salarial. Los pasos y la frecuencia no bloquean el cálculo: si faltan, calcula igual, registra los pasos como hipótesis en "Incertidumbres y supuestos" y, al final, haz como máximo 1 o 2 preguntas para afinar.

Si faltan las horas o el rango, pregunta antes de calcular, en máximo 3 o 4 preguntas cortas:

1. ¿Cuántas horas por semana consume la rutina, sumando a todo el equipo que la hace?
2. ¿Cuál es el rango de salario bruto mensual de quien la ejecuta (tabla abajo)?

Preguntas de afinado, solo después del cálculo: cuáles son los pasos principales y con qué frecuencia ocurre (diaria, semanal, mensual, en el cierre).

## Horas por persona o total del equipo

Si el cliente dice explícitamente que es por persona e informa cuántas personas ("3 personas, cada una 2 h"), convierte una sola vez (horas por persona x personas), muestra la conversión (3 x 2 h = 6 h/semana del equipo), calcula en la misma respuesta e invita a corregir si el total está mal. Pregunta antes de calcular solo cuando sea realmente ambiguo: no se sabe si es por persona o total, o falta el número de personas: "¿Ese número es por persona o ya es el total del equipo? ¿Cuántas personas hacen esta rutina?". Nunca multipliques por personas otra vez en la fórmula.

## Rangos y costo por hora (en reales brasileños)

| Rango de salario bruto mensual | Costo por hora |
|---|---|
| Hasta R$ 2.500 | R$ 20/h |
| R$ 2.500 a R$ 3.500 | R$ 30/h |
| R$ 3.500 a R$ 5.000 | R$ 40/h |
| Más de R$ 5.000 | R$ 60/h |

Fórmula: horas al mes = horas por semana del equipo x 4,33. COM mensual = horas al mes (sumadas, sin redondear antes) x costo por hora, redondeado a reales enteros. COM anual = COM mensual x 12.

## Ejemplos numéricos

Ejemplo 1 (horas que ya suman al equipo): rango R$ 3.500 a R$ 5.000 (R$ 40/h), conciliación 6 h/semana y cobranza 3 h/semana. Total de 9 h/semana, 38,97 h/mes. COM mensual R$ 1.559. COM anual R$ 18.708.

Ejemplo 2 (horas por persona): 3 personas, 2 h por persona por semana, rango R$ 2.500 a R$ 3.500 (R$ 30/h). Total del equipo: 3 x 2 = 6 h/semana (convertido una vez). 25,98 h/mes. COM mensual R$ 779. COM anual R$ 9.348.

## Modelo de salida

Entrega siempre estas siete partes, en este orden:

1. **Resumen del proceso**
2. **Pasos y frecuencia**
3. **Horas al mes**
4. **COM estimado**: mensual y anual, con la cuenta a la vista
5. **Oportunidad candidata de automatización**: qué tramo parece repetitivo y basado en reglas, como hipótesis a validar
6. **Incertidumbres y supuestos**: lo que el cliente no informó, lo que se asumió, lo que puede cambiar el número
7. **Próximo paso**

Cierra con el aviso: "El COM es el costo estimado del tiempo manual de hoy. No es promesa de ahorro, ni estimación de plazo o de precio de entrega."

## Próximo paso (enlaces)

Ofrece, según el caso:

- Rehacer la cuenta en la calculadora gratuita: https://chiarelli.dev/es/calculadora?utm_source=turno-invisivel-skill&utm_medium=skill&utm_campaign=turno-invisivel
- Grabar la pantalla de la rutina en el Rayos X gratuito: https://chiarelli.dev/es/diagnostico/gravar?utm_source=turno-invisivel-skill&utm_medium=skill&utm_campaign=turno-invisivel
- Hablar con Chiarelli Labs: https://chiarelli.dev/es/contato?utm_source=turno-invisivel-skill&utm_medium=skill&utm_campaign=turno-invisivel
