import random
from extras import logo, data, vs

print(logo)

rand_1,rand_2 = random.choices(data,k=2)

def bigger(rand_1,rand_2):
    if rand_1['follower_count'] > rand_2['follower_count']:
        return True
    else:
        return False

run = True
score = 0

while run:
            print(f"{rand_1['name']} , a {rand_1['description']} , from {rand_1['country']}")
            print(vs)
            print(f"{rand_2['name']} , a {rand_2['description']} , from {rand_2['country']}")
            guess = input("Whom do you think have more followers: 'A' or 'B' ").lower()
            if guess == 'a' and bigger(rand_1,rand_2) == True:
                    rand_2 = random.choice(data)
                    score += 1
                    print(f'Your right! Your score is {score}')
            elif guess == 'b' and bigger(rand_1,rand_2) == False:
                    rand_1 = rand_2
                    rand_2 = random.choice(data)
                    score += 1
                    print(f'Your right! Your score is {score}')
            else:
                    print(f'Your Wrong! Your score is {score}')
                    run = False





