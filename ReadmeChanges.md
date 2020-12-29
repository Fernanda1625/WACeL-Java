# Clean Code and Refactoring 

#### ScenarioManipulation.java 

En las líneas a continuación se cambio el uso de while por un if, debido al costo computacional que genera la compilación de cada ciclo while:

>Línea 166:

```java
if(matcherTitle.find()) {
  startIndex = matcherTitle.start();
	endIndex = matcherTitle.end();
}
```
>Línea 183:

```java
if(matcherTitle.find()) {
  startIndex = matcherTitle.start();
	endIndex = matcherTitle.end();
}
```   
>Linea 201:

```java
if(matcherTitle.find()) {
  startIndex = matcherTitle.start();
	endIndex = matcherTitle.end();
}
```
>Línea 239:

```java
if(matcherTitle.find()) {
  startIndex = matcherTitle.start();
	endIndex = matcherTitle.end();
}
```

#### OpenNLPAnalyzer.java 

Se agrega un "tokens == null" (para verificar y detener el ciclo for en caso no se encuentren tokens) en la línea 149:
```java
for(int i = 0; i < chunks.length; i++) {
			if (tokens == null){
				break;
			}
			tokens.get(i).setChunkTag(chunks[i].toString());
		}
		//Tokens with Chunk Info
	    return tokens;
```

#### 
