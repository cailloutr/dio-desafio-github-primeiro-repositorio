# Introdução ao Android
Hibrido: escreve um unico codigo e gera duas aplicações; generalização para rodar em duas plataformas, porem impede grande profundidade
Nativo: um unico codigo que gera uma aplciação para um SO especifico permitindo mais aprofundamento na tecnologia

# Kotlin
Declarar variaveis:
var - valor mutavel, camelCase

val - valor imutavel, camelCase (constante)

const val - valor imutavel, SNAKE_CASE

Uma variavel deve ser declarada ou com um valor base, assim o tipo inferido, ou com o tipo declarado junto da variavel

```
  var nome = "Nome"
  
  ou
  
  var nome: String
  nome = "Nome"
  
```
# Operações Aritimeticas
Expressao a + b == a.plus(b)
a += b

# Operadores Logicos
(&&) == (expressao 1) and (expressao 2)
(||) == (expressao 1) or (expressao 2)

In - Verifica se o valor esta presente em uma lista ou faixa de valores
Range - cria um intervalo de valores que inicia no primeiro parametro e acaba no segundo (incluso)

#Funções
fun <nomeDaFuncao>(<nome:Tipo>): TipoRetorno{ }

# Funções de Ordem Superior
Recebem outra função ou lambda por parametro
