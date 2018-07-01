---
title: "My First Post"
date: 2018-06-30T01:16:31+01:00
draft: False

Hello All, 

	This is the first post of many to come in a blog that will detail the process, problems, and insights 
I come across as I undertake various projects in data science as well as programming in general. My first pet 
project is the development of a poker game for purpose of familiarizing myself with the python programming language. 

	From the onset I knew that being object oriented, classes would lend themselves very well to representing aspects
 of the game such as a card, player, and a player's hand. This is largely because each of these game pieces has multiple data
members which need to be remembered throughout each round, and there are multiple instances of these objects in play with the 
same type of data members but with different data.

	Once done specifying the classes I went about initiallizing the deck to be used in the game as a set of 52 card objects with numbers 1-13 (Ace = 1, J = 11, Q = 12, K = 13) and with one of four suits. I didn't see a need to add color as a data member as it does not affect the value of the hands in poker. The built in shuffle() (within the Random python library) function as well as pop() were very useful for randomizing the deck and allowing cards to be removed so that they cannot be in two player's hands. 

	Getting the names of the players playing was fairly straight forward and taken as an input, however, the real task in this game is to evaluate who was the winner. In short the method I used assigned every possible hand in poker a ranking based on the type of hand (straight, three of a kind, two pair etc.), as well as the value of cards that compose the hand. The HandRank function returns this rank as an integer and is the part of my script that I am the most proud of. Both the system itself and the helper functions used to implement it are original with the exception of the function that detects whether a  hand contains 2, 3, or 4 of a kind of a card which is loosely based off a function I found that detects whether a set contains duplicates. 

	In order to run the game for multiple rounds with the same players the deck and player card initializations are placed in a while loop which exits when the players no longer want to play.
---

