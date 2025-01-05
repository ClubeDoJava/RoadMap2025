# Criando variáveis e nomeando-as
 

## Variáveis

Como você aprendeu na seção anterior, um objeto armazena seu estado em campos.

Vamos supor que temos um objeto Bicicleta:

````java
int cadência = 0;
int velocidade = 0;
int gear = 1;
````
gear = marcha

A seção: O que é um objeto? apresentou os campos, mas você provavelmente ainda tem algumas perguntas, como: 


````bash
> Quais são as regras e convenções para nomear um campo?

> Além de int, que outros tipos de dados existem?

> Os campos precisam ser inicializados quando são declarados? 

> É atribuído um valor padrão aos campos se eles não forem inicializados explicitamente?

````

Exploraremos as respostas a essas perguntas nesta seção, mas, antes disso, há algumas distinções técnicas que você deve conhecer primeiro. 


Na linguagem de programação Java, os termos “campo” e “variável” podem ser usados; 

essa é um ponto comum de confusão entre os novos desenvolvedores, pois ambos parecem se referir à mesma coisa.


 A linguagem de programação Java define os seguintes tipos de variáveis:
 

##  Variáveis de instância (campos não estáticos)


````rust

- Tecnicamente falando, os objetos armazenam seus estados individuais em “campos não estáticos”,

ou seja, campos declarados sem a palavra-chave static. 

- Os campos não estáticos também são conhecidos como variáveis de instância

porque seus valores são exclusivos para cada instância de uma classe (para cada objeto, em outras palavras); 

- Por exemplo: a velocidade atual  de uma bicicleta é independente da velocidade de outra.

````

## Variáveis de classe (campos estáticos)


````python
- Uma variável de classe é qualquer campo declarado com o modificador estático; 

isso informa ao compilador que existe exatamente uma cópia dessa variável,
independentemente de quantas vezes a classe tenha sido instanciada. 

- Um campo que define o número de marchas de um determinado tipo de bicicleta pode ser marcado como estático,

pois conceitualmente o mesmo número de marchas será aplicado a todas as instâncias. 

- O código static int numGears = 6; criaria esse campo estático. Além disso,

a palavra-chave final poderia ser adicionada para indicar que o número de marchas nunca será alterado.
````

## Variáveis locais


````cobol
- Da mesma forma que um objeto armazena seu estado em campos,

um método geralmente armazena seu estado temporário em variáveis locais. 

- A sintaxe para declarar uma variável local é semelhante à declaração de um campo (por exemplo, int count = 0;). 

- Não há nenhuma palavra-chave especial que designe uma variável como local;

essa determinação vem inteiramente do local em que a variável é declarada, que é entre as chaves de abertura e fechamento de um método. 

- Dessa forma, as variáveis locais são visíveis apenas para os métodos em que são declaradas;

elas não são acessíveis pelo restante da classe.
````

## Parâmetros


````java

- Você já viu exemplos de parâmetros,

 tanto na classe Bicycle quanto no método principal do aplicativo “Hello World!”.

- Lembre-se de que a assinatura do método main é public static void main(String[] args). 

- Aqui, a variável args é o parâmetro para esse método.

- O importante é lembrar que os parâmetros são sempre classificados como “variáveis” e não como “campos”. 

- Isso também se aplica a outras construções que aceitam parâmetros (como construtores e manipuladores de exceções),

 sobre as quais você aprenderá mais adiante no tutorial.

- Dito isso, o restante deste tutorial usa as seguintes diretrizes gerais ao discutir campos e variáveis.

- Se estivermos falando de “campos em geral” (excluindo variáveis locais e parâmetros), podemos dizer simplesmente “campos”. 

- Se a discussão se aplicar a “todos os itens acima”, podemos dizer simplesmente “variáveis”.

- Se o contexto exigir uma distinção, usaremos termos específicos
 (campo estático, variáveis locais etc.), conforme apropriado.

- Ocasionalmente, você também poderá ver o termo “membro” sendo usado.

- Os campos, métodos e tipos aninhados de um tipo são chamados coletivamente de membros.

````
 

# Nomeação de variáveis

````

- Toda linguagem de programação tem seu próprio conjunto de regras e convenções para os tipos de nomes que podem ser usados, e a linguagem de programação Java não é diferente. 

- As regras e convenções para nomear suas variáveis podem ser resumidas da seguinte forma:

- Os nomes das variáveis diferenciam maiúsculas de minúsculas. O nome de uma variável pode ser qualquer identificador legal - uma sequência de comprimento ilimitado de letras e dígitos Unicode, 

começando com uma letra, o cifrão $ ou o caractere de sublinhado _.

- Entretanto, a convenção é sempre começar os nomes das variáveis com uma letra, e não com $ ou _.

- Além disso, o caractere de cifrão, por convenção, nunca é usado. 

- Você pode encontrar algumas situações em que os nomes gerados automaticamente conterão o cifrão, mas seus nomes de variáveis devem sempre evitar usá-lo. 

- Existe uma convenção semelhante para o caractere de sublinhado; embora seja tecnicamente legal começar o nome da variável com _, essa prática não é recomendada. Não é permitido espaço em branco.
  
  ````

````
- Os caracteres subsequentes podem ser letras, dígitos, cifrões ou caracteres de sublinhado. As convenções (e o bom senso) também se aplicam a essa regra. 

Ao escolher um nome para suas variáveis, use palavras completas em vez de abreviações enigmáticas. Isso tornará seu código mais fácil de ler e entender. 

Em muitos casos, isso também tornará seu código autodocumentado; os campos denominados cadência, velocidade e marcha, por exemplo, são muito mais intuitivos do que as versões abreviadas, como s, c e g.

Lembre-se também de que o nome escolhido não deve ser uma palavra-chave ou palavra reservada.
````

````
Se o nome que você escolher consistir em apenas uma palavra, escreva essa palavra com todas as letras minúsculas.

Se for composto por mais de uma palavra, coloque a primeira letra de cada palavra subsequente em maiúscula. Os nomes gearRatio e currentGear são ótimos exemplos dessa convenção.

Se a sua variável armazena um valor constante, como static final int NUM_GEARS = 6, a convenção muda um pouco, colocando cada letra em maiúscula e separando as palavras subsequentes com o caractere de sublinhado.

Por convenção, o caractere de sublinhado nunca é usado em outro lugar.
```` 
