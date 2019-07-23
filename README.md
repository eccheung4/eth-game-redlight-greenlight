# Red light, Green light: State Channel Turn-based Game

## Description:
Ethereum State Channel Game Idea born out of the State of Scale hackathon from Jan, Kseniya, and Edwin.

Two types of players: Monitor and Players

One move per red light, green light

Players join with 1 Dai and adds to pot

Monitor automatically gets 20% from pot

## State:
```
monitor position: 100 steps
current move: // To keep track what move monitor is on
player scores
```

## Game Flow:
1. Players roll dice and submit with current move #, if player doesn’t submit move before monitor annoucement, they lose move
2. Monitor submits red light with dice roll or green light
   a. Red Light, take difference between monitor and player number to get amount to move
   b. Green Light, move full value of dice roll
3. Repeat from 1 til someone passes monitor and wins
