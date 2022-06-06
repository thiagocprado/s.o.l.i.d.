SOLID com Java

Single responsability principle
Open Closed principle
Liskov Substitution principle
Interface Segregation principle
Dependency Inversion principle

------------------------------------------------------------------------------------------------

Principios da orientação a objetos

Coesão, Encapsulamente e Acoplamento.

Coesão: 
	Classe -> Atributos e métodos devem estar em harmonia e devem representar coisas em comum.

	Uma classe coesa faz bem uma única coisa.
	
	Classes coesas não devem ter várias responsabilidades.

	"Classes não coesas tendem a crescer indefinidamente, o que as tornam difíceis de manter."

Encapsulamento: 
	Proteção de uma classe contra manipulação externa.

	Getters e setters não são formas eficientes de aplicar encapsulamento.
	
	É interessante fornecer acesso apenas ao que é necessário em nossas classes.
	
	O encapsulamento torna o uso das nossas classes mais fácil e intuitivo.

	"Classes não encapsuladas permitem violação de regras de negócio, além de aumentarem o acoplamento."

Acoplamento:
	Evitar uma dependencia muito forte entre duas classes.

	Acoplamento é a dependência entre classes.
	
	Acoplamento nem sempre é ruim, e que é impossível criar um sistema sem nenhum acoplamento.
	
	Devemos controlar o nível de acoplamento na nossa aplicação.

	"Classes acopladas causam fragilidade no código da aplicação, o que dificulta sua manutenção."


------------------------------------------------------------------------------------------------------------

- Single responsability principle (Principio da responsabilidade única)
	(just because you can, doesn't mean you should)

	"uma classe deveria ter apenas um único motivo para mudar" - Robert Martin

	classes/métodos/funções/módulos devem ter uma única responsabilidade bem definida.

	Focado em coesão.

	Deixar as classes bem enxutas.

	Intuito é facilitar a manutenção, não precisando mexer em vários pontos do sistemas devido a uma unica alteração.

	Ao extrair códigos pensar na fragilidade que isso pode gerar na segurança.

- Open Closed principle (Principio aberto fechado)
	(open chest surgery is not needed when putting on a coat)

	não é necessário expor detalhes internos das classes.

	"Entidades de software (classes, módulos, funções, etc.) devem estar abertas para extensão, porém fechadas para modificação" - Bertrand Meyer

	cada classe deve conhecer e ser responsável por suas próprias regras de negócio

	devemos poder criar novas funcionalidades e estender o sistema sem precisar modificar muitas classes já existentes

	Uma classe que tende a crescer "para sempre" é uma forte candidata a sofrer alguma espécie de refatoração.

- Liskov Substitution principle
	(if it looks like a duck, quacks like a duck, but needs batteries - you probably have the wrong abstraction)

	"se q(x) é uma propriedade demonstrável dos objetos x de tipo T, então q(y) deve ser verdadeiro para objetos y de tipo S, onde S é um subtipo de T" - Barbara Liskov

	mais presente em casos de uso de Herança

	nem sempre herança é a melhor solução, podendo utilizar composição

	embora a herança favoreça o reaproveitamento de código, ela pode trazer efeitos colaterais quando não utilizada da maneira correta;

	 devemos poder substituir classes base por suas classes derivadas em qualquer lugar, sem problema.

- Interface segregation principle
	
	"uma classe não deveria ser forçada a depender de métodos que não utilizará" - Robert Martin

	interfaces devem definir apenas os métodos que fazem sentido para seu contexto;

	uma classe não deve ser obrigada a implementar um método que ela não precisa;

- Dependency Inversion Principle
	(would you solder a lamp directly to the wiring in a wall)

	"abstrações não devem depender de implementações. Implementações devem depender de abstrações" - Robert Martin

	é mais interessante e mais seguro para o nosso código depender de interfaces (classes abstratas, assinaturas de métodos e interfaces em si) do que das implementações de uma classe;
 
 	as interfaces são menos propensas a sofrer mudanças enquanto implementações podem mudar a qualquer momento;


obs: Numa herança tudo será herdado, mas precisamos pensar se faz sentido que tudo seja herdado.

programação orientada a objetos
sobre o java
instanciar 
classes
SOLID
Design Pattern 
Clean Code
injeção de dependencias