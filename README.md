# game-design-curriculum

Table of Contents:
 - [What is a Game?](#what-is-a-game)
 - [Games of Chance / Games of Skill](#games-of-chance-vs-games-of-skill)
   - [Solved Games](#solved-games)
 - [Game Balance](#game-balance)
   - [Fairness](#fairness)
   - [Handicapping](#handicapping)
   - [Hidden Information](#hidden-information)
 - [Feedback Loops](#feedback-loops)
   - [Dynamic Game Difficulty Balancing](#dynamic-game-difficulty-balancing)
 - [Probability](#probability)
   - [Independent Probability - Die Rolls / Coin Flips](#independent-probability---die-rolls--coin-flips)
   - [Dependent Probability - Card Draws](#dependent-probability---card-draws)
   - [Problems with Probability](#problems-with-probability)
   - [Pseudo-Random number generation on computers](#pseudo-random-number-generation-on-computers)
   - [Game Theory: Psychology + Games](#game-theory-psychology--games)
   - [Infinite Repetition](#infinite-repetition)
   - [Markov Chain](#markov-chain---probability-between-states)
 - [Reward Systems](#reward-systems)
   - [Calculating Score](#calculating-score)
   - [Multiple Paths to Victory](#multiple-paths-to-victory)
 - [Player Agency](#player-agency)
   - [Bad Decision Design](#bad-decision-design)
   - [Good Decision Design](#good-decision-design)
 - [Rule Symmetry/Asymmetry](#rule-symmetryasymmetry)
   - [Asymmetric Win Conditions](#asymmetric-win-conditions)
 - [Narrative Writing / World Building](#narrative-writing--world-building)
   - [Show Don't Tell](#show-dont-tell)
   - [Sometimes Less Is More](#sometimes-less-is-more)
   - [Elegant Game Design](#elegant-game-design)
 - [Immersiveness and Flow](#immersiveness-and-flow)
 - [Are Video Games Art?](#are-video-games-art)
   - [Art-y Games](#art-y-games)
 - [Interactive Art](#interactive-art)
 - [Serious Games / Games For Change](#serious-games--games-for-change)

## What Is a Game?

What is a Game?: Crash Course Games
[https://www.youtube.com/watch?v=QPqR2wOs8WI](https://www.youtube.com/watch?v=QPqR2wOs8WI)

Why Do We Play Games? by Vsauce
[https://www.youtube.com/watch?v=e5jDspIC4hY](https://www.youtube.com/watch?v=e5jDspIC4hY)

Toys vs games vs puzzles vs simulations

**READ**: My Definition of 'Game' by Chris Crawford
[http://www.erasmatazz.com/library/the-journal-of-computer/jcgd-volume-4/my-definition-of-game.html](http://www.erasmatazz.com/library/the-journal-of-computer/jcgd-volume-4/my-definition-of-game.html)

Chris Crawford is a veteran game designer and founder of the Game Developers Conference (GDC). He's written several book on game design and his 1984 book [The Art of Computer Game Design](https://www.digitpress.com/library/books/book_art_of_computer_game_design.pdf) is  available online. Crawford's hierarchy/taxonomy of games divides interactive entertainment ("intertainments") into 5 categories: Interactive Stories, Toys, Puzzles, Competitions, and Games.

Which category do the following describe?
- challenges without opponents that have clearly defined goals
- interactive playthings, simulations, and sandbox games without defined goals
- challenges with opponents without direct interaction between the competitors
- narratives with limited interaction in which the primary entertainment value is the storyline
- challenges with opponents in which the players (human or A.I.) directly interact in such a way as to foil each other’s goals

3 Minute Game Design: Episode 2 - The Forms
https://www.youtube.com/watch?v=MgyVwFRrzcU

"X" isn’t a game!
[http://www.raphkoster.com/2012/03/13/x-isnt-a-game/](http://www.raphkoster.com/2012/03/13/x-isnt-a-game/) - review Raph Koster's venn diagram of games and digital interactive art

Cow Clicker by Ian Bogost
[http://bogost.com/games/cow_clicker/](http://bogost.com/games/cow_clicker/) - an experiment and deconstructive satire of social games by a Georgia Tech professor

BF Skinner & Positive Reinforcement
[https://www.youtube.com/watch?v=qG2SwE_6uVM&feature=youtu.be&t=430](https://www.youtube.com/watch?v=qG2SwE_6uVM&feature=youtu.be&t=430)







## Games of Chance vs Games of Skill

**Discuss**: What are some games of chance?

How to Win at Candyland
https://www.youtube.com/watch?v=CC9ogJy2bwk

DataGenetics.com "There is no skill required to play Candyland (other than being able to recognise colours)"
http://datagenetics.com/blog/december12011/index.html

**Discuss**: How would YOU improve Candyland?

https://vignette.wikia.nocookie.net/candy-land/images/3/39/Candyland_Game_Board.jpg

Luck and Skill in Games by Skaff Elias
https://youtu.be/2owa2s8GdlM?t=958

**Discuss**: What are some games of skill?

Not enough luck could lead to:
- Analysis Paralysis
- Solved Games
- Being out-matched / out of your league / swimming out of your depth

### Solved Games

List of Solved Games
https://en.wikipedia.org/wiki/Category:Solved_games
- Connect Four
- Checkers
- Tic Tac Toe
- Order and Chaos
- Nim

**TRY IT >>>** Nim
https://www.archimedes-lab.org/game_nim/play_nim_game.html

### Being out of your league / swimming out of your depth

Imagine playing chess against a Grand Master. Imagine boxing Manny Pacquiao or Floyd Mayweather. Imagine serving as goalkeeper against Lionel Messi or Cristiano Ronaldo. You would likely be so out-matched that it would not be a very fun game.

## Game Balance

A **well balanced** game has multiple paths to victory (strategies, items, options, character choice) and no single path is over-powered.

If one path is always an obvious and better choice, most everyone will use the same path and other aspects of the game suffer. It becomes a game of skill and can become solved.

How Games Get Balanced by Game Maker's Toolkit
https://www.youtube.com/watch?v=WXQzdXPTb2A

### Fairness

Essential question: Is the game fair?

This game is not fair | Trap adventures 2
https://www.youtube.com/watch?v=l7JoFDOU7YA

YOU’RE A TROLL! | TRAP ADVENTURE 2 (Adults React: Gaming)
https://www.youtube.com/watch?v=yfftgaedPwg

UNFAIR MARIO (React: Gaming)
https://www.youtube.com/watch?v=nBWimCDEo7o

A game is considered "unfair" if the player has a lack of control of the outcome. This could be cause by:
- too much random chance (War or Candyland)
- an imbalance caused by poor game design (for example, if the first player wins 90% of all games)
- an imbalance caused by a skill gap (being out-matched) or an extreme level of difficulty

### Handicapping

Some games of skill try to make the game more fair by addressing skill gaps using [handicapping](https://en.wikipedia.org/wiki/Handicapping). Handicapping adjusts the difficulty level of the game based on the player's skill level.

Handicapping exists in:
- Horse racing
- Golf
- Chess
- Go
- Shogi
- Gliding
- Polo
- Sailing
- Tennis

Mario Kart addresses skill gaps this with difficulty level ([50cc/100cc/150cc](http://mariokartwii.wikia.com/wiki/CC)), [item distribution](https://www.youtube.com/watch?v=3FU5OJxj75c&feature=youtu.be&t=148), and dynamic game difficulty balancing.

Difficulty Level
https://en.wikipedia.org/wiki/Game_balance#Difficulty_level



### Hidden Information

Analysis paralysis is a problem in which a player is constantly pausing to think about strategy. The game loses it's flow and slows down.

Choice Paralysis - Too Much of a Good Thing by Extra Credits
https://www.youtube.com/watch?v=_2LKrwiGFFs

Games need to be complex enough that they won't be solved, but simple enough that they are learnable. We can't give the player 0% of the information that they need to win (a completely random game) and we can't give them 100% of the infomation (a solved game).

3 Minute Game Design: Episode 3 - How Games Work
https://www.youtube.com/watch?v=R9io0mK-5Ec

Strategic Uncertainty - Keeping Strategy Games Fresh by Extra Credits
https://www.youtube.com/watch?v=PJKTDz1zYzs

3 Minute Game Design: Episode 7 - Hidden Information
https://www.youtube.com/watch?v=UGQ-EZE-NO4

## Feedback Loops

How Games Use Feedback Loops by Game Maker’s Toolkit [https://drive.google.com/open?id=15zZaQHpK1rmnYvJAOOy-b8TyxCgpWhmg](https://drive.google.com/open?id=15zZaQHpK1rmnYvJAOOy-b8TyxCgpWhmg)

One kind of dynamic that is often seen in games and deserves special attention is known as the feedback loop. There are two types, positive feedback loops and negative feedback loops. These terms are borrowed from other fields such as control systems and biology, and they mean the same thing in games that they mean elsewhere.

Positive Feedback Loops reward players for performing well. It is a reinforcing relationship. Something happens that causes the same thing to happen again, which causes it to happen yet again, getting stronger in each iteration – like a snowball that starts out small at the top of the hill and gets larger and faster as it rolls and collects more snow.

Negative feedback loops are, predictably, the opposite of positive feedback loops in just about every way. A negative feedback loop is a balancing relationship. When something happens in the game (such as one player gaining an advantage over the others), a negative feedback loop makes it harder for that same thing to happen again. If one player gets in the lead, a negative feedback loop makes it easier for the opponents to catch up (and harder for a winning player to extend their lead). In racing games, play is more interesting if the player is in the middle of a pack of cars rather than if they are way out in front or lagging way behind on their own (after all, there is more interaction if your opponents are close by). [Source](https://learn.canvas.net/courses/3/pages/level-4-dot-4-feedback-loops)



### Dynamic Game Difficulty Balancing

https://en.wikipedia.org/wiki/Dynamic_game_difficulty_balancing

Rubber Band A.I.
https://www.giantbomb.com/rubber-band-ai/3015-35/

How does Mario Kart incorporate Dynamic Game Difficulty Balancing? What items does a high ranked player receive compared to a low ranked player?

Mario Kart - Rubber Band AI
https://www.youtube.com/watch?v=Zoh5X30Qz-E&feature=youtu.be&t=29

Is Mario Kart Unfair?
https://www.youtube.com/watch?v=3FU5OJxj75c

Is Mario Kart unfair?
https://www.youtube.com/results?search_query=is+mario+kart+unfair

Left 4 Dead has an AI Director system "...which dynamically adjusts the game’s dramatics and pacing along with the difficulty. For example, spawning enemies are appropriately placed and numbered based on the player's current situation." [Source](https://www.hindawi.com/journals/ijcgt/2012/625476/)

"...in Max Payne the game dynamically adjusts the strength of enemies and can also provide different levels of aiming assistance for players" [Source](https://www.hindawi.com/journals/ijcgt/2012/625476/)

## Probability

Randomness provides variety. It is better to generate something random and allow the player to respond to it, rather than make a player's action random.

**Input randomness** informs the player before they make a decision. Typical examples of input randomness would be map generation in Civilization or Rogue. Random face-up tile placement in board game like Catan. People often use the term “procedural generation” to refer to this kind of randomness in digital games.

How (and Why) Spelunky Makes its Own Levels by Game Maker's Toolkit
https://www.youtube.com/watch?v=Uqk5Zf0tw3o

Procedural Generation - How Games Create Infinite Worlds by Extra Credits
https://www.youtube.com/watch?v=TgbuWfGeG2o

**Output randomness** decides an outcome. It is noise injected between the player’s decision and the outcome. Examples would be the dice roll combat in Risk or Memoir ’44, or the random number generation combat in X-Com or FTL. Can be frustrating to a player when their plans fail due to bad luck.

3 Minute Game Design: Episode 6 - Output Randomness by Keith Burgun
https://www.youtube.com/watch?v=2qfFEP_-LkI

The Two Types of Random by Game Maker's Toolkit
https://www.youtube.com/watch?v=dwI5b-wRLic

The Price of Randomness - Balancing RNG by Extra Credits
https://www.youtube.com/watch?v=ry2xz5yYZwY

### Independent Probability - Die Rolls / Coin Flips
Khan Academy - Intro to theoretical probability
https://www.youtube.com/watch?v=uzkc-qNVoOk

Khan Academy - Theoretical and experimental probability: Coin flips and die rolls
https://www.khanacademy.org/math/ap-statistics/probability-ap/randomness-probability-simulation/a/theoretical-and-experimental-probability-coin-flips-and-die-rolls

1 coin = 2 equally likely possibilities
2 coins = 4 equally likely possibilities
3 coins = 8 equally likely possibilities

- With one die (aka 1d6), what is the prob. of rolling 1?
- With two coins (2d2), what is the prob. of flipping heads & heads?
- With two dice (2d6), what is the prob. of rolling doubles?
- With two dice, what is the prob. of rolling 12?
- With two dice, what is the prob. of rolling 6?
- With two dice, what is the prob. of rolling 1?
- With two dice, what is the prob. of rolling 7?
- With six coins (6d2), what is the prob. of flipping 1 heads & 5 tails?

### Dependent Probability - Card Draws
Khan Academy - Dependent probability introduction
https://www.youtube.com/watch?v=VjLEoo3hIoM
- With a 52-card deck, what is the prob. of drawing 2 Aces?
- With a 52-card deck, what is the prob. of drawing 2 hearts?
- With a 52-card deck, what is the prob. of drawing 2 face cards (J, Q, or K)?

### Problems with Probability
Humans are not always rational

The Monty Hall Problem - Human Perception can be skewed
Monty Hall Problem - Numberphile
https://www.youtube.com/watch?v=4Lb-6rxZxx0

Try to predict the probability for ANY 1-12 on two dice (for example, rolling a 1 and a 2 counts as rolling 1, 2, AND 3)

Liar's Dice - Probability mixed with Bluffing and Hidden Information (see also: Poker)
https://www.youtube.com/watch?v=SRI_Yvze2ms

### Pseudo-Random number generation on computers

Most of the time, we don't need to produce actually random numbers. They just need to seem random. Sequences of pseudo-random numbers look like sequences of genuinely random numbers and have many of the statistical properties associated with random numbers, but they are actually produced using a deterministic process, that is they follow a set rule, a pattern.

How to Generate Pseudorandom Numbers by PBS Infinite Series
https://www.youtube.com/watch?v=C82JyCmtKWg

### Game Theory: Psychology + Games

- The Risk Game - I will give you 50 points now or we can flip a coin and you get 0/100 points
- Loss Aversion Game - We flip a coin and you get -50/100 points. Play or not?
- The Ultimatum Game - 2 players, p1 gets 100 points to split, p2 gets to accept or decline
- Split or Steal - Both split 200, one steals 200, or both steal nothing
- Press Your Luck - I will give you 100 points for each heads, but you bust on tails
- The Risk Game - I will give you 40 points now or we can flip a coin and you get 0/100 points
- Loss Aversion Game - We flip a coin and you get -100/100 points. Play or not?

Prisoners' dilemma and Nash equilibrium | Microeconomics | Khan Academy
https://www.youtube.com/watch?v=UkXI-zPcDIM

Prisoner's Dilemma in [Trivia Murder Party](https://jackboxgames.fandom.com/wiki/Trivia_Murder_Party) by Jackbox. A pile of money is in the middle of the floor. The player can choose to take it or not. If nobody takes the money, nobody dies. If anyone takes the money, everyone who didn’t will die. Players that take the money split $2000. If everyone takes the money, everyone dies.
https://drive.google.com/open?id=1uHGm9jZqNHmXKu6Suk2njpYBVKolKqIU

TRY IT >>> The Evolution of Trust (The Prisoner's Dilemma) by Nicky Case https://ncase.me/trust/

The Prisoner's Dilemma - The Game Theory of Decision-Making by Extra Credits
https://www.youtube.com/watch?v=K5TRstDfQDg

Golden Balls split or steal
https://www.youtube.com/results?search_query=golden+balls+split+or+steal

Game Theory: The Science of Decision-Making
https://www.youtube.com/watch?v=MHS-htjGgSY

Psychology of Gaming: Crash Course Games
https://www.youtube.com/watch?v=MYJBRWT7JGU

7 ways games use psychology to control you
https://www.youtube.com/watch?v=A2gIE5gyA6s


### Infinite Repetition
Monte Carlo Simulation - repeat a random trial a few thousand/million times

Khan Academy - Experimental versus theoretical probability simulation
https://www.youtube.com/watch?v=Nos-xOCpQqg

Coin flip simulator
http://digfir-published.macmillanusa.com/stats_applet/stats_applet_10_prob.html

### Markov Chain - probability between states

A Markov Chain is a finite state machine that moves from one state to another according to certain probabilistic rules. Markov Chains can be used to model the probabilities of game states.

Games are finite state machines. There are a set number of game states. The game is not infinite. 

A **finite state machine** is hardware or software that moves through a series of modes and can only be in one mode at a time. A traffic light is a common example of a finite state machine. 

Discuss: Give me an example of a finite state machine (hardware device or software) and describe a few of its states.

botnik.org's Harry Potter and the Portrait of what Looked Like a Large Pile of Ash
https://www.youtube.com/watch?v=x-uDnlGJRdk

Origin of Markov chains | Journey into information theory | Computer Science | Khan Academy
https://www.youtube.com/watch?v=Ws63I3F7Moc

Probabilities in the Game of Monopoly
http://www.tkcs-collins.com/truman/monopoly/monopoly.shtml#Markov

Analysis of Candyland, Chutes & Ladders, etc. by datagenetics.com
- Chuttes and Ladders http://www.datagenetics.com/blog/november12011/index.html
- Risk http://datagenetics.com/blog/november22011/index.html
- Candyland http://datagenetics.com/blog/december12011/index.html
- Battleship http://www.datagenetics.com/blog/december32011/index.html
- Darts http://www.datagenetics.com/blog/january12012/index.html
- Yahtzee http://datagenetics.com/blog/january42012/index.html
- Hangman http://www.datagenetics.com/blog/april12012/index.html
- Minesweeper http://datagenetics.com/blog/june12012/index.html


The Best Mario Kart Character According to Data Science

https://medium.com/civis-analytics/the-best-mario-kart-character-according-to-data-science-7dfb65d4c18e


## Reward Systems
When should we schedule rewards?
Cookie Clicker and Farmville psychologically manipulate players to keep playing

### Calculating Score
How can you make the player's score go down with time?


### Multiple Paths to Victory

 Discuss: What are some games with multiple victory conditions?
 
Multiple Paths to Victory
https://lanepushinggames.com/article/killer-queen-thoughts-on-multiple-victory-conditions

Multiple victory or loss conditions. For example, a round of Pokémon Trading Card Game can end in three ways... [Source](https://en.wikipedia.org/wiki/Game_mechanics#Combination_conditions):
- When one player has Knocked Out enough of the other's Pokémon to draw all his Prize Cards
- When one player is unable to play a Pokémon from his Bench to replace his Active Pokémon
- When one player has run out of cards in his Deck and is unable to draw at the beginning of his turn.



## Player Agency

FPS Level Design - "...it is always advantageous for the player to have a number of paths to get to and from every major area in a multiplayer map."
https://www.ongamedesign.net/designing-fps-multiplayer-maps-part-1/

Agency (sociology) - the capacity of individuals to act independently and to make their own free choices
https://en.wikipedia.org/wiki/Agency_(sociology)

Player Agency: How Game Design Affects Narrative
https://www.gamasutra.com/blogs/JoshBycer/20150126/234961/Player_Agency_How_Game_Design_Affects_Narrative.php


Decisions are, in essence, what players do in a game. Remove all decisions and you have a movie or some other linear activity, not a game. As pointed out in Challenges, there are two important exceptions, games which have no decisions at all: some children’s games and some gambling games.

### Bad Decision Design

Source: [https://learn.canvas.net/courses/3/pages/level-6-dot-1-tips-on-decision-making?module_item_id=44557](https://learn.canvas.net/courses/3/pages/level-6-dot-1-tips-on-decision-making?module_item_id=44557)

Before describing good kinds of decisions, it is worth explaining some common kinds of uninteresting decisions commonly found in games.

**Meaningless decisions** are perhaps the worst kind: there is a choice to be made, but it has no effect on gameplay. If you can play either of two cards but both cards are identical, that’s not really much of a choice.

**Obvious decisions** at least have an effect on the game, but there is clearly one right answer, so it’s not really much of a choice. Most of the time, the number of dice to roll in the board game RISK falls into this category; if you are attacking with 3 or more armies, you technically have a "decision" of whether to roll 1, 2, or 3 dice… but your odds are MUCH, MUCH better rolling all 3, so it’s not much of a decision. You roll 3.

**Blind decisions** have an effect on the game, and the answer is not obvious, but there is now an additional problem: the players do not have sufficient knowledge on which to make the decision, so it is essentially random. Playing Rock-Paper-Scissors against a truly random opponent falls into this category; your choice affects the outcome of the game, but you have no way of knowing what to choose.

### Good Decision Design

Source: [https://learn.canvas.net/courses/3/pages/level-6-dot-1-tips-on-decision-making?module_item_id=44557](https://learn.canvas.net/courses/3/pages/level-6-dot-1-tips-on-decision-making?module_item_id=44557)

Now that we know what makes weak decisions, the easiest answer is "don’t do that!" But we can take it a little further. Generally, interesting decisions involve some kind of tradeoff. That is, you are giving up one thing in exchange for another.

**Resource trades**: You give one thing up in exchange for another, where both are valuable. Which is more valuable? This is a value judgment, and the player’s ability to correctly judge or anticipate value is what determines the game’s outcome.

**Risk versus reward**: One choice is safe. The other choice has a potentially greater payoff, but also a higher risk of failure. Whether you choose safe or dangerous depends partly on how desperate a position you’re in, and partly on your analysis of just how safe or dangerous it is. The outcome is determined by your choice, plus a little luck… but over a sufficient number of choices, the luck can even out and the more skillful player will generally win. (Corollary: if you want more luck in your game, reduce the total number of decisions.)

**Choice of actions**: You have several potential things you can do, but you can’t do them all. The player must choose the actions that they feel are the most important at the time.

**Short term versus long term**: You can have something right now, or something better later on. The player must balance immediate needs against long-term goals.

**Social information**: In games where bluffing, deal-making and backstabbing are allowed, players must choose between playing honestly or dishonestly. Dishonesty may let you come out better on the current deal, but may make other players less likely to deal with you in the future. In the right (or wrong) game, backstabbing your opponents may have very negative real-world consequences.

**Dilemmas**: You must give up one of several things. Which one can you most afford to lose?


## Rule Symmetry/Asymmetry

Rule Symmetry means that all players share the same goals, rules, victory conditions.

Rule Asymmetry means that some players have different goals, rules, victory conditions.

The rules are different for goalies compared to other hockey players, but this does not mean that ice hockey is an asymmetric game. Both teams share the same goals, rules, and victory conditions. It would only be asymmetric if one team were all-time offense and the other team all-time defense.

### Asymmetric Win Conditions
Common styles of asymmetric games:
- social deduction games (hidden loyalty games) such as Werewolf, The Resistance, Two Rooms and a Boom, Spyfall, Saboteur, A Fake Artist Goes to New York, or Battlestar Galactica. In these games, asymmetry is critical because it facilitates deduction of a player's hidden allegiance based on how they act.
- chase games, such as Scotland Yard, Mr. Jack, Fury of Dracula, or freeze tag. In these games, the primary game activity is inherently asymmetric.
- one-versus-many games, such as Betrayal at House on the Hill, Descent, Dead of Winter, or Mansions of Madness (first edition), which I suspect are mostly offshoots of tabletop RPGs (such as D&D) and so have inherited the concept of an "adventuring party". You could also look at these as cooperative games where the "game system" has been expanded into an actual player role. Ultimately, I think this model derives from traditional storytelling--their asymmetry results from the fact that one side is "protagonists" and the other is "antagonists".

[Source](https://boardgamegeek.com/article/27705805#27705805)

BANG! is an asymmetric card game:
- Sheriff and Deputies: Win if all outlaws and renegade dead, sheriff still alive.
- Outlaws: Win if Sheriff dead.
- Renegade: All players dead but himself. The game ends when the sheriff dies, so the renegade only wins if he kills the sheriff last.

[Source](https://boardgamegeek.com/geeklist/24128/item/480422#item480422)

Overwatch and Asymmetric Level Design - What Makes the Maps Fun? by Extra Credits
https://www.youtube.com/watch?v=4DynhzEQtog

Overwatch and Asymmetric Character Design - The Challenge of Varied Playstyles by Extra Credits
https://www.youtube.com/watch?v=NEpeGSFQ1tM

## Narrative Writing / World Building

How the inventor of Mario designs a game (Level 1 - The Story)
https://youtu.be/K-NBcP0YUQI?t=58

> Miyamoto based the story on the love triangle in Popeye between a bad guy, a hero, and a damsel in distress. But since Nintendo couldn’t secure the rights to use those characters, Miyamoto replaced them with a gorilla, a carpenter, and his girlfriend. In later games, that carpenter became a plumber. And his named changed, from Mr. Video, to Jumpman, and then to Mario, after this guy, the landlord of a Nintendo warehouse near Seattle.This was one of the first times that a video game’s plot and characters were designed before the programming. That change in approach came at a key time for video games. When Donkey Kong was first released in 1981, the video game market in North America was on the verge of collapse. It was saturated with a lot of different consoles, and the boom in home computers made a lot of people question why they’d want a separate device just to play games. But the storytelling in games like Super Mario Bros. and The Legend of Zelda — which you could only play on Nintendo's own hardware — helped set them apart as best-sellers.

How to Create a Video Game World
– Determine the Scope of Your World
– Develop a Backstory for This World
– Create a Culture and a System of Order
– Create Items for Your World
– Draw Out the Layout of This World

[Source](https://www.emwelsh.com/blog/video-game-world)

In Medias Res - Latin for "into the middle of things." Beginning the story with action. For example, "Where's Papa going with that ax?" This is preferable when compared to a boring intro giving the entire backstory.
https://en.wikipedia.org/wiki/In_medias_res

Exposition - From Latin, meaning "a showing forth." Introducing background info about events, settings, characters, etc to the audience/readers. In other words, backstory. For example, "A long time ago in a galaxy far away, far away…" Too much exposition is generally considered a bad thing.
https://en.wikipedia.org/wiki/Exposition_(narrative)

Exposition is a two-edged sword. While it is extremely useful for establishing setting, plot, and characterization, too much exposition at once can bog down a story and slow the pace to a crawl. An exposition that is overly long or wordy is known as an Information Dump (or Info Dump for short) and is very difficult to do well. Source: https://tvtropes.org/pmwiki/pmwiki.php/Main/Exposition

More Than Exposition - Building Worlds without Info Dumps by Extra Credits
https://www.youtube.com/watch?v=TEERJ1a2rsU

### First Level Design

You should be able to say, "Everything I needed to know about the game, I learned from the first level." The player should be able to infer the basic moves of the game, the mood and feel of the game, the culture of the world, etc.

How the inventor of Mario designs a game (Level 2 - Simplicity)
https://youtu.be/K-NBcP0YUQI?t=170

> A lot of Miyamoto’s genius can be seen in the first level of Super Mario Bros. — probably the most iconic level in video game history. It’s designed to naturally teach you the game mechanics while you play. If you look at a breakdown, there’s a lot of really subtle design work going on here. Though Mario is usually at the center of the screen, in this first scene he starts at the far left. All the empty space to the right of him gives you a sense of where to go. This character’s look and movement suggest it’s harmful. But don’t worry. If you run into it, you’ll just start the game over without much of a penalty. Next, you see gold blocks with question marks. These are made to look intriguing — and once you hit one, you’re rewarded. That then encourages you to hit the second block, which releases a mushroom. Even if you’re now scared of mushrooms, the positioning of the first obstacle makes it just about guaranteed that you're gonna run into this thing. When you do, Mario gets bigger and stronger. And just like that, you’ve learned all the basic rules in the game without having to read a single word.

How Level Design Can Tell a Story by Game Maker's Toolkit
https://www.youtube.com/watch?v=RwlnCn2EB9o

Tutorials That Don't Talk Down To You - Context Sensitive Design by Extra Credits
https://www.youtube.com/watch?v=hFdEEzgc7pg

Teach players the mechanics by "showing" them, not "telling" them.

Half-Life 2's Invisible Tutorial | Teaching Players by Game Maker's Toolkit https://www.youtube.com/watch?v=MMggqenxuZc

### Show Don't Tell

"Show, Don't Tell" - Advice that narrative writing should show actions, relationships, and feelings instead of just directly telling the reader what happened. Too much exposition is generally considered a bad thing.
https://en.wikipedia.org/wiki/Show,_don%27t_tell

Mechanics Shaping Story - Re-examining the Core Gameplay Loop by Extra Credits
https://www.youtube.com/watch?v=f5I6uo39ujQ

God of War and the Mechanics of an Epic Story (No Spoilers) by NIKMOE
https://www.youtube.com/watch?v=wCB1JOcJHOE

Storytelling Tools to Boost Your Indie Game's Narrative and Gameplay
https://youtu.be/8fXE-E1hjKk?t=826

### Sometimes Less Is More

> "I'd like to go with as little story as possible," he (Shigeru Miyamoto) said. "I've always felt that the Mario games themselves aren't particularly suited to having a very heavy story." The Legend of Zelda games, he feels, should have deep storylines – but not Mario. [Source](https://www.wired.com/2009/06/super-mario-galaxy-2/)

Using Narrative as Context - Balancing Gameplay and Story Elements by Extra Credits
https://www.youtube.com/watch?v=Izk-e0WrjP0

> 	"Perfection is achieved, not when there is nothing more to add, but when there is nothing left to take away" - Antoine de Saint-Exupéry

Information Density - How Mr. Robot Does a Lot with a Little by Extra Credits
https://www.youtube.com/watch?v=ghrI2Vb8u2U

### Elegant Game Design

An elegant game is simple (not complex) and clever, yet has depth of play with multiple paths available.

3 Minute Game Design: Episode 4 - Elegance and Depth
https://www.youtube.com/watch?v=IMsFHCdqjTk

Game Complexity - the mental burden put on the player by the game. This includes information the player has to remember, rules they have to process, and calculations they have to make to make a meaningful choice.

BoardGameGeek.com has Complexity ratings for board and card games. Some of [the least complex games](https://boardgamegeek.com/geeksearch.php?action=search&advsearch=1&objecttype=boardgame&q=&include%5Bdesignerid%5D=&geekitemname=&geekitemname=&include%5Bpublisherid%5D=&range%5Byearpublished%5D%5Bmin%5D=&range%5Byearpublished%5D%5Bmax%5D=&range%5Bminage%5D%5Bmax%5D=&floatrange%5Bavgrating%5D%5Bmin%5D=&floatrange%5Bavgrating%5D%5Bmax%5D=&range%5Bnumvoters%5D%5Bmin%5D=&floatrange%5Bavgweight%5D%5Bmin%5D=&floatrange%5Bavgweight%5D%5Bmax%5D=1.2&range%5Bnumweights%5D%5Bmin%5D=500&colfiltertype=&searchuser=20hz20khz&range%5Bminplayers%5D%5Bmax%5D=&range%5Bmaxplayers%5D%5Bmin%5D=&playerrangetype=normal&range%5Bleastplaytime%5D%5Bmin%5D=&range%5Bplaytime%5D%5Bmax%5D=&B1=Submit) include The Game of Life, Yahtzee, and UNO. Some of [the most complex games](https://boardgamegeek.com/search/boardgame?sort=numvoters&advsearch=1&q=&include%5Bdesignerid%5D=&include%5Bpublisherid%5D=&geekitemname=&range%5Byearpublished%5D%5Bmin%5D=&range%5Byearpublished%5D%5Bmax%5D=&range%5Bminage%5D%5Bmax%5D=&range%5Bnumvoters%5D%5Bmin%5D=&range%5Bnumweights%5D%5Bmin%5D=500&range%5Bminplayers%5D%5Bmax%5D=&range%5Bmaxplayers%5D%5Bmin%5D=&range%5Bleastplaytime%5D%5Bmin%5D=&range%5Bplaytime%5D%5Bmax%5D=&floatrange%5Bavgrating%5D%5Bmin%5D=&floatrange%5Bavgrating%5D%5Bmax%5D=&floatrange%5Bavgweight%5D%5Bmin%5D=3&floatrange%5Bavgweight%5D%5Bmax%5D=&colfiltertype=&searchuser=20hz20khz&playerrangetype=normal&B1=Submit) include Magic: The Gathering (1993), Chess (1475), Civilization (1980).

Game Depth - the number of meaningful choices that the player has available. For example, Tic-Tac-Toe is a low depth game because its rules don't create many different possibilities for the player.

Elegant Game Design - is design with a high depth to complexity ratio. Few rules to learn, but many possibilities. For example, the game Go.

Depth vs Complexity - Why More Features Don't Make a Better Game - Extra Credits
https://www.youtube.com/watch?v=jVL4st0blGU


## Immersiveness and Flow

> All forms of entertainment strive to create *suspension of disbelief*, a state in which the … mind forgets that it is being subjected to entertainment and instead accepts what it perceives as reality. - François Dominic Laramée; ‘Immersion’

Definition of immersive: providing, involving, or characterized by deep absorption or immersion in something (such as an activity or a real or artificial environment) [Source](https://www.merriam-webster.com/dictionary/immersive)

> The game is incredibly *immersive*, with stunning 3-D graphics and an excellent array of sound effects that bring the Star Trek universe to life. — Newsweek

How the inventor of Mario designs a game (Level 3 - Immersiveness)
https://youtu.be/K-NBcP0YUQI?t=243

Immersiveness in a video game has a lot to do with the controls — the more precisely you can move your character, the more you feel like you’re part of the story.

The Magic Circle - How Games Transport Us to New Worlds - Extra Credits
https://www.youtube.com/watch?v=qZ-EY9gTsgU

## Are Video Games Art?

Roger Ebert "Video games can never be art"
[https://www.rogerebert.com/rogers-journal/video-games-can-never-be-art](https://www.rogerebert.com/rogers-journal/video-games-can-never-be-art)
[https://www.eurogamer.net/articles/news301105ebert](https://www.eurogamer.net/articles/news301105ebert)


"I am prepared to believe that video games can be elegant, subtle, sophisticated, challenging and visually wonderful. But I believe the nature of the medium prevents it from moving beyond craftsmanship to the stature of art. To my knowledge, no one in or out of the field has ever been able to cite a game worthy of comparison with the great dramatists, poets, filmmakers, novelists and composers. That a game can aspire to artistic importance as a visual experience, I accept. But for most gamers, video games represent a loss of those precious hours we have available to make ourselves more cultured, civilized and empathetic."
 - Roger Ebert [Source](https://www.rogerebert.com/answer-man/why-did-the-chicken-cross-the-genders)



Hideo Kojima (Metal Gear Solid) "I don't think they're art either, videogames."
[https://www.eurogamer.net/articles/news240106kojimaart](https://www.eurogamer.net/articles/news240106kojimaart)

Game Rules as Art
[http://www.escapistmagazine.com/articles/view/video-games/issues/issue_41/247-Game-Rules-as-Art](http://www.escapistmagazine.com/articles/view/video-games/issues/issue_41/247-Game-Rules-as-Art)

### Art-y Games

Braid by Jonathan Blow
[https://www.youtube.com/watch?v=u7C1qxggPHg](https://www.youtube.com/watch?v=u7C1qxggPHg)
[https://www.youtube.com/watch?v=2zK8ItePe3Y](https://www.youtube.com/watch?v=2zK8ItePe3Y)

Flow by Jenova Chen
http://interactive.usc.edu/projects/cloud/flowing/

Journey, Flower and Flow (re-released) by Thatgamecompany (founded by Jenova Chen and Kellee Santiago)
[http://thatgamecompany.com/](http://thatgamecompany.com/)

Journey Trailer
[https://www.youtube.com/watch?v=5NlVttFRPpU](https://www.youtube.com/watch?v=5NlVttFRPpU)

Flower Trailer
[https://www.youtube.com/watch?v=U7IUDWMU6ZI](https://www.youtube.com/watch?v=U7IUDWMU6ZI)

A Slow Year by Ian Bogost
[http://bogost.com/games/aslowyear/](http://bogost.com/games/aslowyear/)

A Slow Year from Ian Bogost on Vimeo
[https://vimeo.com/9592601](https://vimeo.com/9592601)

Walden, A Game by USC Game Innovation Lab
[http://www.gamesforchange.org/game/featured-game-3/](http://www.gamesforchange.org/game/featured-game-3/)

That Dragon, Cancer by Numinous Games
[http://www.gamesforchange.org/game/that-dragon-cancer/](http://www.gamesforchange.org/game/that-dragon-cancer/)

Games by Daniel Benmergui
[http://ludomancy.com/](http://ludomancy.com/)

Today I Die by Daniel Benmergui
[http://www.ludomancy.com/games/today.php?lang=en](http://www.ludomancy.com/games/today.php?lang=en)

I Wish I Were The Moon by Daniel Benmergui
[http://www.kongregate.com/games/danielben/i-wish-i-were-the-moon](http://www.kongregate.com/games/danielben/i-wish-i-were-the-moon)

Papa Sangre by Somethin' Else
[http://boingboing.net/2010/12/19/papa-sangre-binaural.html](http://boingboing.net/2010/12/19/papa-sangre-binaural.html)
[http://www.somethinelse.com/projects/gaming-for-gamers-audio-games/](http://www.somethinelse.com/projects/gaming-for-gamers-audio-games/)

Entering the Palace of Bones from Papa Sangre on Vimeo
[https://vimeo.com/9916119](https://vimeo.com/9916119)

Façade by Michael Mateas and Andrew Stern
[http://www.playabl.ai/past-work/](http://www.playabl.ai/past-work/)

The Marriage by Rod Humble
[http://www.rodvik.com/rodgames/marriage.html](http://www.rodvik.com/rodgames/marriage.html)

Passage by Jason Rohrer
[http://hcsoftware.sourceforge.net/passage/](http://hcsoftware.sourceforge.net/passage/)

Gravitation by Jason Rohrer
[http://hcsoftware.sourceforge.net/gravitation/](http://hcsoftware.sourceforge.net/gravitation/)

### Arcane Kids
[https://en.wikipedia.org/wiki/Arcane_Kids](https://en.wikipedia.org/wiki/Arcane_Kids)

Bubsy 3D: Bubsy Visits the James Turrell Retrospective by Arcane Kids
[https://www.youtube.com/watch?v=-qJflQ3srSo](https://www.youtube.com/watch?v=-qJflQ3srSo)
[https://www.youtube.com/watch?v=z14U33GFLEI](https://www.youtube.com/watch?v=z14U33GFLEI)

Sonic Dreams Collection
[https://www.youtube.com/watch?v=Jd9pIR1hCJY](https://www.youtube.com/watch?v=Jd9pIR1hCJY)

Anamanaguchi's Capsule Silence XXIV
[https://www.youtube.com/watch?v=ZCNhkNL5ti8&feature=youtu.be&t=950](https://www.youtube.com/watch?v=ZCNhkNL5ti8&feature=youtu.be&t=950)

## Interactive Art

Yayoi Kusama’s "Obliteration Room"
[http://www.wired.com/beyond_the_beyond/2012/03/showtime-yayoi-kusama-obliteration-room/](http://www.wired.com/beyond_the_beyond/2012/03/showtime-yayoi-kusama-obliteration-room/)

Yayoi Kusama’s “Infinity Dots”
http://nymag.com/travel/weekends/pittsburgh/index2.html

Andy Warhol's Silver Clouds
https://youtu.be/QpCOp5TPOkI?t=45

Toledo Museum of Art, Play Time
https://www.youtube.com/watch?v=8ci393bTuy8
https://www.youtube.com/watch?v=0MCIdnzAJ0o
https://www.youtube.com/watch?v=shwjITmIXWA

Amazing Art Installation Turns You Into A Bird | Chris Milk "The Treachery of Sanctuary"
https://www.youtube.com/watch?v=I5__9hq-yas&feature=youtu.be&t=444

Interactive Art: Playing with Light
https://www.youtube.com/watch?v=y-lOAoWcAV8
Interactive Art Pushes Boundaries of Viewer, Artist
http://www.wired.com/gadgetlab/2009/10/utterback/

Reactive Sparks: Interactive LED Art Responds to Traffic
http://technabob.com/blog/2008/03/28/reactive-sparks-interactive-led-art-responds-to-traffic/

“Guitar Pedals” by David Byrne
http://davidbyrne.com/art/guitar_pedals/

Sleep No More: Interactive Theatre
http://www.coolhunting.com/culture/sleep-no-more.php
http://gizmodo.com/5912789/sleep-no-more-what-its-like-inside-the-worlds-most-interactive-play

Eko: an interactive storytelling platform that lets viewers shape stories as they are told
https://helloeko.com/

Bad Trip by Alan Kwan
http://www.thecreatorsproject.com/blog/explore-someone-elses-mind-using-a-video-game-controller

http://www.fastcodesign.com/1670801/creepy-video-game-lets-you-explore-its-makers-memories

Bad Trip: Navigate My Mind from KwanAlan on Vimeo
https://vimeo.com/47943812

## Serious Games / Games For Change

Monopoly, the World's Best-Selling Game
[https://blog.ncase.me/i-do-and-i-understand/](https://blog.ncase.me/i-do-and-i-understand/)

Candyland Was Invented for Polio Wards
[https://www.theatlantic.com/technology/archive/2019/07/how-polio-inspired-the-creation-of-candy-land/594424/](https://www.theatlantic.com/technology/archive/2019/07/how-polio-inspired-the-creation-of-candy-land/594424/)

Dumb Ways To Die by McCann
[http://www.gamesforchange.org/game/dumb-ways-to-die/](http://www.gamesforchange.org/game/dumb-ways-to-die/)

Lim by Merritt Kopas
[http://www.gamesforchange.org/game/lim/](http://www.gamesforchange.org/game/lim/)
[https://www.youtube.com/watch?v=Dr0LdXhSnFk](YouTube review of Lim)

Foldit by University of Washington
[http://www.gamesforchange.org/game/foldit/](http://www.gamesforchange.org/game/foldit/)

Zombies, Run! by Six to Start
[http://www.gamesforchange.org/game/zombies-run/](http://www.gamesforchange.org/game/zombies-run/)

Unity Games For Change Challenge
https://blogs.unity3d.com/2018/07/25/making-games-for-change/

The Dad That Hacked Into Donkey Kong for his Daughter
[https://www.youtube.com/watch?v=XFS_xn-EpRY](https://www.youtube.com/watch?v=XFS_xn-EpRY)

Creating Games with a Purpose
[https://www.youtube.com/watch?v=QCCFaWnBDlM](https://www.youtube.com/watch?v=QCCFaWnBDlM)

Depression Quest by Zoë Quinn, Patrick Lindsey, and music by Isaac Schankler
[http://www.depressionquest.com/](http://www.depressionquest.com/)

"Depression Quest is the most important game I’ve ever played" by Mark Chen
[http://depts.washington.edu/critgame/project/depression-quest-is-the-most-important-game-ive-ever-played/](http://depts.washington.edu/critgame/project/depression-quest-is-the-most-important-game-ive-ever-played/)

Papers, Please
[http://www.slate.com/blogs/future_tense/2013/08/23/papers_please_serious_video_game_raises_tricky_moral_questions.html](http://www.slate.com/blogs/future_tense/2013/08/23/papers_please_serious_video_game_raises_tricky_moral_questions.html)

Darfur is Dying
[http://www.darfurisdying.com/](http://www.darfurisdying.com/)

Sweatshop
[http://www.gamesforchange.org/game/sweatshop/](http://www.gamesforchange.org/game/sweatshop/)

This War of Mine by 11 bit studios
[http://www.gamesforchange.org/game/this-war-of-mine/](http://www.gamesforchange.org/game/this-war-of-mine/)

### Nicky Case
https://ncase.me/

Parable of the Polygons by Nicky Case & Vi Hart
[http://www.gamesforchange.org/game/parable-of-the-polygons/](http://www.gamesforchange.org/game/parable-of-the-polygons/)

To Build A Better Ballot
https://ncase.me/ballot/

The Evolution of Trust (The Prisoner's Dilemma)
https://ncase.me/trust/




## Recommended YouTube channels for additional information

Crash Course Games
https://www.youtube.com/watch?v=QPqR2wOs8WI&list=PL8dPuuaLjXtPTrc_yg73RghJEOdobAplG

Wired Game|Life
https://video.wired.com/series/game-life

PBS Game/Show
https://www.youtube.com/channel/UCr_2H8pPitVJ85bmpLwFUyQ

Game Maker's Toolkit
https://www.youtube.com/user/McBacon1337
