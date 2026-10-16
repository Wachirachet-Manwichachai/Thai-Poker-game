# Documentation
# Innovator’s Journal: Developing My Pok Deng Game

## 1. My Development Process

During the development of my Thai poker game or Pok Deng, I used WebbGPT as a tool to help me understand and develop the code. Since the game involved many different systems and complex function like dealing cards, calculation the hand value, player decision making(draw or stay) and determined the winner which not only compare between me and the deal but also the other players. Which I found I way to understand a system before deep analyse the code and it properties.
Which is asking AI to generate flowchart which is programming structure, which help us understand the structure of the game in this case. Additionally, I asked AI to generate the code but with comment of what does the line and the function mean.

## 2. How I Used AI and Improved My Results

My interaction with AI was a process of learning and refinement. Initially, I needed help understanding how the different functions and variables connected. I then focused on understanding the sequence of events in the game rather than looking at the code as one large block.

For example, I examined how the `playRound()` function starts a round, shuffles the deck, distributes cards, and determines whose turn it is. I also explored how `handVal()` calculates a player's hand value and how `showdown()` compares the players' hands against the dealer.

I used these functions as examples to understand the difference between the overall game flow and the smaller calculations that support it. By directing my attention toward specific parts of the program, I could use AI to explain the code in a more understandable way instead of receiving explanations that were too broad.

I also learned that AI-generated code should not automatically be assumed to be correct. I needed to examine the logic, compare the explanations with the actual code, and consider whether the program behaved as intended. This helped me approach AI as a learning assistant rather than a tool that should make every decision for me.


## 3. What I Learned About Software and Coding

Through this project, I deepened my understanding of several programming concepts.

First, I learned about **variables and state**. Variables such as `chips`, `bet`, `hands`, and `phase` store information that changes throughout the game. The `phase` variable is particularly important because it helps prevent the player from starting another round while the current round is still in progress.

Second, I learned about **functions and modular programming**. Functions such as `cardVal()`, `handVal()`, `dengInfo()`, and `showdown()` each have specific responsibilities. Separating the program into functions makes the code easier to understand, test, and modify.

Third, I developed a better understanding of **conditional statements and decision-making**. The game uses conditions to determine whether a player has Pok, whether a player should draw another card, and whether a hand wins or loses against the dealer.

Finally, I learned about **asynchronous programming**. The use of `async`, `await`, and `sleep()` allows the game to pause between actions, creating animations and making the gameplay feel more natural. This showed me that programming involves not only calculating correct results but also controlling the timing and sequence of events.

## 4. How I Might Approach Software Development in the Future

In the future, I would approach software development in a more structured way. Before writing code, I would identify the main features of the program and create a flowchart showing how users interact with it and how the program responds.

Next, I would divide the program into smaller functions and develop one feature at a time. I would test each feature before connecting it to the rest of the program. If I used AI, I would ask specific questions about the logic, request explanations of unfamiliar functions, and use the answers to improve my own understanding.

I would also use flowcharts when debugging. If a feature did not work correctly, I could trace the sequence of decisions and identify where the actual behavior differed from the intended behavior. This would help me find the source of a problem instead of randomly changing lines of code.

Overall, this project taught me that successful software development requires more than generating code. It requires planning, logical thinking, testing, and understanding how individual components work together. By combining AI assistance with flowcharts and my own evaluation of the results, I can become more independent and systematic when developing software in the future.

# Thai-Poker-game
# Autopsy
# Size
In my code instead of using HTML <canvas> element. Instead, it uses different HTML elements like <div> to disply the game table, cards, chips, and button
# Variables
My game keeps track of the deck of cards, player's hands, dealer's hand, chip balances, bets, current round, and game phase. These variables are declared in the JavaScript code. The main variables include deck, hands, dealerHand, chips, bet, bets, roundN, and phase.
# Loop
In my game doesn't contain loop like requestAnimationFrame() or setInterval(). I use a more simple playRound() to control sequence of the play in each round. It deals cards and manages the player's turns, then showdown() to calculate the results. The function run to calculate the result card.
# Game Control
My game doesn't use keyboard control. Instead, it uses click event listener for betting the chip and the draw and stay button. Clicking these control changes the selected bet or determined wheter the player draws another card or end the turns.
# Win-lose logic
My game doesn't have physical collision detection, but the showdown() function compares player's hand value and compare it to dealer's hand to determine the winner. The program evaluate card combanation by the Pok Deng rule.
# Scoring
The score is represented by the chip array, which count player's chip balance. chips[i] += delta this code update after each round ended. The delta variable represent chnages in chips based on the showdown(). if (chips[0] < bet) { setStatus('Not enough chips for that bet!'); return; } If the player don't have enough chip, it will return saying 'Not enough chips for that bet!'
# What I noticed
During the game development with Webbgpt, I asked for many version of it, most of those, I asked for python and c++ version, but after testing the python version. The GUI is bad compared to HTML which make me realised that each coding langauge have it own Uniqueness and strength. After some researching, python is diverse and easy but slow because of the compiler needed to preceed heavily. C++ fast and efficient but complex as it is one of the most fastest coding language. HTML is just language that is use to structured display content and needed to use javascript for game or content algorithm. HTML also have CSS is to control the visual design.
# What I learn
I learned how HTML, CSS, and JavaScript work together to create an interactive game. HTML provides the structure, CSS controls the visual design, and Javascript manages the algorithm.
I also learn that not every game have loop as my game don't use it instead it using playround() to start the round but I feel like I wanted to make the game more continuous as I'll add the loop later when I improving the relaibility of the game.
# Goals for this week
1. To improve the reliability of the game: I wanted to change the game into loop to make it continuous as each round is very short.
2. Analyse the game logic: I will review the playRound() and showdown() functions and deeply analyse the code.
# Reflection
Overall, this project helped me understand the use of coding language usage and combanation of it in HTML + CSS + JAVASCRIPT as each langauge have difference strength. I learned that building a game is more than designing visual and algorithm but it also need structure.
# Innovator’s Journal: Developing My Pok Deng Game

## 1. My Development Process

During the development of my Pok Deng game, I used AI as a tool to help me understand and develop the code. Since the game involved many different systems, such as dealing cards, calculating hand values, allowing players to draw or stay, and determining the winner, I found it difficult to understand how every part of the code worked together.

Instead of simply asking AI to generate the entire game, I used it to help me understand the program's structure and the purpose of different sections of code. One method I focused on was using a **flowchart to visualize the logic of the game**. This helped me break a complicated program into smaller steps and understand how the game moves from one stage to another.

## 2. How I Used AI and Improved My Results

My interaction with AI was a process of learning and refinement. Initially, I needed help understanding how the different functions and variables connected. I then focused on understanding the sequence of events in the game rather than looking at the code as one large block.

For example, I examined how the `playRound()` function starts a round, shuffles the deck, distributes cards, and determines whose turn it is. I also explored how `handVal()` calculates a player's hand value and how `showdown()` compares the players' hands against the dealer.

I used these functions as examples to understand the difference between the overall game flow and the smaller calculations that support it. By directing my attention toward specific parts of the program, I could use AI to explain the code in a more understandable way instead of receiving explanations that were too broad.

I also learned that AI-generated code should not automatically be assumed to be correct. I needed to examine the logic, compare the explanations with the actual code, and consider whether the program behaved as intended. This helped me approach AI as a learning assistant rather than a tool that should make every decision for me.

## 3. Using a Flowchart to Understand the Code

One of the most useful techniques I learned was converting the game's logic into a flowchart. A flowchart makes the sequence of actions and decisions easier to understand because it represents the program visually.

For example, the main gameplay process can be represented as follows:

```text
          START GAME
               |
               v
        Choose a bet
               |
               v
       Press the DEAL button
               |
               v
       Check available chips
               |
               v
        Shuffle the deck
               |
               v
       Deal the first cards
               |
               v
       Check for dealer Pok
               |
          +----+----+
          |         |
         Yes        No
          |         |
          v         v
     Skip player   Player's turn
       turns           |
          |             v
          |       Pok already?
          |        +----+----+
          |        |         |
          |       Yes        No
          |        |         |
          |        |         v
          |        |     Draw or Stay
          |        |         |
          +--------+---------+
                   |
                   v
            Bot players' turns
                   |
                   v
             Dealer's turn
                   |
                   v
             Reveal all cards
                   |
                   v
           Compare hand values
                   |
                   v
          Calculate chip changes
                   |
                   v
           Update the scoreboard
                   |
                   v
             More chips left?
              +----+----+
              |         |
             Yes        No
              |         |
              v         v
          Next round   Restart
```

This flowchart helped me understand that a program is not just a collection of individual instructions. The instructions must execute in the correct order, and decisions determine which part of the program runs next.

I also learned that a flowchart can reveal the purpose of a function before I understand every line of its implementation. For example, I can understand that `showdown()` compares hands and updates chips without needing to memorize every JavaScript statement inside it.

## 4. What I Learned About Software and Coding

Through this project, I deepened my understanding of several programming concepts.

First, I learned about **variables and state**. Variables such as `chips`, `bet`, `hands`, and `phase` store information that changes throughout the game. The `phase` variable is particularly important because it helps prevent the player from starting another round while the current round is still in progress.

Second, I learned about **functions and modular programming**. Functions such as `cardVal()`, `handVal()`, `dengInfo()`, and `showdown()` each have specific responsibilities. Separating the program into functions makes the code easier to understand, test, and modify.

Third, I developed a better understanding of **conditional statements and decision-making**. The game uses conditions to determine whether a player has Pok, whether a player should draw another card, and whether a hand wins or loses against the dealer.

Finally, I learned about **asynchronous programming**. The use of `async`, `await`, and `sleep()` allows the game to pause between actions, creating animations and making the gameplay feel more natural. This showed me that programming involves not only calculating correct results but also controlling the timing and sequence of events.

## 5. How I Might Approach Software Development in the Future

In the future, I would approach software development in a more structured way. Before writing code, I would identify the main features of the program and create a flowchart showing how users interact with it and how the program responds.

Next, I would divide the program into smaller functions and develop one feature at a time. I would test each feature before connecting it to the rest of the program. If I used AI, I would ask specific questions about the logic, request explanations of unfamiliar functions, and use the answers to improve my own understanding.

I would also use flowcharts when debugging. If a feature did not work correctly, I could trace the sequence of decisions and identify where the actual behavior differed from the intended behavior. This would help me find the source of a problem instead of randomly changing lines of code.

Overall, this project taught me that successful software development requires more than generating code. It requires planning, logical thinking, testing, and understanding how individual components work together. By combining AI assistance with flowcharts and my own evaluation of the results, I can become more independent and systematic when developing software in the future.
