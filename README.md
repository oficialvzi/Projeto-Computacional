# Projeto Computacional - Little Tiger Roulette
Projeto final de CPE - Little Tiger Roulette

<p align="center">
  <img src="roleta.gif" width="500" height="500" alt="Gif de uma Roleta">
</p>

## Integrantes
-Arthur Choi Braga - 242014300 <br />
-Matheus Cunha de Freitas - 242014355 <br />
-Beatriz Aguiar de Almeida - 242014319 <br />
-Felipe Hiohan de Jesus Silva - 242014391 <br />
-Larissa Julie Ferreira Lima - 242014426 <br />
-Maria Paula Vieira Ferreira - 242014382 <br />


## Descrição do projeto
O projeto consiste em fazer um simulador de roleta (Europeia) programado em C++. O usuário começa com 1000 dinheiros e pode apostar quanto quiser. O objetivo é fazer com que o usuário se divirta e se sinta em uma roleta real.

## 🛠️ Biblioteca incluídas
- `#include <iostream>` - Biblioteca base do entrada e saída do C++
- `#include <ctime>` - Biblioteca para o uso do horário do sistema para gerar números aleatórios
- `#include <cstdlib>` - Biblioteca para gerar números aleatórios
- `#include <thread>` e `#include <chrono>` - Bibliotecas para usar a função sleep() e dar um delay no programa

## ⚠️ Funções
### Girar Roleta()
```cpp	
//Função que gira a roleta (gera um número entre 0-36)
int girarRoleta() {
	return rand() % 37; // 0-36
}
```
### ehVermelho()
```cpp
//Função que retorna true se o número for vermelho ou false se for preto
bool ehVermelho(int numero) {
	const int vermelhos[] = {1,3,5,7,9,12,14,16,18,19,21,23,25,27,30,32,34,36};
	for(int i = 0; i < 18; i++) {
		if(numero == vermelhos[i]) return true;
	}
	return false;
}
```
