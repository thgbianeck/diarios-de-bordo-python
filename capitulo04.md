# Capítulo 4: Variáveis no Python

## Diário de Bordo

**Data Estelar 42001.5**
**Entrada da Capitã T'Pral Bieniek**

Explorar as variáveis no Python é como descobrir novos planetas em nossa jornada pela galáxia. Cada variável é um recipiente que guarda dados valiosos, assim como cada planeta pode esconder recursos preciosos. Cadetes, preparem-se para aprender a manipular esses recipientes de dados com a precisão e a lógica que esta missão exige.

---

## Introdução às Variáveis

### O que são Variáveis?

Variáveis são contêineres para armazenar valores de dados. Em Python, não é necessário declarar uma variável com um comando específico; ela é criada no momento em que você atribui um valor a ela[^1]. Pense nas variáveis como compartimentos na nave estelar U.S.S. Pythonrise, cada um armazenando um item específico que pode ser utilizado a qualquer momento.

Por exemplo:

```python
x = 5
y = "John"
print(x)
print(y)
```

Neste exemplo, x é uma variável que armazena o valor 5 e y armazena a string "John".

### Mudança de Tipo

Em Python, as variáveis não precisam ser declaradas com um tipo específico e podem mudar de tipo após terem sido definidas[^2]. Isso é como um compartimento modular na nave que pode armazenar diferentes tipos de suprimentos conforme necessário.

```python
x = 4  # x é do tipo int
x = "Sally"  # x agora é do tipo str
print(x)
```

### Casting

Se você quiser especificar o tipo de dado de uma variável, isso pode ser feito com o casting[^3]. Imagine que você está ajustando a configuração de um compartimento para armazenar um tipo específico de material.

```python
x = str(3)    # x será '3'
y = int(3)    # y será 3
z = float(3)  # z será 3.0
```

### Obtendo o Tipo

Você pode obter o tipo de uma variável usando a função type()[^4]. Isso é semelhante a usar um scanner para verificar o conteúdo de um compartimento na nave.

```python
x = 5
y = "John"
print(type(x))
print(type(y))
```

### Aspas Simples ou Duplas?

Variáveis de string podem ser declaradas usando aspas simples ou duplas[^5]. É como ter diferentes chaves para abrir o mesmo compartimento.

```python
x = "John"
# é o mesmo que
x = 'John'
```

### Sensibilidade a Maiúsculas e Minúsculas

Os nomes de variáveis são sensíveis a maiúsculas e minúsculas[^6]. Assim como os códigos de acesso na nave, onde "ALPHA" e "alpha" seriam reconhecidos como diferentes.

```python
a = 4
A = "Sally"
# A não sobrescreverá a
```

## Nomes de Variáveis

Os nomes das variáveis podem conter letras, números e o caractere _, mas devem começar com uma letra ou um _[^7]. Pense nos nomes de variáveis como identificadores de compartimentos que devem seguir regras específicas para evitar confusão a bordo.

### Exemplos de nomes válidos:

```python
myvar = "Python"
my_var = "Python"
_my_var = "Python"
myVar = "Python"
MYVAR = "Python"
myvar2 = "Python"
```

### Exemplos de nomes inválidos:

```python
2myvar = "Python"
my-var = "Python"
my var = "Python"
```

## Atribuição de Vários Valores

Python permite a atribuição de valores a múltiplas variáveis em uma única linha[^8]. Imagine distribuir diferentes cargas em vários compartimentos simultaneamente.

### Exemplo:

```python
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```

Também é possível atribuir o mesmo valor a múltiplas variáveis em uma única linha.

```python
x = y = z = "Orange"
print(x)
print(y)
print(z)
```

## Saída de Variáveis

A função `print()` é frequentemente usada para exibir variáveis. Você pode combinar texto e variáveis usando o operador +[^9]. Pense nisso como enviar um relatório de status que inclui informações de diferentes compartimentos.

### Exemplo:

```python
x = "Python"
print("Eu amo " + x)
```

Você também pode usar a vírgula , para adicionar variáveis a um texto impresso.

```python
x = "Python"
y = "é"
z = "fantástico"
print(x, y, z)
```

## Variáveis Globais

Variáveis que são criadas fora de uma função são conhecidas como variáveis globais. Elas podem ser usadas por qualquer função dentro do programa[^10]. Isso é similar a um compartimento central de suprimentos acessível a toda a tripulação.

### Exemplo:

```python
x = "fantástico"

def myfunc():
  print("Python é " + x)

myfunc()
```

Se você criar uma variável com o mesmo nome dentro de uma função, essa variável será local e só poderá ser usada dentro dessa função[^11]. Pense nisso como um compartimento de acesso restrito.

```python
x = "fantástico"

def myfunc():
  x = "maravilhoso"
  print("Python é " + x)

myfunc()
print("Python é " + x)
```

Para criar uma variável global dentro de uma função, você pode usar a palavra-chave global[^12]. Isso seria como fornecer um acesso universal a um compartimento específico.

