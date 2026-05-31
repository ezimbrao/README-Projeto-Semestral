Documentação do Projeto – Jogo de Corrida 2D
Visão Geral

O projeto consiste em um jogo de corrida 2D desenvolvido na Godot Engine, onde dois jogadores competem em tempo real para completar circuitos, desviando de obstáculos e acumulando pontos.

O jogo possui múltiplos níveis, sistema de pontuação, HUD em tempo real e tela final de vencedor.

Mecânicas do Jogo
Jogadores
Dois jogadores locais:
Player 1 (Carro Azul)
Player 2 (Carro Verde)
Controles
Cada jogador possui controles independentes (teclado)
Movimentação em 4 direções
Objetivo
Cruzar a linha de chegada
Acumular pontos ao completar voltas/fases
Funcionalidades Implementadas
Sistema de Pontuação
Controlado pelo script Global.gd
Variáveis:
map_score_p1
map_score_p2
HUD (Interface)
Exibe pontuação em tempo real
Atualizado continuamente via hud.gd
Sistema de Fases
Controle feito por level_controller.gd
Permite mudança automática de cena
Linha de Chegada
Detecta quando o jogador finaliza (finish.gd)
Incrementa pontuação
Checkpoints
Permitem validar se o jogador pode pontuar
Obstáculos Dinâmicos
Spawn automático (spawner.gd)
Movimentação contínua
Desaparecem ao sair da tela
Tela de Vitória
Exibe vencedor com base na pontuação
Implementado em winner_screen.gd
Estrutura do Projeto
Scripts Principais
player.gd → movimentação dos jogadores
game_manager.gd → controle de pontuação
level_controller.gd → troca de fases
hud.gd → interface
spawner.gd → geração de obstáculos
finish.gd → lógica de chegada
Assets
Sprites de carros (cores diferentes)
Tilesets de pista
Obstáculos e cenário
Fluxo do Jogo
Jogadores iniciam corrida
Desviam de obstáculos
Passam por checkpoints
Cruzam linha de chegada
Pontuação é atualizada
Próximo nível ou tela final
Possíveis Melhorias
Sistema de voltas (laps)
Inteligência artificial para NPCs
Multiplayer online
Efeitos sonoros e música
Menu inicial mais completo
Sistema de colisão mais refinado
Tecnologias Utilizadas
Godot Engine
GDScript
Conclusão

O projeto demonstra conceitos importantes de desenvolvimento de jogos, como controle de estado, interação entre cenas, lógica de pontuação e gameplay multiplayer local.
