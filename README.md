# Thai-Poker-game
#Autopsy
# 	Where is it in the HTML? What size is it? What do you think happens if you change its width or height?
In my code instead of using HTML <canvas> element. Instead, it uses different HTML elements like <div> to disply the game table, cards, chips, and button
# What values does the game keep track of (position, speed, score, game-over)? Where are they declared?
My game keeps track of the deck of cards, player's hands, dealer's hand, chip balances, bets, current round, and game phase. These variables are declared in the JavaScript code. The main variables include deck, hands, dealerHand, chips, bet, bets, roundN, and phase.
# What function runs over and over? How often (look for requestAnimationFrame or setInterval)? What two things does it do each time it runs?
In my game doesn't contain loop like requestAnimationFrame() or setInterval(). I use a more simple playRound() to control sequence of the play in each round. It deals cards and manages the player's turns, then showdown() to calculate the results. The function run to calculate the result card.
# What key(s) control the game? Find the event listener — what does it actually change when a key is pressed?
My game doesn't use keyboard control. Instead, it uses click event listener for betting the chip and the draw and stay button. Clicking these control changes the selected bet or determined wheter the player draws another card or end the turns.
# How does the game know when something has hit something else, or when the game is over? Find the actual comparison in the code.
My game doesn't have physical collision detection, but the showdown() function compares player's hand value and compare it to dealer's hand to determine the winner. The program evaluate card combanation by the Pok Deng rule.
# Where does the score live(score board), and what line of code changes it?
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
