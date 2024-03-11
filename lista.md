
# Questões objetivas

**1)** O que o código a seguir faz?

![Uma imagem](assets/ex01.PNG)

Escolha a opção que responde corretamente:

a) Imprime os números pares de 1 a 10.

b) Imprime os números ímpares de 1 a 10.

c) Imprime os números pares de 2 a 10.

d) Imprime os números ímpares de 2 a 10.

**RESPOSTA = OPÇÃO A**

______

**2)** Identificar a linha que falta no código para criar uma classe Veiculo com atributo marca, e uma classe Carro que herda de Veiculo com um método ligar(). 

![Uma imagem](assets/ex02.PNG)

No lugar onde está escrito “// linha” qual das opções abaixo deve estar para funcionar corretamente o código?

A) let carro = new Carro("Toyota");

B) let ligar = new ligar("Toyota");

C) class Moto extends Veiculo {};

D) carro1.ligar();

**RESPOSTA = OPÇÃO A**

______

**3)** Qual é o valor de resultado após a execução deste código?

![Uma imagem](assets/ex03.PNG)

Escolha a opção que responde corretamente:

A) 18

B) 16

C) 14

D) 12

**RESPOSTA = OPÇÃO A**

______

**4)** Como você criaria um método `acelerar()` em uma classe `Carro`, que recebe um parâmetro `velocidade` e o adiciona a um atributo `velocidadeAtual`?

A) ![Uma imagem](assets/ex04_1.PNG)

B) ![Uma imagem](assets/ex04_2.PNG)

C) ![Uma imagem](assets/ex04_3.PNG)

D) ![Uma imagem](assets/ex04_4.PNG)

**RESPOSTA = OPÇÃO A**

______

**5)** Qual a forma correta de definir uma classe Carro em JavaScript, com um método ligar() e um atributo marca?

A) ![Uma imagem](assets/ex05_1.PNG)

B) ![Uma imagem](assets/ex05_2.PNG)

C) ![Uma imagem](assets/ex05_3.PNG)

D) ![Uma imagem](assets/ex05_4.PNG)

**RESPOSTA = OPÇÃO A**

______

**6)** Observe o código abaixo:

![Uma imagem](assets/ex06.PNG)

Qual será a saída do código acima?

A) "Olá, meu nome é João. Olá, meu nome é Maria."

B) "Olá, meu nome é ."

C) "João Maria"

D) "undefined undefined"

**RESPOSTA = OPÇÃO A**

______

# Questões dissertativas

**7)** Vamos criar um programa em JavaScript para entender classes, métodos e atributos!
Classe Animal:
- Crie uma classe chamada Animal.
- Adicione dois atributos: nome e idade.
- Adicione um método chamado descrever() na classe Animal.
  - Este método deve exibir no console uma descrição do animal com seu nome e idade.

Criando e manipulando Animais:
- Crie dois objetos da classe Animal: um chamado "cachorro" e outro "gato", com idades distintas.
- Para cada animal, chame o método descrever() para ver a descrição no console.

Dica: Utilize `console.log()` para exibir as informações!

```javascript
class Animal {
    constructor(nome, idade) {
        this.nome = nome;
        this.idade = idade;
    }

    descrever() {
        console.log(`Eu sou um ${this.nome} e tenho ${this.idade} anos`);
    }
}

let gato = new Animal("gato", 10);
gato.descrever();
let cachorro = new Animal("cachorro", 3);
cachorro.descrever();

```
______

**8)** Nos últimos dias tivemos a oportunidade de ter contato com Programação Orientada a Objetos, e tivemos contato com o tema "herança". Herança é um princípio de orientação a objetos, que permite que classes compartilhem atributos e métodos. Ela é usada na intenção de reaproveitar código ou comportamento generalizado ou especializar operações ou atributos. Então vamos praticar esse conteúdo nessa questão.
Vamos criar um programa em JavaScript para entender classes, métodos, atributos e herança!

Classe Animal:
- Crie uma classe chamada Animal.
- Adicione dois atributos: nome e idade.
- Adicione um método descrever() que exiba no console uma descrição do animal com seu nome e idade.

Classe Gato (Herda de Animal):
- Crie uma classe chamada Gato que herda da classe Animal.
- Adicione um atributo extra cor específico para gatos.
- Adicione um método miar() que exiba no console o som que um gato faz.

Criando Animais:
- Crie dois objetos da classe Animal: um chamado cachorro e outro gato, com idades distintas.
- Para o gato, também defina a cor.

Chamando os Métodos:
- Para cada animal, chame o método descrever() para ver a descrição no console.
- Para o gato, chame o método miar() para "ouvir" o som que ele faz (é também para ver o som no console).

Dica: Utilize console.log() para exibir as informações!

