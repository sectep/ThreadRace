# ThreadRace
A Java-based project that simulates a race between two threads with different priorities. The higher priority thread completes its task faster, while the lower priority thread is delayed, demonstrating how thread priority influences execution in a multithreading environment.

This Java project simulates a race between two threads with different priorities. The threads print dots to indicate their progress, and their race speed is determined by the thread priority. The higher priority thread runs faster, whereas the lower priority one runs slower.

## Features:
- **Multithreading**: Utilizes Java threads to simulate a race between two players.
- **Thread Priority**: Demonstrates how thread priority can be used to influence thread execution speed.
- **Race Simulation**: Two threads, one with the highest priority and the other with the lowest, race each other by printing dots.

## How It Works:
1. **MyThread Class**: Implements the `Runnable` interface to create threads that can be prioritized. 
2. **Main Class**: Initializes the race and monitors both players' progress.
3. The race uses two players, `Racer1` (maximum priority) and `Racer2` (minimum priority).
4. The dot printing speed is determined by the thread's priority: higher priority results in a faster race.

## Classes:
1. **MyThread**: Contains logic for creating a thread, setting its priority, and starting the thread.
2. **Main**: The main class that creates the players (threads), sets their priorities, and waits for them to finish the race.

## Usage:
1. Clone the repository:
    ```bash
    git clone https://github.com/sectep/ThreadRace.git
    ```
2. Compile the project:
    ```bash
    javac MyThread.java
    javac Main.java
    ```
3. Run the program:
    ```bash
    java Main
    ```
4. Watch the race and observe how thread priorities affect the race outcome.

## Example Output:
```
Racer1 is running
.
Racer2 is running
.
.
.
.
Racer2 finished racing
.
.
.
Racer1 finished racing
The race is over.
```

## Requirements:
- Java 8 or higher.

## Author:
sectep

