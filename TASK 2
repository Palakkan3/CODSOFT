import random

def get_user_choice():
    """Prompt the user to choose Rock, Paper, or Scissors and return their choice."""
    while True:
        print("\nChoose one: Rock, Paper, Scissors")
        user_choice = input("Your choice: ").strip().lower()
        if user_choice in ['rock', 'paper', 'scissors']:
            return user_choice
        else:
            print("Invalid choice! Please choose Rock, Paper, or Scissors.")

def get_computer_choice():
    """Randomly select Rock, Paper, or Scissors for the computer."""
    return random.choice(['rock', 'paper', 'scissors'])

def determine_winner(user_choice, computer_choice):
    """Determine the winner based on user and computer choices."""
    if user_choice == computer_choice:
        return "It's a tie!"
    elif (user_choice == 'rock' and computer_choice == 'scissors') or \
         (user_choice == 'paper' and computer_choice == 'rock') or \
         (user_choice == 'scissors' and computer_choice == 'paper'):
        return "You win!"
    else:
        return "Computer wins!"

def play_game():
    """Main function to play the Rock, Paper, Scissors game."""
    user_score = 0
    computer_score = 0
    
    while True:
        print("\nLet's play Rock, Paper, Scissors!")
        
        user_choice = get_user_choice()
        computer_choice = get_computer_choice()
        
        print(f"\nYour choice: {user_choice.capitalize()}")
        print(f"Computer's choice: {computer_choice.capitalize()}")
        
        result = determine_winner(user_choice, computer_choice)
        print(result)
        
        # Update scores
        if result == "You win!":
            user_score += 1
        elif result == "Computer wins!":
            computer_score += 1
        
        # Ask if the user wants to play again
        play_again = input("\nDo you want to play again? (yes/no): ").strip().lower()
        if play_again != 'yes':
            break
    
    print(f"\nFinal Scores:")
    print(f"You: {user_score}   Computer: {computer_score}")

# Run the game
if __name__ == "__main__":
    play_game()
