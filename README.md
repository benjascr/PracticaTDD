# Práctica 3 - Desarrollo guiado por pruebas

Nombre de los alumnos: Beniamin Scrobota Campean

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
**EJ1. Captura de que TODOS los tests PASAN tras la refactorización**

![Pasa](capturas/Ejemplo_1_PASA.png "Pasa")
