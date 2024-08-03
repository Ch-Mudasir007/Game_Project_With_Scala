# Scala-based Board Game Database Parser and Event Listener

## Table of Contents
1. [Introduction](#introduction)
2. [Project Structure](#project-structure)
3. [Class Descriptions](#class-descriptions)
4. [Usage Instructions](#usage-instructions)
5. [Installation](#installation)
6. [Configuration](#configuration)
7. [Execution](#execution)
8. [Conclusion](#conclusion)

## Introduction
The Board Game Event Notifier is a Scala-based application designed to manage and process a comprehensive database of board games. It performs tasks such as parsing the database, handling various events, and notifying users about specific board games based on certain criteria.

## Project Structure
The project is organized into the following main components:
- **Game**: A case class representing a board game.
- **GameParser**: An object that reads a CSV file and parses it into a list of Game objects.
- **EventManager**: An object that handles different types of events based on a computed value s.
- **Main**: The main entry point of the application.

### Directory Structure
project/
│
├── src/
│ ├── main/
│ │ ├── scala/
│ │ │ ├── Game.scala
│ │ │ ├── GameParser.scala
│ │ │ ├── EventManager.scala
│ │ │ └── Main.scala
│ │ ├── resources/
│ │ │ └── boardgames.csv
│ │ └── sbt/
│ │ └── build.sbt
│ └── test/


## Class Descriptions

### Game
A case class representing a board game with attributes such as `id`, `name`, `yearPublished`, `minPlayers`, `maxPlayers`, `playTime`, `minAge`, `category`, and `mechanic`.

### GameParser
An object responsible for reading and parsing the CSV file into a list of Game objects. It handles potential errors in the data and ensures only valid games are parsed.

### EventManager
An object that processes different events based on the value of s. It includes listeners for friends’ interests, company needs, and missing data detection.

### Main
The main entry point of the application. It generates random values for `n`, `a`, and `y`, parses the CSV file, and processes events based on the value of s.

## Usage Instructions

1. **Download the CSV File**: Ensure the board games dataset CSV file is downloaded and placed in the correct directory.
2. **Setup**: Configure the path to the CSV file in `Main.scala`.
3. **Compile and Run**: Use sbt to compile and run the project.

## Installation

1. **Install Scala**: Ensure Scala is installed on your system. You can download it from the [official Scala website](https://www.scala-lang.org/download/).
2. **Install sbt**: sbt (Scala Build Tool) is required to build and run the project. Download it from the [sbt website](https://www.scala-sbt.org/download.html).

## Configuration
Ensure the `build.sbt` file is correctly set up with the necessary dependencies, including the Scala version and any required libraries.

## Execution

1. **Compile the Project**: Use sbt to compile the project.
   ```bash
   sbt compile
##Run the Project: Use sbt to run the project
sbt run
