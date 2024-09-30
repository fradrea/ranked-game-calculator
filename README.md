# Calculadora de Partidas Rankeadas

Este repositório contém um projeto prático de uma Calculadora de Partidas Rankeadas. O objetivo deste projeto é calcular o saldo de vitórias de um jogador em um jogo competitivo, determinar o nível do jogador com base nas vitórias e derrotas e exibir uma mensagem de saída que informa o saldo e o nível.

## Funcionalidades

- Recebe a quantidade de vitórias e derrotas como entrada.
- Calcula o saldo de vitórias.
- Classifica o jogador em diferentes níveis (Ferro, Bronze, Prata, Ouro, Diamante, Lendário e Imortal) com base no número de vitórias.
- Exibe uma mensagem informativa sobre o saldo e o nível do jogador.

## Níveis de Classificação

A classificação do jogador é baseada no número de vitórias:

- **Ferro**: Menos de 10 vitórias
- **Bronze**: 11 a 20 vitórias
- **Prata**: 21 a 50 vitórias
- **Ouro**: 51 a 80 vitórias
- **Diamante**: 81 a 90 vitórias
- **Lendário**: 91 a 100 vitórias
- **Imortal**: 101 ou mais vitórias

## Tecnologias Utilizadas

- **JavaScript**

## Instruções para Uso

1. Clone este repositório.
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git


    // Determina o nível com base no número de vitórias
    if (vitorias < 10) {
        nivel = "Ferro";
    } else if (vitorias >= 11 && vitorias <= 20) {
        nivel = "Bronze";
    } else if (vitorias >= 21 && vitorias <= 50) {
        nivel = "Prata";
    } else if (vitorias >= 51 && vitorias <= 80) {
        nivel = "Ouro";
    } else if (vitorias >= 81 && vitorias <= 90) {
        nivel = "Diamante";
    } else if (vitorias >= 91 && vitorias <= 100) {
        nivel = "Lendário";
    } else {
        nivel = "Imortal";
    }

    // Retorna o saldo de vitórias e o nível do jogador
    return { saldoVitorias, nivel };
}

// Exemplo de uso da função
const vitorias = 55; // Exemplo de vitórias
const derrotas = 30; // Exemplo de derrotas

const resultado = calcularNivel(vitorias, derrotas);
console.log(`O Herói tem de saldo de ${resultado.saldoVitorias} está no nível de ${resultado.nivel}`);
