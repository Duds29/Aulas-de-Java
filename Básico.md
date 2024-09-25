# Iniciando o aprendizado em JAVA: 

Classe: É uma maneira de se criar objetos que possuem mesmo comportamento e mesma estrutura.
    a estrutura de uma classe é composta por: dados, metódos(operam os dados) e mecanismos de instanciação dos objetos.
      As classes possuem duas formas de serem declaradas: Normal ou Enum
   #Normal:
       Cada classe possui elementos opcionais e obrigatórios para sua criação, sua classe é escrita como: class + nomedaclasse, e assim oque estiver escrito antes/depois fazem parte de seus elementos
             ex: public class Alunos
                   public é um elemento modificador
      Cada classe possui um elemento antes dela indicando se é pública ou privada, essa instrução modifica a acessibilidade dos métodos, atributos e classes, alguns modificadores podem ser combinados.
            ex: annotation(anotação em java, pode ser substituida por uma anotação padrão), public, protected, private (são parte do encapsulamento, modificam o acesso), abstract, final(modificadores que relancionam-se com hierarquia de classe), static(afeta o ciclo de vida da instância, somente usado em classes membro) e strictfp(modificador que torna a implementação de cálculos de pontos flutuantes independentes da plataforma).
            ex de combinações: public abstract class Teste
   Caso a classe seja publica, em Java é exigido que seja salvo cada classe publica em um arquivo separado com o mesmo nome da classe. (Ou seja Arquivo Aluno.java, possui em seu código public class aluno)

Objeto: Possui duas caraterísticas (State e Behavior), seu state é guardado em variáveis e expõem seu behavior em methods(funções), as funções operam na parte interna do state e funcionam como mecanismo de comunicação. 
  Esconder o state e requisição de interações são performadas a partir dos methods, devido a data encapsulation  
  Atribuindo o state e methods para a mudança do state, estamos permitindo o controle do objeto. 

# Exemplo de States e Behavior: 
Cachorro:  
State - Nome, cor, raça, fome. 
Behavior - Latir, buscar, balançar o rabo. 

Pessoa: 
State – Nome, RG, CPF, data de nascimento. 
Behavior – Andar, correr, engatinhar.
