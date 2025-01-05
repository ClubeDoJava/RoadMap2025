# Objetos, classes, interfaces, pacotes e herança


Se você nunca usou uma linguagem de programação orientada a objetos antes, precisará aprender alguns conceitos básicos antes de começar a escrever qualquer código. 

Esta seção o apresentará a objetos, classes, herança, interfaces e pacotes. 

Cada discussão se concentra em como esses conceitos se relacionam com o mundo real 
e, ao mesmo tempo, fornece uma introdução à sintaxe da linguagem de programação Java.

 

# O que é um objeto?

Um objeto é um pacote de software com estado e comportamento relacionados.

Esta seção explica como o estado e o comportamento são representados em um objeto, 
apresenta o conceito de encapsulamento de dados e explica os benefícios de projetar o software dessa maneira.

Os objetos compartilham duas características: todos eles têm estado e comportamento. 
Os cães têm estado (nome, cor, raça, fome) e comportamento (latir, buscar, abanar a cauda). 
As bicicletas também têm estado (marcha atual, cadência atual do pedal, velocidade atual) e comportamento (mudança de marcha, mudança de cadência do pedal, aplicação de freios). 
Identificar o estado e o comportamento de objetos do mundo real é uma ótima maneira de começar a pensar em termos de programação orientada a objetos.


Reserve um minuto agora mesmo para observar os objetos do mundo real que estão em sua área imediata. 

Para cada objeto que você vir, faça a si mesmo duas perguntas: “Em que estados possíveis esse objeto pode estar?” e ‘Que comportamento possível esse objeto pode executar?’. 
Não se esqueça de anotar suas observações. Ao fazer isso, você perceberá que os objetos do mundo real variam em complexidade; 
sua lâmpada de casa pode ter apenas três estados possíveis (ligado e desligado ou queimada kkkk) e dois comportamentos possíveis (ligar, desligar), 
mas seu rádio pode ter estados adicionais (ligado, desligado, volume atual, estação atual) e comportamentos (ligar, desligar, aumentar o volume, diminuir o volume, buscar, procurar e sintonizar). 
Você também pode notar que alguns objetos, por sua vez, também conterão outros objetos. 
Essas observações do mundo real são um ponto de partida para entender o mundo da programação orientada a objetos.

Um objeto de software

Um objeto de software
Os objetos de software consistem em um estado e em um comportamento relacionado.
Um objeto armazena seu estado em campos (variáveis em algumas linguagens de programação) e expõe seu comportamento por meio de métodos (funções em algumas linguagens de programação). 
Os métodos operam no estado interno de um objeto e servem como o principal mecanismo de comunicação entre objetos. 

Ocultar o estado interno e exigir que toda a interação seja realizada por meio dos métodos de um objeto é conhecido como encapsulamento de dados - um princípio fundamental da programação orientada a objetos.

Considere uma bicicleta, por exemplo:

Uma bicicleta modelada como um objeto de software

Uma bicicleta modelada como um objeto de software
Ao atribuir um estado (velocidade atual, cadência atual do pedal e marcha atual) e fornecer métodos para alterar esse estado, o objeto permanece no controle de como o mundo externo pode usá-lo. 

Por exemplo, se a bicicleta tiver apenas 6 marchas, um método para mudar as marchas poderá rejeitar qualquer valor menor que 1 ou maior que 6.

O agrupamento de código em objetos de software individuais oferece vários benefícios, incluindo

Modularidade: O código-fonte de um objeto pode ser escrito e mantido independentemente do código-fonte de outros objetos. Uma vez criado, um objeto pode ser facilmente transmitido dentro do sistema.
Ocultação de informações: Ao interagir apenas com os métodos de um objeto, os detalhes de sua implementação interna permanecem ocultos do mundo externo.
Reutilização de código: Se um objeto já existir (talvez escrito por outro desenvolvedor de software), você poderá usá-lo em seu programa. Isso permite que os especialistas implementem/testem/depurem objetos complexos e específicos de tarefas, aos quais você pode confiar a execução em seu próprio código.
Facilidade de conexão e depuração: Se um determinado objeto se mostrar problemático, você pode simplesmente removê-lo do aplicativo e conectar um objeto diferente para substituí-lo. Isso é análogo a consertar problemas mecânicos. Isso é análogo ao conserto de problemas mecânicos no mundo real. Se um parafuso quebrar, você o substitui, não a máquina inteira.
 
