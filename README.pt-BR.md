# Orientação a Objetos 1 (AD32C)

Este repositório é um portfólio dos exercícios práticos e estudos de caso da disciplina de Orientação a Objetos 1 da UTFPR.

O projeto demonstra uma progressão estruturada através dos conceitos centrais da POO, desde a instanciação básica de classes até tópicos mais complexos como herança e polimorfismo. O código-fonte está organizado por tópico, refletindo a ementa.

## Tecnologias
* **Linguagem:** Java (JDK 14)
* **IDE:** Eclipse (implícito pela estrutura do projeto)

## Conceitos e Implementações

Abaixo está um detalhamento dos principais conceitos de POO demonstrados neste repositório, com links para o código-fonte relevante.

### 1. Classes, Objetos e Métodos
* [cite_start]**`src/aula03/classeobjeto`**: Define a classe inicial `Carro` [cite: 10][cite_start], demonstrando a **instanciação de classes/objetos** e atribuição de atributos[cite: 11].
* [cite_start]**`src/aula05/metodos`**: Evolui a classe `Carro` ao adicionar **métodos** (comportamentos) como `ligar()`, `acelerar()` e `toString()`[cite: 12, 13].

### 2. Variáveis de Classe vs. Instância (Static)
* **`src/aula06/variaveis`**: Demonstra a diferença entre variáveis de instância e variáveis de classe usando `static`.
    * [cite_start]`Galinha.java`: Usa `static int quantidadeOvosGranja` para rastrear um estado global compartilhado por todas as instâncias[cite: 14].
    * [cite_start]`ContaBancaria.java`: Usa `static int contatorContas` como um contador para atribuir IDs únicos[cite: 15].

### 3. Construtores e Sobrecarga
* [cite_start]**`src/aula07/metodosconstrutores`**: Implementa múltiplos **construtores** na classe `Carro` (Sobrecarga de Construtor) para fornecer diferentes formas de instanciar um objeto[cite: 16, 17].

### 4. Encapsulamento
* **`src/aula09/encapsulamentodados`**: Um exemplo central de encapsulamento.
    * `ContaBancaria.java`: Atributos (`saldo`, `titular`) são `private`. [cite_start]O acesso é controlado via métodos públicos (`sacar()`, `depositar()`, `getSaldo()`, `setTitular()`)[cite: 4, 7].

### 5. Associação e Composição
* **`src/aula10/associacoesclasses`**: Demonstra o relacionamento "tem-um" (Composição).
    * [cite_start]`Pessoa.java`: A classe `Pessoa` *tem-um* `private Endereco endereco`, compondo dois objetos para formar uma estrutura maior[cite: 9].

### 6. Enumerações (Enums)
* **`src/aula11/enumeracoes`**: Mostra o uso de `enum` para conjuntos de constantes fixos e seguros.
    * [cite_start]`Status.java`: Define estados simples para um `Pedido`[cite: 18].
    * [cite_start]`DiaSemana.java`: Um `enum` mais complexo com atributos (`diaSemanaNumerico`) e métodos (`getDiaSemanaExtenso()`)[cite: 19].

### 7. Coleções
* **`src/aula12/listas`**: Implementa `ArrayList` para gerenciar coleções de objetos.
    * [cite_start]`ExemploListas.java`: Usa `List<Carro>`[cite: 20].
    * [cite_start]`Banco.java`: Usa `List<ContaBancaria>` para gerenciar múltiplas contas bancárias dentro de um único objeto `Banco`[cite: 21].

### 8. Herança
* **`src/aula13/heranca`**: Demonstra o relacionamento "é-um" (Herança).
    * [cite_start]`exemplo01`: Um `Carro` [cite: 23] [cite_start]e um `Aviao` [cite: 24] `extend Veiculo`, compartilhando atributos e métodos comuns.
    * [cite_start]`exemplo02`: Um `CoordenadorCurso` [cite: 22] [cite_start]`extends Professor`[cite: 25], herdando suas propriedades e adicionando métodos especializados.
    * [cite_start]`exercicio`: `Aluno` [cite: 26] [cite_start]e `Professor` [cite: 27] [cite_start]`extend Pessoa`[cite: 28], demonstrando uma hierarquia polimórfica clara.