```javascript
class Animal {
    constructor(nome, idade) {
        this.nome = nome;
        this.idade = idade;
    }

    descrever() {
        console.log(`Eu sou um ${this.nome} e tenho ${this.idade} anos`);
    }
}

class Gato extends Animal {
    constructor(nome, idade, cor) {
        super(nome, idade);
        this.cor = cor;
    }

    miar() {
        console.log('MIAL');
    }
}

let gato = new Gato("gato", 5, 'preto');
gato.miar();
gato.descrever();

let cachorro = new Animal("cachorro", 1);
cachorro.descrever();


```

______

**9)** Vamos criar um programa em JavaScript para somar notas!

Classe SomadorDeNotas:
- Crie uma classe chamada SomadorDeNotas.
- Adicione um atributo total inicializado com 0 para armazenar a soma das notas.

Método adicionarNota:
- Adicione um método chamado adicionarNota(nota) na classe SomadorDeNotas.
- Este método deve receber um parâmetro nota e somá-lo ao atributo total.

Criando o Somador e Adicionando Notas:
- Crie um objeto da classe SomadorDeNotas, chamado somador.
- Utilize o método adicionarNota(nota) para adicionar algumas notas ao somador.

Chamando o Método para Ver o Total:
- Após adicionar todas as notas, chame um método verTotal() para exibir o total das notas adicionadas.

Dica: Utilize console.log() para exibir as informações!

```javascript
  class SomadorDeNotas{
    constructor(){
        this.total = 0
    }
    adicionarNota(nota){
        this.nota = nota
        this.total += this.nota
    }
    verTotal(){
        console.log(this.total)
    }
}
let somador = new SomadorDeNotas()
somador.adicionarNota(4)
somador.adicionarNota(5)
somador.adicionarNota(2)  
somador.verTotal()

```
______

**10)** Imagine que você está criando um programa em JavaScript para uma escola. Neste programa, existem diferentes tipos de funcionários, cada um com suas próprias características. Considere as seguintes classes:

Funcionário:
- atributo: Nome
- atributo: Idade
- atributo: Salário base
- método: calcularSalario() - Este método calcula o salário total do funcionário. Para cada tipo de funcionário, o cálculo será diferente.

Professor (herança de Funcionário):
- atributo: Disciplina
- atributo: Horas de aula por semana
- método: calcularSalario() - Para calcular o salário do professor, multiplicamos suas horas de aula pelo valor da hora/aula.

Agora, sua tarefa é escrever um código em JavaScript que crie as classes Funcionário e Professor, com suas características e métodos descritos acima. Depois de criar as classes, crie:
- Dois objetos do tipo Professor com informações fictícias.
- Para cada objeto, chame o método calcularSalario() e mostre o salário calculado no console.

Certifique-se de explicar cada parte do código utilizando comentários, explicando para que serve cada atributo e método, bem como a lógica por trás do cálculo de salário para o tipo de funcionário Professor.

```javascript
class Funcionario {
    constructor(nome, idade, salarioBase) {
        this.nome = nome; // Define o nome do funcionário
        this.idade = idade; // Define a idade do funcionário
        this.salarioBase = salarioBase; // Define o salário base do funcionário
    }

    calcularSalario() {
        // Este método será implementado posteriormente para calcular o salário de um funcionário hipotético que não é professor.
    }
}

class Professor extends Funcionario {
    constructor(nome, idade, salarioBase, disciplina, horasAula) { // Define a classe Professor que herda da classe Funcionario
        super(nome, idade, salarioBase); // Chama o construtor da classe pai (Funcionario) para inicializar os atributos herdados
        this.salarioTotal = salarioBase * horasAula; // Calcula o salário total do professor baseado no salário base e nas horas de aula
        this.disciplina = disciplina; // Define a disciplina que o professor leciona
        this.nome = nome; // Define o nome do professor
    }

    calcularSalario(salarioBase, horasAula) {
        this.salarioTotal = salarioBase * horasAula; // Calcula o salário total do professor baseado no salário base e nas horas de aula
        console.log(`O salário total de ${this.nome} é de ${this.salarioTotal}`); // Exibe o salário total do professor
    }

    descrever(nome, idade, disciplina) {
        console.log(`Meu nome é ${nome}, tenho ${idade} anos e sou professor(a) de ${disciplina}`); // Exibe informações sobre o professor (nome, idade e disciplina)
    }
}

let professor1 = new Professor("Cristiano"); // Cria uma instância do professor Cristiano
professor1.calcularSalario(300, 30); // Calcula o salário do professor Cristiano
professor1.descrever("Cristiano", 22, "programação"); // Descreve o professor Cristiano

let professor2 = new Professor("Laura"); // Cria uma instância da professora Laura
professor2.calcularSalario(500, 40); // Calcula o salário daa professora Laura
professor2.descrever("Laura", 25, "química"); // Descreve a professora laura


```
