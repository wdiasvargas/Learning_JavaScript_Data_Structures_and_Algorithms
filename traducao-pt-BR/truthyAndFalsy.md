Verdadeiro e Falso

Em javascript verdadeiro e false são pequenos bit tricky.
Em muitas linguagens, os valores boleanos true e false representam o verdadeiro/falso resultado.
Em Javascript, uma string such as Packt avaliado como verdadeiro.
Na tabela seguinte podemos ajudar a entender melhor como true e false funcionam em Javascript:
Tipo de Valor -> Resultado
undefined -> false
null -> false
Boolean -> true é verdadeiro e false é false
Numero -> o resultado false para +0, -0 ou NaN; otherwise, o resultado é true
String -> O resultado é false se a string é vazia (tamanho é 0); otherwise, o resultado é

true(length >= 1)
Objeto -> true

Vamos considerar alguns exemplos e verificar sua saída

function testeVerdadeiro(valor){
    return valor ? console.log('verdadeiro') : console.log('falso');
}

//ES6
//const testeVerdadeiro = valor => valor ? console.log('verdadeiro) : console.log('falso')

Verdadeiro e Falso

Em javascript verdadeiro e false sao pequenos bit tricky.
Em muitas linguagens, os valores boleanos true e false representao o verdadeiro/falso resutado.
Em Javascript, uma string suche as Packt avaliado como verdadeiro.
Na tabela seguinte podemos ajudar a entender melhor como true e false funcionam em Javascript:
Tipo de Valor -> Resultado
undefined -> false
null -> false
Boolean -> true é verdadeiro e false é false
Numero -> o resultado false para +0, -0 ou NaN; otherwise, o resultado é true
String -> O resultado é false se a string pe vazia (tamanho é 0); otherwise, o resultado é

true(length >= 1)
Objeto -> true

Vamos considerar alguns exemplos e verificar sua saida

function testeVerdadeiro(valor){
    return valor ? console.log('verdadeiro') : console.log('falso');
}

const testeVerdadeiro = valor => valor ? console.log('verdadeiro) : console.log('falso')

Verdadeiro e Falso

Em javascript verdadeiro e false sao pequenos bit tricky.
Em muitas linguagens, os valores boleanos true e false representao o verdadeiro/falso resutado.
Em Javascript, uma string suche as Packt avaliado como verdadeiro.
Na tabela seguinte podemos ajudar a entender melhor como true e false funcionam em Javascript:
Tipo de Valor -> Resultado
undefined -> false
null -> false
Boolean -> true é verdadeiro e false é false
Numero -> o resultado false para +0, -0 ou NaN; otherwise, o resultado é true
String -> O resultado é false se a string pe vazia (tamanho é 0); otherwise, o resultado é

true(length >= 1)
Objeto -> true

Vamos considerar alguns exemplos e verificar sua saida

function testeVerdadeiro(valor){
    return valor ? console.log('verdadeiro') : console.log('falso');
}

const testeVerdadeiro = valor => valor ? console.log('verdadeiro) : console.log('falso')

Verdadeiro e Falso

Em javascript verdadeiro e false sao pequenos bit tricky.
Em muitas linguagens, os valores boleanos true e false representao o verdadeiro/falso resutado.
Em Javascript, uma string suche as Packt avaliado como verdadeiro.
Na tabela seguinte podemos ajudar a entender melhor como true e false funcionam em Javascript:
Tipo de Valor -> Resultado
undefined -> false
null -> false
Boolean -> true é verdadeiro e false é false
Numero -> o resultado false para +0, -0 ou NaN; otherwise, o resultado é true
String -> O resultado é false se a string pe vazia (tamanho é 0); otherwise, o resultado é

true(length >= 1)
Objeto -> true

Vamos considerar alguns exemplos e verificar sua saida

function testeVerdadeiro(valor){
    return valor ? console.log('verdadeiro') : console.log('falso');
}

const testeVerdadeiro = valor => valor ? console.log('verdadeiro) : console.log('falso')

testeVerdadeiro(true)//true
testeVerdadeiro(false)//false
testeVerdadeiro(new Boolean(false)) // true(objeto é always true)

testeVerdadeiro('')//false
testeVerdadeiro('Packt')//true
testeVerdadeiro(new String('')); // true(objeto é always true)

testeVerdadeiro(1); //true
testeVerdadeiro(-1);//true
testeVerdadeiro(NaN) //false
testeVerdadeiro(new Number(NaN))//true Objeto é always true

testeVerdadeiro({});//true (object is always true)

var obj = { name: 'Jhon' };
testeVerdadeiro(obj); //true
testeVerdadeiro(obj.name); // true
testeVerdadeiro(obj.age); //age(propriedade não existe)


