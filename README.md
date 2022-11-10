# padr-es-de-projeto
Prototype

O Prototype é um padrão de projeto criacional que permite a clonagem de objetos, mesmo complexos, sem que os códigos dependam das suas classes específicas.
 Todas as classes de prototypes(protótipos) devem ter uma interface comum que permita copiar objetos, mesmo que suas classes concretas sejam desconhecidas. Objetos protótipos podem produzir cópias completas, pois objetos da mesma classe podem acessar os campos privados um do outro.
Quando se trata de herança, o JavaScript tem somente um construtor: objetos. Cada objeto tem um link interno para um outro objeto chamado prototype . Esse objeto prototype também tem um atributo prototype , e assim por diante até o que o valor null seja encontrado como sendo o seu prototype
Vantagens: 
Classes podem ser definidas em nível de execução;
Alternativa simples quando o padrão Abstract Factory se mostrar complexo, principalmente na questão de hierarquia;
Conjunto inicial independente da hierarquia.

Desvantagens: 
Cada subclasse de Prototype deve implementar a operação clone, o que pode ser difícil quando as classes consideradas já existem por exemplo;
A implementação de clone pode ser complicada quando uma estrutura interna de classe inclui objetos circulares e que não suportam operação de cópia;
É necessário saber a classe do objeto para poder fazer a cópia, ou seu código acaba se tornando dependente daquela classe;
Algumas vezes você só sabe a interface que o objeto segue, mas não sua classe concreta, quando, por exemplo, um parâmetro em um método aceita quaisquer objetos que seguem uma interface;
Para que seja feita a cópia é necessário criar um novo objeto da mesma classe, e então ir clonando parte por parte até possuir o objeto como um todo. Porém, algumas dessas partes podem ser privadas e não ficando visíveis fora do projeto.


Referências:
https://refactoring.guru/pt-br/design-patterns/prototype
https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Inheritance_and_the_prototype_chain#:~:text=Quando%20se%20trata%20de%20heran%C3%A7a,como%20sendo%20o%20seu%20prototype%20.
https://pt.slideshare.net/tceufrasio1/prototype-10016673

