# Tetris

This project is a Java Tetris game built with Gradle and JGameGrid. The main game entry point is `tetris.Driver`, and the default launch configuration loads `properties/game1.properties`.

## How to run

From the repository root:

```bash
./gradlew :app:run
```

To launch a different properties file, pass its path as the first argument:

```bash
./gradlew :app:run --args="properties/game2.properties"
```

## How to play

Use the arrow keys while the game window is focused:

- Left arrow: move the current piece left
- Right arrow: move the current piece right
- Up arrow: rotate the current piece
- Down arrow: drop the current piece faster

Click Start to begin a new round.

## Scoring

When you complete a full horizontal line, it is cleared and your score increases by 1. As the game continues, pieces fall faster, so each round becomes more challenging.

## Notes

- The next piece is shown in the preview panel.
- The game saves statistics to `statistics.txt`.