```python
def myfunc():
  global x
  x = "fantástico"

myfunc()
print("Python é " + x)
```

## História: Dr. Zathras e o Teste de Clean Code

**Data Estelar 42002.3**
**Localização: U.S.S. Pythonrise**

A U.S.S. Pythonrise foi abordada por uma pequena nave de configuração desconhecida. A tripulação foi surpreendida ao ver Dr. Zathras, um renomado mas instável especialista em clean code, que apareceu na tela principal.

**Dr. Zathras:** "Tripulação da Pythonrise, recebi ordens diretas da Federação para realizar um teste de clean code com seus cadetes. Qualquer falha resultará em consequências severas. Preparem-se para serem testados sobre a correta atribuição de variáveis!"

Os cadetes ficaram tensos, mas estavam prontos para enfrentar o desafio. Dr. Zathras começou a fazer perguntas sobre os nomes das variáveis e a importância de seguir as normas de clean code.

**Dr. Zathras:** "Qual das seguintes opções é um nome de variável válido?"

1. 2myvar
2. my-var
3. my_var
4. my var
5. -myvar

Alguns cadetes hesitaram e não conseguiram responder corretamente. Cada resposta errada resultava em uma punição virtual dolorosa aplicada por Dr. Zathras. Cadete Zora Chen e Cadete Nex'ala estavam ansiosos. Cadete Zora tentou responder, mas errou a resposta.

**Dr. Zathras:** "Resposta errada! Prepare-se para uma punição."

Cadete Nex'ala também tentou, mas errou. A situação estava ficando crítica quando um jovem cadete, Cadete Thalor, de Betazed, que é autista, levantou a mão com calma.

**Cadete Thalor:** "A resposta correta é my_var."

Dr. Zathras ficou intrigado e impressionado com a precisão de Thalor. Ele ofereceu ao cadete um comunicador especial para contato exclusivo, sugerindo que ele poderia se juntar à sua nave futuramente. Thalor, no entanto, decidiu ficar com seus amigos na U.S.S. Pythonrise, apreciando o espaço e a inclusão que lhe foram dados.

**Cadete Thalor:** "Agradeço a oferta, Dr. Zathras, mas prefiro ficar aqui com meus amigos. Este é o meu lugar."

Dr. Zathras, embora relutante, entregou o comunicador e partiu, deixando a tripulação aliviada e orgulhosa do cadete Thalor. Ao partir, todos os cadetes que haviam sido punidos voltaram ao normal, como se nada tivesse acontecido.

## Glossário de Termos - Dra. T'Lara

**Variável**: Um contêiner para armazenar valores de dados[^1].
**Casting**: Atribuição de um tipo específico a uma variável[^3].
**Função `print()`**: Usada para imprimir a saída na tela[^9].
**Tipo de Dados**: A categoria de dados que uma variável pode armazenar[^4], como `int`, `str`, `float`.
**Variável Global**: Uma variável que pode ser acessada em qualquer lugar do código[^10].
**Variável Local**: Uma variável que só pode ser acessada dentro da função onde foi criada[^11].

## Resumo - Capitã T'Pral Bieniek

Neste capítulo, aprendemos sobre variáveis no Python, incluindo como criá-las, mudá-las e utilizá-las em diferentes contextos. Exploramos a diferença entre variáveis globais e locais e entendemos a importância da nomenclatura adequada. Essas habilidades são fundamentais para a construção de programas eficientes e bem-estruturados.

## Teste

1. Qual é a maneira correta de declarar uma variável em Python?

   - A) var x = 5
   - B) #x = 5
   - C) $x = 5
   - D) x = 5
   - E) var x: 5

2. Qual das seguintes opções é um nome de variável válido?

   - A) 2myvar
   - B) my-var
   - C) my_var
   - D) my var
   - E) myvar!

3. Como você obtém o tipo de uma variável em Python?

   - A) typeof(x)
   - B) type(x)
   - C) getType(x)
   - D) varType(x)
   - E) typeOf(x)

4. Qual é a saída do seguinte código?

   ```python
    x = 5
    x = "John"
    print(x)
   ```

   - A) 5
   - B) John
   - C) Erro
   - D) 5John
   - E) None

5. O que significa "variáveis são sensíveis a maiúsculas e minúsculas"?

   - A) `a` é o mesmo que `A`
   - B) `a` não é o mesmo que `A`
   - C) `a` e `A` são variáveis globais
   - D) `a` e `A` são variáveis locais
   - E) `a` é igual a `A`

6. Qual é a saída do seguinte código?

   ```python
   x, y, z = "Orange", "Banana", "Cherry"
   print(y)
   ```

   - A) Orange
   - B) Banana
   - C) Cherry
   - D) Erro
   - E) None

7. Como você declara uma variável global dentro de uma função?

   - A) global x
   - B) var x
   - C) def x
   - D) global.x
   - E) global: x

