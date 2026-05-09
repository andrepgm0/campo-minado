# Campo Minado em Java

Projeto desenvolvido em Java inspirado no jogo clássico Minesweeper, utilizando conceitos de Programação Orientada a Objetos, tratamento de exceções e testes unitários.

---

# Estrutura do Projeto

```plaintext
src
└── br.com.cod3r.cm
    ├── excecao
    │   ├── ExplosaoException.java
    │   └── SairException.java
    │
    ├── modelo
    │   ├── Campo.java
    │   └── Tabuleiro.java
    │
    ├── visao
    │   └── TabuleiroConsole.java
    │
    └── Aplicacao.java

test
└── br.com.cod3r.cm.modelo
    └── CampoTeste.java
```

---

# Sobre o Projeto

O projeto simula o funcionamento do jogo Campo Minado, onde o jogador deve abrir os campos do tabuleiro sem encontrar minas escondidas.

O sistema foi organizado em pacotes para separar:
- regras do jogo;
- interface;
- tratamento de exceções;
- testes automatizados.

---

# Pacote `modelo`

Responsável pela lógica principal do jogo.

## `Campo.java`

Representa cada célula individual do tabuleiro.

### Responsabilidades:
- armazenar posição da célula;
- verificar se possui mina;
- controlar abertura do campo;
- controlar marcações;
- armazenar vizinhos;
- verificar explosões.

### Funcionalidades principais:
- abrir campo;
- adicionar vizinhos;
- alternar marcação;
- verificar minas na vizinhança.

---

## `Tabuleiro.java`

Responsável por controlar todo o tabuleiro do jogo.

### Responsabilidades:
- criar os campos;
- associar vizinhos;
- distribuir minas;
- verificar vitória;
- reiniciar partida.

### Funcionalidades principais:
- gerar tabuleiro;
- sortear minas;
- validar objetivo alcançado;
- reiniciar jogo.

---

# Pacote `visao`

Responsável pela interação com o usuário.

## `TabuleiroConsole.java`

Classe responsável pela interface em console.

### Responsabilidades:
- exibir tabuleiro;
- receber comandos do jogador;
- mostrar mensagens de vitória ou derrota;
- controlar fluxo da partida.

---

# Pacote `excecao`

Responsável pelas exceções personalizadas do projeto.

## `ExplosaoException.java`

Exceção lançada quando o jogador abre um campo minado.

### Objetivo:
- interromper a execução da partida;
- indicar derrota.

---

## `SairException.java`

Exceção utilizada para encerrar o jogo de maneira controlada.

### Objetivo:
- permitir saída do jogo sem encerrar abruptamente o programa.

---

# `Aplicacao.java`

Classe principal do projeto.

## Responsabilidade:
- iniciar o sistema;
- criar o tabuleiro;
- iniciar o jogo no console.

Contém o método:

```java
public static void main(String[] args)
```

---

# Pasta `test`

Responsável pelos testes automatizados do projeto.

## `CampoTeste.java`

Classe de testes unitários utilizando JUnit.

### Objetivos:
- validar funcionamento das regras do jogo;
- testar explosões;
- testar abertura de campos;
- validar vizinhança entre campos.

---

# Conceitos Utilizados

- Programação Orientada a Objetos (POO)
- Encapsulamento
- Tratamento de Exceções
- Testes Unitários
- Organização em Pacotes
- Separação de Responsabilidades

---

# Funcionalidades do Jogo

- geração automática do tabuleiro;
- distribuição aleatória de minas;
- abertura de campos;
- marcação de bandeiras;
- verificação de vitória;
- sistema de derrota ao encontrar minas.

---

# Tecnologias Utilizadas

- Java
- JUnit
- Eclipse IDE

---

# Objetivo do Projeto

O projeto foi desenvolvido com foco em aprendizado de:
- lógica de programação;
- orientação a objetos;
- boas práticas em Java;
- estruturação de projetos;
- testes automatizados.
