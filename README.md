# Create-Task-Draft
#Surviving High school game

print("Welcome to Future High!")
print("You have a Final Exam in a week that you have to study for.")
print("You also have a championship game this weekend for your sports team!")
print("Choose the best option for you to do that help you to fully prepare for the exam, and your championship game.")
print("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~")



def main():
    day = 0
    daysLeft = 7
    examReady = 0
    gameReady = 0
    rest = 5
    while True:
        day = day+1       
        print("Day", day)
        print("What do you want to do today?")
    
        print("A. Study for 1 hour")
        print("B. Go to Practice")
        print("C. Rest for the day")
        print("Q. Quit simulation")
        userInput = input()

        if userInput == "A" or userInput == "a":
            daysLeft = daysLeft-1
            examReady = examReady+1
            print("You have", daysLeft, "days left until the exam.")
            print("You have", daysLeft, "days left until the game.")
    
        elif userInput == "B" or userInput == "b":
            daysLeft = daysLeft-1
            gameReady = gameReady+1
            print("You have", daysLeft, "days left until the exam.")
            print("You have", gameReady, "days left until the game.")

        elif userInput == "C" or userInput == "c":
            daysLeft = daysLeft-1
            print("You have", daysLeft, "days left until the exam.")
            print("You have", gameReady, "days left until the game.")

        elif userInput == "Q" or userInput == "q":
            print("Thank you for playing!")
            break
main() 