8. Qual das seguintes afirmações é verdadeira sobre variáveis em Python?

   - A) Elas devem ser declaradas antes de serem usadas
   - B) Elas podem mudar de tipo após serem definidas
   - C) Elas não podem ser usadas fora da função onde foram criadas
   - D) Elas só podem armazenar strings
   - E) Elas são imutáveis

9. Qual é a saída do seguinte código?

   ```python
   x = "Python"
   y = "é"
   z = "fantástico"
   print(x, y, z)
   ```

   - A) Python é
   - B) Python é fantástico
   - C) Pythonéfantástico
   - D) Erro
   - E) None

10. Como você especifica o tipo de uma variável em Python?

    - A) typeof()
    - B) int()
    - C) str()
    - D) casting()
    - E) type()

## Respostas do Teste - Tenente Comandante Vorik

1. **D) `x = 5`**Explicação: Em Python, variáveis são declaradas simplesmente atribuindo um valor a um nome de variável.
2. **C) `my_var`**Explicação: Os nomes de variáveis podem conter letras, números e o caractere _, mas devem começar com uma letra ou um _.
3. **B) `type(x)`**Explicação: A função `type()` retorna o tipo da variável.
4. **B) John**Explicação: Em Python, o tipo de uma variável pode mudar após ser definido.
5. **B) a não é o mesmo que A**Explicação: Python diferencia maiúsculas de minúsculas, portanto, `a` e `A` são variáveis distintas.
6. **B) Banana**Explicação: `y` é atribuído ao valor "Banana".
7. **A) global x**Explicação: A palavra-chave `global` torna a variável global dentro da função.
8. **B) Elas podem mudar de tipo após serem definidas**Explicação: Em Python, uma variável pode ser redefinida para outro tipo de dado.
9. **B) Python é fantástico**Explicação: A função `print()` pode combinar texto e variáveis.
10. **D) casting()**
    Explicação: Casting é usado para especificar o tipo de uma variável.

## Exercício Prático - Capitã Mira Romanov

**Desafio 1:**

Crie um script Python que declare três variáveis: `nome`, `idade` e `cidade`. Atribua a elas valores de acordo com suas preferências. Em seguida, imprima uma frase que use essas variáveis para formar uma sentença completa.

```python
# Seu código aqui
nome = "Spock"
idade = 35
cidade = "Vulcano"
print(nome, "tem", idade, "anos e mora em", cidade)
```

**Desafio 2:**

Crie uma função que receba duas variáveis numéricas e retorne a soma delas. Chame essa função e exiba o resultado.

```python
# Seu código aqui

def soma(a, b):
 return a + b

resultado = soma(10, 5)
print("A soma é:", resultado)
```

Cadetes, preparem seus códigos e continuem explorando as fronteiras do universo Python!

## Diálogo entre a Capitã e um Cadete

**Cadete Nex'ala:** "Capitã T'Pral, por que precisamos usar nomes de variáveis tão específicos? Não podemos simplesmente usar qualquer nome?"

**Capitã T'Pral Bieniek:** "Nex'ala, nomes de variáveis significativos ajudam a tornar o código mais legível e compreensível. Usar nomes de variáveis claros e consistentes é uma prática essencial de clean code. Isso facilita a manutenção do código e a colaboração com outros programadores."

**Cadete Nex'ala:** "Entendi, Capitã. Então, é como seguir um mapa estelar claro para evitar nos perdermos no espaço do código."

**Capitã T'Pral Bieniek:** "Exatamente, cadete. A clareza e a precisão são tão importantes na programação quanto na navegação estelar."

---

[^1]: Referência: [W3Schools - Python Variables](https://www.w3schools.com/python/python_variables.asp)
[^2]: Referência: [W3Schools - Python Variables](https://www.w3schools.com/python/python_variables.asp)
[^3]: Referência: [W3Schools - Python Casting](https://www.w3schools.com/python/python_casting.asp)
[^4]: Referência: [W3Schools - Python Variables](https://www.w3schools.com/python/python_variables.asp)
[^5]: Referência: [W3Schools - Python Strings](https://www.w3schools.com/python/python_strings.asp)
[^6]: Referência: [W3Schools - Python Variables](https://www.w3schools.com/python/python_variables.asp)
[^7]: Referência: [W3Schools - Variable Names](https://www.w3schools.com/python/python_variables_names.asp)
[^8]: Referência: [W3Schools - Assign Multiple Values](https://www.w3schools.com/python/python_variables_multiple.asp)
[^9]: Referência: [W3Schools - Output Variables](https://www.w3schools.com/python/python_variables_output.asp)
[^10]: Referência: [W3Schools - Global Variables](https://www.w3schools.com/python/python_variables_global.asp)
[^11]: Referência: [W3Schools - Global Variables](https://www.w3schools.com/python/python_variables_global.asp)
[^12]: Referência: [W3Schools - Global Variables](https://www.w3schools.com/python/python_variables_global.asp)
