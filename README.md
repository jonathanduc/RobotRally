# RobotRally - JavaFX Multiplayer Game

Academic software-development project inspired by the **RoboRally** board game. The application was developed in Java with JavaFX and follows an MVC-oriented structure with a client/server architecture.

> This was a **team project**. The repository is kept public as an earlier software-engineering project and as part of the progression visible in my GitHub profile.

## Project objective

The goal was to recreate the main mechanics of RoboRally for **2 to 4 players**. Each player controls a robot and selects movement cards that determine the robot's actions during a turn.

The intended game loop includes:

- distribution of movement cards
- selection of five cards per player
- turn execution in player order
- robot movement and orientation
- checkpoints
- damage and life management
- special board tiles
- multiplayer communication between clients and a server

## Implemented architecture

The repository contains both client-side game/interface code and server-side networking code.

```text
.
├── Main.java
├── controllers/
├── views/
├── classes/
├── player/
├── Cards/
└── RbRServer/
```

The project uses:

- Java
- JavaFX
- FXML / Scene Builder
- MVC-style separation
- client/server communication
- Java serialization

## Gameplay concepts implemented

The codebase contains logic for several RoboRally mechanics, including movement cards and special board effects such as rotation tiles, walls, boosts, lasers, black holes, repair tiles, checkpoints and damage management.

Some mechanics were implemented in code but were not fully integrated into a finished playable version.

## Current limitations

The project was not completed before the academic deadline. Known limitations from the original implementation include:

- some special-board interactions are incomplete in the final playable flow
- some movement cards can become unselectable
- a robot can leave the board in some situations
- the server port may need to be changed if already occupied
- several original board image assets were too large to include in the repository

These limitations are documented intentionally rather than hidden, because this repository represents an earlier stage of my software-development experience.

## Running the project

The original workflow is:

1. Start the server from the `RbRServer` project.
2. Wait until the server reports that it is ready.
3. Start the client application.
4. Launch additional client instances for additional players, up to four.

Depending on the local Java/JavaFX configuration, the project may require IDE or module-path configuration before it runs on a recent JDK.

## What this project taught me

This project was one of my first substantial collaborative software projects. It introduced me to:

- structuring an application across models, controllers and views
- coordinating client/server components
- representing game state through Java classes
- serializing objects for network communication
- working on a shared codebase with multiple contributors
- dealing with incomplete features, integration issues and technical debt

My more recent projects are primarily focused on Python, Data Engineering and AI, but I keep RobotRally public because it documents the evolution of my engineering experience.

## Team

- Alya Zouzou
- Audric Girondin
- Noa Thebaut
- Jonathan Duckes
- Lucas Martinez

## Jonathan Duckes

- GitHub - https://github.com/jonathanduc
- LinkedIn - https://www.linkedin.com/in/jonathan-duckes/
- Portfolio - https://jonathanduc.github.io/portfolio/
