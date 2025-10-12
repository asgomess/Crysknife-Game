    INICIAR JOGO
        Mostrar tela Welcome
        Esperar jogador iniciar

    NIVEL = 1
    TEMPO_RESTANTE = TEMPO_STANDARD
    PONTUACAO = 0

    ENQUANTO jogo_ativo
        Atualizar tela
            Mostrar jogador
            Mostrar vermes vivos
            Mostrar pontuação (PONTUACAO)
            Mostrar tempo restante (TEMPO_RESTANTE)
            Mostrar nível atual (NIVEL)

    LER input jogador
        Mover jogador conforme input

    PARA cada verme VIVO
        Mover verme aleatoriamente
        SE jogador colidir com verme
            Remover verme
            PONTUACAO += pontos_verme  # Atualiza score

    SE todos os vermes mortos
        BONUS_SCORE = TEMPO_RESTANTE * 5  # opcional, pontos por tempo restante
        PONTUACAO += BONUS_SCORE
        NIVEL += 1
        Aumentar dificuldade
        Mostrar tela NextLevel
        Reiniciar vermes para novo nível

    Diminuir TEMPO_RESTANTE

    SE TEMPO_RESTANTE == 0
        Mostrar tela GameOver
    SENAO SE NIVEL > NIVEL_FINAL
        Mostrar tela FinalGame
