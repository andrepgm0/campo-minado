# 💣 Campo Minado

Um jogo inspirado no clássico **Minesweeper**, desenvolvido em **Java** utilizando **Swing** para a interface gráfica.

O projeto foi criado com o objetivo de aplicar conceitos de Programação Orientada a Objetos (POO), eventos, observadores (Observer Pattern) e desenvolvimento de interfaces gráficas desktop utilizando Java.

---

## 🎮 Sobre o Jogo

O Campo Minado é um jogo de lógica onde o jogador deve revelar todas as casas seguras do tabuleiro sem clicar em uma bomba.

Ao selecionar uma casa:

- Se não houver bomba, a casa é revelada.
- Se houver uma bomba, ocorre uma explosão.
- Após a explosão, todas as bombas do tabuleiro são exibidas.
- O jogador pode marcar casas suspeitas com bandeiras para facilitar sua estratégia.

A partida termina quando:

✅ Todas as casas seguras forem abertas (Vitória)

❌ Uma bomba for acionada (Derrota)

---

## 🛠️ Tecnologias Utilizadas

- Java
- Java Swing
- Eclipse IDE
- Programação Orientada a Objetos
- Observer Pattern

---

## 📂 Estrutura do Projeto

```text
src
└── br.com.cod3r.cm
    ├── modelo
    │   ├── Campo.java
    │   ├── CampoEvento.java
    │   ├── CampoObservador.java
    │   ├── ResultadoEvento.java
    │   └── Tabuleiro.java
    │
    └── visao
        ├── BotaoCampo.java
        ├── PainelTabuleiro.java
        └── TelaPrincipal.java
```

### 📦 Pacote Modelo

Responsável pelas regras de negócio do jogo.

| Classe | Responsabilidade |
|----------|------------------|
| Campo | Representa uma célula do tabuleiro |
| CampoEvento | Eventos gerados pelas ações do campo |
| CampoObservador | Interface de observação dos eventos |
| ResultadoEvento | Resultado final da partida |
| Tabuleiro | Gerencia todo o tabuleiro e suas regras |

### 🖥️ Pacote Visão

Responsável pela interface gráfica.

| Classe | Responsabilidade |
|----------|------------------|
| BotaoCampo | Representação visual de cada campo |
| PainelTabuleiro | Painel contendo todas as células |
| TelaPrincipal | Janela principal do jogo |

---

## 🚀 Funcionalidades

- Campo minado totalmente funcional
- Interface gráfica com Java Swing
- Sistema de explosão
- Revelação automática das bombas
- Marcação de bandeiras
- Verificação de vitória
- Atualização visual em tempo real
- Separação entre lógica e interface

---

## 🎯 Como Jogar

### Clique Esquerdo

Abre uma casa do tabuleiro.

### Clique Direito

Marca ou desmarca uma casa suspeita de conter bomba.

### Objetivo

Abrir todas as casas seguras sem acionar nenhuma bomba.

---

## ▶️ Executando o Projeto

### Pré-requisitos

- Java JDK 8+
- Eclipse IDE (ou outra IDE Java)

### Passos

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/campo-minado.git
```

2. Abra o projeto no Eclipse.

3. Execute a classe:

```java
TelaPrincipal.java
```

4. Aproveite o jogo!

---

## 📚 Conceitos Aplicados

- Programação Orientada a Objetos (POO)
- Encapsulamento
- Eventos
- Observer Pattern
- Componentes Swing
- Interfaces Gráficas Desktop
- Manipulação de Matrizes
- Lógica de Jogos

---

## 🎓 Objetivo Acadêmico

Este projeto foi desenvolvido como forma de aprendizado e prática dos principais conceitos de Java Desktop, simulando o funcionamento do clássico Campo Minado através de uma arquitetura organizada entre modelo e visão.

---

## 👨‍💻 Autor

Desenvolvido em Java utilizando Swing no Eclipse IDE.
