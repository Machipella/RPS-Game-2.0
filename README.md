# RPS-Game-2.0
I improved the old version of the RPS game I had developed before.
Here is the code:
#Simple 2-player Rock, Paper, Scissors game 
# #Here is the Code: 
print("ROCK🥔 PAPER📃 SCISSORS✂ BATTLE")

#Game Loop, players can restart the game if they want
while True:
    score1 = 0
    score2 = 0

#Option to play until someone reaches 3 
    while score1 < 3 and score2 < 3:
        player1_move = input("Player 1, Please select your move (Rock, Paper,Scissors:)") 
        print ("Player 1 has chosen:", player1_move)

        player2_move = input("Player 2, Please select your move (Rock, Paper,Scissors:)") 
        print ("Player 2 has chosen:", player2_move) 
    #GameLogic
            #Player1Conditions
        if player1_move == player2_move: 
            print("It's a tie! 😐") 
        elif (player1_move == "Rock" and player2_move == "Scissors"): 
            print("Player 1 wins! 🎉😎") 
            score1 += 1
        elif (player1_move == "Paper" and player2_move == "Rock") : 
            print("Player 1 wins! 🎉😎") 
            score1 += 1
        elif (player1_move == "Scissors" and player2_move == "Paper"): 
            print("Player 1 wins! 🎉😎") 
            score1 += 1

                #Player2Conditions 
        elif (player2_move == "Rock" and player1_move == "Scissors"): 
            print("Player 2 wins! 🎉😎") 
            score2 +=1
        elif (player2_move == "Paper" and player1_move == "Rock"): 
            print("Player 2 wins! 🎉😎") 
            score2 +=1
        elif (player2_move == "Scissors" and player1_move == "Paper"): 
            print("Player 2 wins! 🎉😎") 
            score2 += 1

        else: 
            print("Invalid input! Please choose rock, paper, or scissors")

    #Show Scores after each round
        print(f"Score: Player 1 = {score1}, Player 2 = {score2}\n")
        # End of match
    if score1 == 3:
            print("🎊 Player 1 WINS the match! 🎊")
    else:
            print("🎊 Player 2 WINS the match! 🎊")

        # Ask if players want to restart
    play_again = input("Do you want to play again? (yes/no): ").lower()
    if play_again != "yes":
        print("Thanks for playing! Goodbye 👋")
        break
        





