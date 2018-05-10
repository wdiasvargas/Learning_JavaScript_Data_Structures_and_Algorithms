# Functions of the equals operators ( == and ===)
Os dois operadores suportados por Javascript podem causar uma pequena confusao quando trabalhamos com them.
Quando usamos `==`, valores podem ser considerados `equal` iguais quando eles sao diferentes tipos. Isso pode ser confuso even para um Desenvolvedor Senior Javascript.
Let's analizar como `==` trabalha usando a tabela seguinte:

| Type(x)        | Type(y)          | Result  |
| ------------- |:-------------:| -----:|
| `null`|`undefined`|`true` |
| `undefined`|`null`|`true` |
| `Number`|`String`|`x== toNumber(y)`|
| `String`|`Number`|`toNumber(x) == y`|
| `Boolean`|`Any`|`toNumber(x) == y`|
| `Any`|`Boolean`|`x == toNumber(y)`|
| `String or Number`|`Object`|`x == toPrimitive(y)`|
| `String or Number`|`Object`|`x == toPrimitive(x) == y`|

Se `x` e `y` sao do mesmo tipo, quando Javascript vai usar o metodo `equals`
para comparar os dois valores ou objetos. Any outros combinações que não é listado na tabela gives um resultado `false`.
O `toNumber` e `toPrimitive` sao metodos internos e avaliam  de acordo com a tabela seguinte
O `toNumber` metodo é como segue:

| Type(x)       | Type(y)		|
| ------------- |:-------------:|
| `undefined`	|This is `NaN`	|
|`Boolean`		|Se o valor é `true`, o resultado é 1;
se o valor é `false`, o resultado é `+0`	|
|`Number`		|is o valor de numero	|
Finalmente, `toPrimitive` é como segue: