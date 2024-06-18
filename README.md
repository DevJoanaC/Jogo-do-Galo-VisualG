# Jogo do Galo 🎮

Bem-vindo ao repositório do Jogo do Galo! Este projeto foi desenvolvido para simular o clássico jogo do Galo, proporcionando uma experiência interativa para dois jogadores competirem entre si.

## Introdução

O desafio deste projeto é criar uma aplicação interativa que permita dois jogadores alternarem suas jogadas num tabuleiro 3x3. Cada jogador é identificado por 'X' ou 'O', e o objetivo é formar uma linha, coluna ou diagonal com suas marcas. O jogo termina quando um jogador vence ou quando todas as células são preenchidas, resultando em empate.

O Jogo do Galo é um excelente exercício para praticar conceitos de lógica de programação, estruturas de controlo, e manipulação de eventos de interface. Este projeto não apenas permite aos jogadores desfrutarem de partidas divertidas, mas também serve como uma introdução prática ao desenvolvimento de jogos simples em ambiente computacional.

## Fundamentação

O jogo foi implementado utilizando lógica de programação em VisualG. A estrutura básica envolve:
- Um tabuleiro 3x3 representado por uma matriz.
- Dois jogadores que se alternam nas jogadas.
- Verificação de vitória ou empate após cada jogada.

## Funcionalidades

- **Jogadores Alternados:** Os jogadores 'X' e 'O' alternam suas jogadas.
- **Tabuleiro 3x3:** O tabuleiro é uma matriz 3x3 onde os jogadores marcam suas jogadas.
- **Verificação de Vitória:** O programa verifica se um jogador formou uma linha, coluna ou diagonal após cada jogada.
- **Empate:** O jogo também verifica se todas as células estão preenchidas, resultando em empate se ninguém venceu.
- **Interface Interativa:** Desenvolvido em VisualG, permitindo uma experiência interativa e educativa.

## Como Jogar

1. **Inicie o jogo:** O programa inicializa um tabuleiro vazio e informa que o jogador 'X' começa.
2. **Jogadas Alternadas:** Os jogadores alternam-se para marcar suas jogadas no tabuleiro.
3. **Verificação:** Após cada jogada, o programa verifica se houve um vencedor ou se o jogo terminou em empate.
4. **Resultado:** O jogo exibe uma mensagem informando o vencedor ou se houve empate, e então reinicia para uma nova partida.

## Exemplo de Código

```visualg
// Inicialização do tabuleiro
para i de 1 ate 3 faca
    para j de 1 ate 3 faca
        tabuleiro[i, j] <- " "
    fimpara
fimpara

// Loop do jogo
repita
    // Exibir tabuleiro
    ...
    
    // Jogada do jogador atual
    se jogadorAtual = "X" entao
        // Lógica para jogada do jogador X
    senao
        // Lógica para jogada do jogador O
    fimse
    
    // Verificar vitória ou empate
    ...
    
    // Alternar jogador
    se jogadorAtual = "X" entao
        jogadorAtual <- "O"
    senao
        jogadorAtual <- "X"
    fimse
ate que (vencedor ou empate)
