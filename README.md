# Práctica 3 - Desarrollo guiado por pruebas

Nombre del alumno: Beniamin Scrobota Campean

### Ejemplo 1

**INPUT y OUTPUT**: "1" -> 1

**EJ1. Código de test**
```java
@Test
void parseSingleDigitNumber() {
    assertEquals(1, calculatorParser.parse("1"));
}
```

**EJ1. Mensaje del test añadido que NO PASA**

```log
java.lang.UnsupportedOperationException: Not implemented yet
```

**EJ1. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java
public int parse(String expression) {
    return 1;
}
```

**EJ1. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

### Ejemplo 2

**INPUT y OUTPUT**: "2" -> 2

**EJ2. Código de test**
```java
@Test
void parseSingleDigitNumber2() {
    assertEquals(2, calculatorParser.parse("2"));
}
```

**EJ2. Mensaje del test añadido que NO PASA**

```log
org.opentest4j.AssertionFailedError: expected: <2> but was: <1>
```

**EJ2. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java
public int parse(String expression) {
    if (expression.equals("1")) {
        return 1;
    }
    return 2;
}
```

**EJ2. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

### Ejemplo 3

**INPUT y OUTPUT**: "3" -> 3

**EJ3. Código de test**
```java
@Test
void parseSingleDigitNumber2() {
    assertEquals(3, calculatorParser.parse("3"));
}
```

**EJ3. Mensaje del test añadido que NO PASA**

```log
org.opentest4j.AssertionFailedError: expected: <3> but was: <2>
```

**EJ3. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java
public int parse(String expression) {
	if (expression.equals("1")) {
		return 1;
	}
	if (expression.equals("2")) {
	        return 2;
	}
	return 3;
}
```

**EJ3. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

**EJ3. Refactorización**

Justificar vuestra refactorización aquí.

```java
public int parse(String expression) {
	return Integer.parseInt(expression);
}
```
**EJ3. Captura de que TODOS los tests PASAN tras la refactorización**

![Pasa](capturas/Ejemplo_1_PASA.png "Pasa")

### Ejemplo 4

**INPUT y OUTPUT**: "1 + 1" -> 2

**EJ4. Código de test**

```java
@Test
void parseSimpleAddition1() {
    assertEquals(2, calculatorParser.parse("1 + 1"));
}
```

**EJ4. Mensaje del test añadido que NO PASA**

```log
java.lang.NumberFormatException: For input string: "1 + 1"
```

**EJ4. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java
public int parse(String expression) {
	if(expression.length() > 1) {
		String[] splittedExpression = expression.split(" ");
		return Integer.parseInt(splittedExpression[0]) + Integer.parseInt(splittedExpression[2]);
	}
	return Integer.parseInt(expression);
}
```

**EJ4. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

**EJ4. Refactorización**

Justificar vuestra refactorización aquí.

```java

```
**EJ4. Captura de que TODOS los tests PASAN tras la refactorización**

![Pasa](capturas/Ejemplo_1_PASA.png "Pasa")

### Ejemplo 5

**INPUT y OUTPUT**: "2 + 3" -> 5

**EJ5. Código de test**

```java

```

**EJ5. Mensaje del test añadido que NO PASA**

```log

```

**EJ5. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java

```

**EJ5. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

**EJ5. Refactorización**

Justificar vuestra refactorización aquí.

```java

```
**EJ5. Captura de que TODOS los tests PASAN tras la refactorización**

![Pasa](capturas/Ejemplo_1_PASA.png "Pasa")

### Ejemplo 6

**INPUT y OUTPUT**: "2 + 3 + 4" -> 9

**EJ6. Código de test**

```java

```

**EJ6. Mensaje del test añadido que NO PASA**

```log

```

**EJ6. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java

```

**EJ6. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

**EJ6. Refactorización**

Justificar vuestra refactorización aquí.

```java

```
**EJ6. Captura de que TODOS los tests PASAN tras la refactorización**

![Pasa](capturas/Ejemplo_1_PASA.png "Pasa")

### Ejemplo 7

**INPUT y OUTPUT**: "1 + 2 + 3 + 4" -> 10

**EJ7. Código de test**

```java

```

**EJ7. Mensaje del test añadido que NO PASA**

```log

```

**EJ7. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java

```

**EJ7. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

**EJ7. Refactorización**

Justificar vuestra refactorización aquí.

```java

```
**EJ7. Captura de que TODOS los tests PASAN tras la refactorización**

![Pasa](capturas/Ejemplo_1_PASA.png "Pasa")

### Ejemplo 8

**INPUT y OUTPUT**: "A" -> Invalid expression

**EJ8. Código de test**

```java

```

**EJ8. Mensaje del test añadido que NO PASA**

```log

```

**EJ8. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java

```

**EJ8. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

**EJ8. Refactorización**

Justificar vuestra refactorización aquí.

```java

```
**EJ8. Captura de que TODOS los tests PASAN tras la refactorización**

![Pasa](capturas/Ejemplo_1_PASA.png "Pasa")

### Ejemplo 9

**INPUT y OUTPUT**: "B" -> Invalid expression

**EJ9. Código de test**

```java

```

**EJ9. Mensaje del test añadido que NO PASA**

```log

```

**EJ9. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java

```

**EJ9. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

**EJ9. Refactorización**

Justificar vuestra refactorización aquí.

```java

```
**EJ9. Captura de que TODOS los tests PASAN tras la refactorización**

![Pasa](capturas/Ejemplo_1_PASA.png "Pasa")

### Ejemplo 10

**INPUT y OUTPUT**: "k" -> Invalid expression

**EJ1. Código de test**

```java

```

**EJ10. Mensaje del test añadido que NO PASA**

```log

```

**EJ10. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java

```

**EJ10. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

**EJ10. Refactorización**

Justificar vuestra refactorización aquí.

```java

```
**EJ10. Captura de que TODOS los tests PASAN tras la refactorización**

![Pasa](capturas/Ejemplo_1_PASA.png "Pasa")

### Ejemplo 11

**INPUT y OUTPUT**: "HoLa" -> Invalid expression

**EJ11. Código de test**

```java

```

**EJ11. Mensaje del test añadido que NO PASA**

```log

```

**EJ11. Código mínimo para que el test pase**

Describe brevemente el código mínimo implementado

```java

```

**EJ11. Captura de que TODOS los test PASAN**

AÑADIR CAPTURA

**EJ11. Refactorización**

Justificar vuestra refactorización aquí.

```java

```
**EJ11. Captura de que TODOS los tests PASAN tras la refactorización**

![Pasa](capturas/Ejemplo_1_PASA.png "Pasa")
