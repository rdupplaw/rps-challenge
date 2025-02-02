# RPS

This project contains a Sinatra application which allows a user to register a name and then play rock-paper-scissors against a computer. This application roughly follows the Model-View-Controller pattern.

## Model

The RPSGame class. RPSGame#play takes the player's choice ('rock', 'paper' or 'scissors') as an argument and returns a hash containing the outcome of the game and the computer's choice.

The outcome ('win', 'loss' or 'draw') is decided by randomly sampling an array containing the three possibilities. The computer's choice is then computed, corresponding to the player's choice and the outcome.

## Views

The views are contained in ERB files (registration.erb, game.erb, outcome.erb and the default template layout.erb).

## Controller

app.rb controls routing.

![image](https://user-images.githubusercontent.com/36577903/118403253-84bf1700-b665-11eb-9ecf-69f6149b4047.png)

# Installation

```
git clone https://github.com/rdupplaw/rps-challenge.git
cd rps-challenge
bundle
```

# Usage

```
rackup
```

# Testing

```
rspec
```
