# Jogo de Corrida 2D - Multiplayer Local

## Sobre o Projeto

Este projeto consiste em um jogo de corrida 2D desenvolvido utilizando a Godot Engine. A proposta é oferecer uma experiência competitiva local, onde dois jogadores disputam em tempo real, desviando de obstáculos e acumulando pontos ao completar o percurso.

O jogo conta com múltiplos níveis, sistema de pontuação, interface em tempo real (HUD) e tela final de vencedor.

---

## Gameplay

* Multiplayer local para dois jogadores
* Corrida com objetivo de chegar primeiro
* Obstáculos dinâmicos durante a pista
* Sistema de pontuação em tempo real
* Tela de vitória ao final da partida

---

## Controles

Cada jogador possui controles independentes no teclado:

* Movimentação em quatro direções
* Jogadores:

  * Player 1 (Carro Azul)
  * Player 2 (Carro Verde)

---

## Funcionalidades

### Sistema de Pontuação

* Gerenciado pelo script `Global.gd`
* Variáveis principais:

  * `map_score_p1`
  * `map_score_p2`

### HUD (Interface)

* Exibe pontuação em tempo real
* Atualização contínua via `hud.gd`

### Sistema de Fases

* Controlado por `level_controller.gd`
* Transição automática entre níveis

### Linha de Chegada

* Detecta finalização (`finish.gd`)
* Responsável por contabilizar pontos

### Checkpoints

* Garantem que o percurso seja seguido corretamente

### Obstáculos Dinâmicos

* Gerados automaticamente (`spawner.gd`)
* Movimento contínuo na pista
* Remoção automática ao sair da tela

### Tela de Vitória

* Exibe o jogador vencedor
* Implementada em `winner_screen.gd`

---

## Estrutura do Projeto

```
Projeto
 ├── scripts/
 │   ├── player.gd
 │   ├── game_manager.gd
 │   ├── level_controller.gd
 │   ├── hud.gd
 │   ├── spawner.gd
 │   └── finish.gd
 ├── scenes/
 ├── assets/
 └── project.godot
```

---

## Fluxo do Jogo

1. Jogadores iniciam a corrida
2. Desviam de obstáculos
3. Passam pelos checkpoints
4. Cruzam a linha de chegada
5. Pontuação é atualizada
6. Avançam de fase ou finalizam o jogo

---

## Possíveis Melhorias

* Sistema de voltas (laps)
* Multiplayer online
* Inteligência artificial (NPCs)
* Sons e trilha sonora
* Menu inicial mais elaborado
* Sistema de colisão mais avançado

---

## Tecnologias Utilizadas

* Godot Engine
* GDScript

---

## Como Executar o Projeto

1. Instale a Godot Engine
2. Clone ou baixe este repositório
3. Abra o projeto na Godot
4. Execute a cena principal

---

## Conclusão

Este projeto foi desenvolvido com o objetivo de aplicar conceitos fundamentais de desenvolvimento de jogos, incluindo lógica de programação, organização de scripts, gerenciamento de estados, interação entre cenas e desenvolvimento multiplayer local.

---

## Autores

Projeto desenvolvido como trabalho acadêmico.
