# TT-TicTacToe

Introduction

  I was tasked with creating a single player tic tac toe game via web application. There was complete freedom
and leeway in choosing the tech stack for implementation. Due to the applications simplicity and some 
familiarity, I felt as though Flask and VueJS were best suited for this application, but due to environmental 
issues I decided to stick with a Jupyter notebook and pygames. 

  The user is welcomed to the homepage with a question asking which game mode, Easy or Hard, would they like to 
play this round. Afterwards, the user is asked which player they would like to be, X starts first for the game. 
Then the fun begins as the game screen is loaded and continues until a winner is found or all positions are 
filled, then the user is asked if they would like to play another round or return home/reset scoreboard. 

Approach

  I approached this task by first running through a tic tic toe game against myself and redrawing the board 
every step. Afterwards, I examined the process to observe at each step what am I checking for before I place my 
next mark, for example, is the space I want available and if it is have I won or gotten any closer to victory. 
After playing against myself and extracting the criteria questions that change the course of the game, I then 
imagined what it would be like to play against a computer that generates its own moves. This led me to figuring 
out that not only do I want a single piece to be added at a time, but also that I would like different levels 
for the computer. The easy level simply chooses a random position based on available positions on board. The 
hard level chooses the computer’s next position by performing a Minimax algorithm on the current board. 


Challenges

  Most of my challenges stemmed from equipment and also trying to prevent overengineering. I initially thought 
that maybe I’d do Django instead of Flask, but due to the web app not needing/utilizing much of Django’s 
extensive let alone basic features, I believe that Flask’s straightforward and easy to implement framework 
works best for my backend needs. I should also note that I only considered these two for backend use because of 
my comfort ability and knowledge in Python is stronger than Javascript. Another reason why I choose Python over 
Javascript was due to the fact that in the beginning stages I was forced to use Google’s Colab as my IDE 
because my laptop was getting fixed, which worked well and ensured that my backend logic alone was solid. 
  Another route I considered for hosting was Github.io/Github Pages. I am familiar with is and think that it’s 
one of the easiest hosting services available but I soon learned that it was due to the fact that it only 
handles static pages. After that realization, I researched various game hosting servers like Socket.io, but 
since my game is a single player, meaning player vs computer, I thought that this route was a little too 
overengineered. I wanted to choose the local server route, but my machine’s RAM couldn’t handle the application 
so Jupyter notebook became the best option for “hosting” my game. 
  Another challenge I’d like to mention due to the nature of this task was implementing the MiniMax Algorithm 
for the Hard level of the game. I say I wanted to mention it because this is a coding challenge for a job 
position and algorithms is typically tested during this process. This was my first time hearing and 
implementing the algorithm and it did remind me of preparing for coding interviews by solving Leetcode 
problems. I started out with visualizing how I go about choosing my next position in tic tac toe, and soon 
realized the pattern, ensuring that my next mark leads me closer to victory while also minimizing my opponents 
chance of victory. From there I researched potential algorithms that would work, and coded a simple recursion 
implementation of the algorithm. 

