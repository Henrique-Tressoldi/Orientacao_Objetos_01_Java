# Object-Oriented Programming 1 (AD32C)

This repository is a portfolio of the practical exercises and case studies from the Object-Oriented Programming 1 course at UTFPR.

The project demonstrates a structured progression through the core concepts of OOP, from basic class instantiation to more complex topics like inheritance and polymorphism. The source code is organized by topic, reflecting the syllabus.

## Technology Stack

* **Language:** Java (JDK 14)
* **IDE:** Eclipse (implied by project structure)

## Core Concepts & Implementations

Below is a breakdown of the key OOP concepts demonstrated in this repository, with links to the relevant source code.

### 1. Classes, Objects, and Methods
* [cite_start]**`src/aula03/classeobjeto`**: Defines the initial `Carro` class [cite: 10][cite_start], demonstrating basic **class/object instantiation** and attribute assignment[cite: 11].
* [cite_start]**`src/aula05/metodos`**: Evolves the `Carro` class by adding **methods** (behaviors) like `ligar()`, `acelerar()`, and `toString()`[cite: 12, 13].

### 2. Class vs. Instance Variables (Static)
* **`src/aula06/variaveis`**: Demonstrates the difference between instance variables and class variables using `static`.
    * [cite_start]`Galinha.java`: Uses `static int quantidadeOvosGranja` to track a global state shared by all instances[cite: 14].
    * [cite_start]`ContaBancaria.java`: Uses `static int contatorContas` as a counter to assign unique IDs[cite: 15].

### 3. Constructors and Overloading
* [cite_start]**`src/aula07/metodosconstrutores`**: Implements multiple **constructors** in the `Carro` class (Constructor Overloading) to provide different ways of instantiating an object[cite: 16, 17].

### 4. Encapsulation
* **`src/aula09/encapsulamentodados`**: A core example of encapsulation.
    * `ContaBancaria.java`: Attributes (`saldo`, `titular`) are `private`. [cite_start]Access is controlled via public methods (`sacar()`, `depositar()`, `getSaldo()`, `setTitular()`)[cite: 4, 7].

### 5. Association and Composition
* **`src/aula10/associacoesclasses`**: Demonstrates the "has-a" relationship (Composition).
    * [cite_start]`Pessoa.java`: The `Pessoa` class *has-a* `private Endereco endereco`, composing two objects to form a larger structure[cite: 9].

### 6. Enumerations (Enums)
* **`src/aula11/enumeracoes`**: Shows the use of `enum` for type-safe, fixed sets of constants.
    * [cite_start]`Status.java`: Defines simple states for a `Pedido`[cite: 18].
    * [cite_start]`DiaSemana.java`: A more complex `enum` with attributes (`diaSemanaNumerico`) and methods (`getDiaSemanaExtenso()`)[cite: 19].

### 7. Collections
* **`src/aula12/listas`**: Implements `ArrayList` to manage collections of objects.
    * [cite_start]`ExemploListas.java`: Uses `List<Carro>`[cite: 20].
    * [cite_start]`Banco.java`: Uses `List<ContaBancaria>` to manage multiple bank accounts within a single `Banco` object[cite: 21].

### 8. Inheritance
* **`src/aula13/heranca`**: Demonstrates the "is-a" relationship (Inheritance).
    * [cite_start]`exemplo01`: A `Carro` [cite: 23] [cite_start]and an `Aviao` [cite: 24] both `extend Veiculo`, sharing common attributes and methods.
    * [cite_start]`exemplo02`: A `CoordenadorCurso` [cite: 22] [cite_start]`extends Professor`[cite: 25], inheriting its properties while adding specialized methods.
    * [cite_start]`exercicio`: `Aluno` [cite: 26] [cite_start]and `Professor` [cite: 27] [cite_start]both `extend Pessoa`[cite: 28], demonstrating a clear polymorphic hierarchy.
