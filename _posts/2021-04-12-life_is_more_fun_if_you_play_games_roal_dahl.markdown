---
layout: post
title:      "'Life is more fun if you play games' – Roal Dahl"
date:       2021-04-12 23:18:10 +0000
permalink:  life_is_more_fun_if_you_play_games_roal_dahl
---


All my previous projects created for the school revolved around education, hence for the final project I have decided to do something different. That is one of the reasons why I have created my own version of the Hangman game. This project could prove an invaluable source of entertainment during lockdown ;)

 The CRUD functions allow players to manipulate words or sentences that they chose to play with. Frontend of the game is being handled by the HTML rendering react-redux app. 

The game itself was built using 5 stateless components: MaskedSentece - disguises sentences, Hangman - tracks number of mistakes made by the user, SentenceActions - handles edits & tests routes while WinScreen & LoseScreen are in charge of the user messaging. The app is using react-router and the Redux middleware handles the state change. Async functions combined with redux-thunk are responsible to send and receive data from a server while good old CSS was chosen to provide styling of the game.





