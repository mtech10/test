def display():
    game_list = ['R for rock','P for paper','S for scissors']
    print('This is a rock,paper,scissors game \nRock beats scissors\nPaper beats rock\nScissors beats paper')
    print(game_list)
    print("Let's play")

def user_input():
    choice = 'wrong'
    while choice not in ['R','P','S']:
        choice = input('R,P or S?: ')
        if choice not in ['R','P','S']:
            print('Invalid input')
    return(choice)

from random import choice
from random import shuffle
def cpu_choice():
    game_list = ['R','P','S']
    shuffle(game_list)
    cpu_move = choice(game_list)
    return cpu_move

def check(player_move,cpu_move):
    while player_move == cpu_move:
        print("we have a tie \nLet's play again!")
        break
    if player_move =='R':
        if cpu_move == 'P':
            print(f'cpus move is {cpu_move}')
            print('Game over!')
        elif cpu_move == 'S':
            print(f'cpus move is {cpu_move}')
            print('You win!')
    elif player_move == 'P':
        if cpu_move == 'R':
            print(f'cpus move is {cpu_move}')
            print('You win!')
        elif cpu_move == 'S':
            print(f'cpus move is {cpu_move}')
            print('Game over!')
    elif player_move =='S':
        if cpu_move == 'R':
            print(f'cpus move is {cpu_move}')
            print('Game over!')
        if cpu_move =='P':
            print(f'cpus move is {cpu_move}')
            print('You win!')
        
def gameon():
    response = input('Do you want to keep playing? (Y or N): ')
    while response not in ['Y','N']:
        print('Invalid Choice!')
        response = input('Do you want to keep playing? (Y or N): ')
        
    if response in ['Y','N']:
        if response =='Y':
            return True
        elif response == 'N':
            return False
        
#ensure game is on
game_on = True
#introduction/game rules
while game_on == True:
    display()
    #player's choice
    player_move = user_input()
    #cpu's choice
    cpu_move = cpu_choice()
    #check
    check(player_move,cpu_move)
    game_on = gameon()