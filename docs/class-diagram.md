mermaid```
    classDiagram
        %% ======================
        %% Core Game Structure
        %% ======================
        class Game {
            - int level
            - int score
            - int remainingTime
            - boolean active
            + startGame()
            + update()
            + checkCollisions()
            + nextLevel()
            + gameOver()
        }

    class Player {
        - int x
        - int y
        - int speed
        - Image sprite
        + move(direction)
        + attack()
        + draw()
    }

    class Worm {
        - int x
        - int y
        - int speed
        - boolean alive
        - Image sprite
        + moveRandom()
        + die()
        + draw()
    }

    class LevelManager {
        - int currentLevel
        - List~Worm~ worms
        + spawnWorms(int count)
        + increaseDifficulty()
        + resetLevel()
    }

    class HUD {
        + drawScore(int score)
        + drawTime(int remainingTime)
        + drawLevel(int level)
    }

    class SoundManager {
        + playSound(String name)
        + stopSound(String name)
    }

    class ImageLoader {
        + loadImage(String path)
    }

    %% ======================
    %% Relationships
    %% ======================
    Game "1" *-- "1" Player : controls >
    Game "1" *-- "1" LevelManager : manages >
    LevelManager "1" *-- "*" Worm : contains >
    Game "1" *-- "1" HUD : displays >
    Game "1" *-- "1" SoundManager : uses >
    Game "1" *-- "1" ImageLoader : loads >
```
