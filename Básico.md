# Iniciando o aprendizado em JAVA: 

Classe: É uma maneira de se criar objetos que possuem mesmo comportamento e mesma estrutura.

a estrutura de uma classe é composta por: dados(são atributos/variáveis), metódos(operam os dados, chamados funções) e mecanismos de instanciação dos objetos(construtor).

As classes possuem duas formas de serem declaradas: Normal ou Enum

   ## Normal:
   
> Cada classe possui elementos opcionais e obrigatórios para sua criação, sua classe é escrita como: class + nomedaclasse, e assim oque estiver escrito antes/depois fazem parte de seus elementos

 ex: public class Alunos
     public é um elemento modificador

     
Cada classe possui um elemento antes dela indicando se é pública ou privada, essa instrução modifica a acessibilidade dos métodos, atributos e classes, alguns modificadores podem ser combinados.

 ex: annotation(anotação em java, pode ser substituida por uma anotação padrão), public, protected, private (são parte do encapsulamento, modificam o acesso), abstract, final(modificadores que relancionam-se com hierarquia de classe), static(afeta o ciclo de vida da instância, somente usado em classes membro) e strictfp(modificador que torna a implementação de cálculos de pontos flutuantes independentes da plataforma).
 
ex de combinações: public abstract class Teste
 
 Caso a classe seja publica, em Java é exigido que seja salvo cada classe publica em um arquivo separado com o mesmo nome da classe. (Ou seja Arquivo Aluno.java, possui em seu código public class aluno)
 
   Elementos opcionais: 
   
 - Tipoparametros: Implementação de programação genérica.
- Superclasses/Superinterface: Implementação de herança entre classes e interfaces.
  
   - Superclasses sempre serão do tipo extends identificadorClasses, pois extends indica que a classe é uma
                        subclasse do identificadorClasse e que irá herdar as suas caracteristicas;
  
  - Superinterfaces utiliza implements identificadorInterface, pois indica a implementação da interface
                        indicadorInterface;
    
# Instanciação de classes (criação de objeto)

Para poder utilizar as classes em um programa é necessário intanciá-las, e essas instâncias são chamadas de objetos, ou seja, a classe funciona como um modelo, em que objeto é baseado para sua construção, como uma planta de uma casa, em que a casa é baseada
no modelo da planta.

- Construtor:
  Quando criamos um objeto e instanciamos ele, precisamos inserir quais informações são obrigatória, essa é a função do construtor, indicar quais parametros serão incluidos a quais atributos.

Ex de processo de criação de objetos: 
```java
public Aluno (String nome, int idade) // Construtor
Aluno objetoAluno = new Aluno("Eduarda", 22) // Instanciação

```
public aluno = criação do contrutor.

(String nome, int idade)= atributo obrigatórios para o objeto.

Aluno objetoAluno = criação de um objeto(objetoAluno) que puxa os atributos e metodos da classe (Aluno).

new Aluno("Eduarda", 22) = chamada do construtor com as informações exigidas.

Após a execução teremos um novo objeto armazenado na memória, esse processo 
                        
# Objeto: 

Objetos para serem declarados é necessário que tenham as caracteristicas da classe que são referentes, ou seja, Aluno objetoAluno, Aluno é a classe e objetoAluno é o objeto.

O objeto possui duas caracteríticas (State e Behavior), seu state são os atributos, provenientes da classe, e tem o behavior, que são methods(são funções), que expõem o comportamente da classe, para manipular o atributo.

Ex: Classe gato, tem o atributo sede, e o metodo beber água, o metodo beber agua manipular o atributo sede, ou seja beber ou não água influencia a sede.

As funções operam na parte interna do state e funcionam como mecanismo de comunicação. 

  Esconder o state e requisição de interações são performadas a partir dos methods, devido a data encapsulation  
  Atribuindo o state e methods para a mudança do state, estamos permitindo o controle do objeto. 

# Exemplo de States e Behavior: 
Cachorro:  
State - Nome, cor, raça, fome. 
Behavior - Latir, buscar, balançar o rabo. 

Pessoa: 
State – Nome, idade. 
Behavior – Andar, correr, engatinhar.

# Destruição do Objeto

Em Java não é possível destruir manualmente um objeto, mas possui um conceito de coletor de  lixo.

O programa JVM, que verifica quais objetos não estão sendo mais referenciados e os destrói liberando espaço na memória, porém o programador não possui controle sobre o progama JVM.

# Encapsulamento de código

O encapsulamente tem como objetivo ocultar os atributos e funcionamentos de determinada classe, apartir do encapsulamento determina quais interações podem ocorrer, disponibilizando certos módulos apenas o necessário para realização das suas tarefas
O encapsulamento também pode ser relacionado a visibilidade de um método ou atributo

- PRIVATE: Só pode ser acessado internamente, para ser acessador é necessário usar métodos publicos (getters e setters), que controlam a leitura(get) e gravação(set), para que possam ser acessados e modificados de forma controlada e sem afetar a integridade do mesmo.
  
- PUBLIC: São vísiveis a todos
