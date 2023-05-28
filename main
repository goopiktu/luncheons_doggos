#include<stdio.h>
#include <stdlib.h>
#include <time.h>
#include <ctype.h>
#define N 1

int roll_die(void);
void Hooman_Action (int die_roll, int* heart, int* stars, int* ignore);
void Doggo_Beg(int die_roll);
void Doggo_Action(int die_roll);
void Hooman_Treats(int die_roll, int* stars, int* Doggo_Biscuit, int* French_Fries, int* Cheese, int* Pickle);
void Doggo_Play(int die_roll,int* play_time, int* chase_tail, int* zoomies, int* roll_over, int* neighbor_dog, int* neighbor_cat, int* sun);
void check_gender(int gender);

int main()
{
    int choice = 1;
do{
    time_t t;
    srand( time( &t ) );
    int chase_tail = 0, zoomies = 0, roll_over = 0, neighbor_dog = 0, neighbor_cat = 0, sun = 0,
        grill = 0, garden_times = 0, meat = 0, play_time = 0, ignore = 0, stars = 0, heart = 0,
        Doggo_Biscuit = 0, French_Fries = 0, Cheese = 0, Pickle = 0, Burger = 0, Hotdog = 0;
    int ask = 0;
    int die_roll;
    int gender, garb;

    printf("=================================WELCOME===============================\n");
    printf("        In this game you play as the dog of the family and               ");
    printf("\n       *your Objective of the game is to get 3 pieces of meat.*        ");
    printf("\n             enter the enter key to roll the die                       ");
    printf("\n               Enter any number to continue                            ");
    printf("\n=======================================================================\n");
    scanf("%d", &garb);

    printf("Are you a Male[1] or Female[0] ? ");
    scanf("%d",&gender);
    printf("Hello ");
    check_gender(gender);
    printf("Please roll the die.\n");
    getchar();


    while (meat != 3)
    {
/* Roll for Doggo Aciton */

            getchar();
            die_roll = roll_die();
            printf("You rolled a %d\n", die_roll);
            Doggo_Action(die_roll);

/* For kid #1 */

            if (die_roll == 1)
            {
                while(ask < 3)
                {
                    if (ask < 3)
                    {
                        printf("How do you want to beg for treatos?\n");
                    }
                    printf("Please roll the die.\n");
                    getchar();
                    die_roll = roll_die();
                    printf("You rolled a %d\n", die_roll);
                    Doggo_Beg(die_roll);
                    printf("Let's see how hooman reacts.\n");
                    if (die_roll == 4)
                        {
                            printf("Jackpot! Kid #1 gives you a Burger\n");
                            meat++;
                            Burger++;
                            break;
                        }
                    die_roll = roll_die();
                    if (die_roll >= 1 && die_roll <= 3)
                    {
                        if (die_roll == 1 || die_roll == 2)
                        {
                            printf("Kid #1 Gives you a Burger\n");
                            stars += 5;
                            meat++;
                            Burger++;
                            ask++;
                            if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                        }
                        else
                        {
                            printf("Kid #1 gives u ");
                            Hooman_Treats(die_roll, &stars, &Doggo_Biscuit, &French_Fries, &Cheese, &Pickle);
                            ask++;
                            if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                        }

                    }
                    else if (die_roll >= 4 && die_roll <= 6)
                    {
                        Hooman_Action(die_roll, &heart, &stars, &ignore);
                        if (ignore == 3)
                        {
                            printf("Steal Burger from Kid #1\n");
                            meat++;
                            Burger++;
                            stars -= 2;
                        }
                        ask++;
                        if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                    }
                }
                ask = 1;
                ignore = 0;
            }


/* For kid #2 */

            else if (die_roll == 2)
            {
                while(ask < 3)
                {
                    if (ask < 3)
                    {
                        printf("How do you want to beg for treatos?\n");
                    }
                    printf("Please roll the die.\n");
                    getchar();
                    die_roll = roll_die();
                    printf("You rolled a %d\n", die_roll);
                    Doggo_Beg(die_roll);
                    printf("Let's see how hooman reacts.\n");
                    if (die_roll == 3)
                        {
                            printf("Jackpot! Kid #2 gives you a Hotdog\n");
                            meat++;
                            Hotdog++;
                            break;
                        }
                    die_roll = roll_die();
                    if (die_roll >= 1 && die_roll <= 3)
                    {
                        if (die_roll == 1 || die_roll == 2)
                        {
                            printf("Kid #2 Gives you a Hotdog\n");
                            stars += 5;
                            meat++;
                            Hotdog++;
                            ask++;
                            if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                        }
                        else
                        {
                            printf("Kid #2 gives u ");
                            Hooman_Treats(die_roll, &stars, &Doggo_Biscuit, &French_Fries, &Cheese, &Pickle);
                            ask++;
                            if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                        }

                    }
                    else if (die_roll >= 4 && die_roll <= 6)
                    {
                        Hooman_Action(die_roll, &heart, &stars, &ignore);
                        if (ignore == 3)
                        {
                            printf("Steal Hotdog from Kid #2\n");
                            meat++;
                            Hotdog++;
                            stars -= 2;
                        }
                        ask++;
                        if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                    }
                }
                ask = 1;
                ignore = 0;
            }
/* For kid #3 */

            else if (die_roll == 3)
            {
                while(ask < 3)
                {
                    if (ask < 3)
                    {
                        printf("How do you want to beg for treatos?\n");
                    }
                    printf("Please roll the die.\n");
                    getchar();
                    die_roll = roll_die();
                    printf("You rolled a %d\n", die_roll);
                    Doggo_Beg(die_roll);
                    if (die_roll == 5)
                        {
                            printf("Jackpot! Kid #3 gives you a Hotdog\n");
                            meat++;
                            Hotdog++;
                            break;
                        }
                    printf("Let's see how hooman reacts.\n");
                    die_roll = roll_die();
                    if (die_roll >= 1 && die_roll <= 3)
                    {
                        if (die_roll == 1 || die_roll == 2)
                        {
                            printf("Kid #3 Gives you a Hotdog\n");
                            stars += 5;
                            meat++;
                            Hotdog++;
                            ask++;
                            if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                        }
                        else
                        {
                            printf("Kid #3 gives u ");
                            Hooman_Treats(die_roll, &stars, &Doggo_Biscuit, &French_Fries, &Cheese, &Pickle);
                            ask++;
                            if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                        }

                    }
                    else if (die_roll >= 4 && die_roll <= 6)
                    {
                        Hooman_Action(die_roll, &heart, &stars, &ignore);
                        if (ignore == 3)
                        {
                            printf("Steal Hotdog from Kid #3\n");
                            meat++;
                            Hotdog++;
                            stars -= 2;
                        }
                        ask++;
                        if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                    }
                }
                ask = 1;
                ignore = 0;
            }

/* For table parent */
            else if (die_roll == 4)
            {
                while(ask < 3)
                {
                    if (ask < 3)
                    {
                        printf("How do you want to beg for treatos?\n");
                    }
                    printf("Please roll the die.\n");
                    getchar();
                    die_roll = roll_die();
                    printf("You rolled a %d\n", die_roll);
                    Doggo_Beg(die_roll);
                    if (die_roll == 6)
                        {
                            printf("Jackpot! Parent #1 gives you a Burger\n");
                            meat++;
                            Burger++;
                            break;
                        }
                    printf("Let's see how hooman reacts.\n");
                    die_roll = roll_die();
                    if (die_roll >= 1 && die_roll <= 3)
                    {
                        if (die_roll == 1 || die_roll == 2)
                        {
                            printf("Parent #1 Gives you a Burger\n");
                            stars += 5;
                            meat++;
                            Burger++;
                            ask++;
                            if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                        }
                        else
                        {
                            printf("Parent #1 gives u ");
                            Hooman_Treats(die_roll, &stars, &Doggo_Biscuit, &French_Fries, &Cheese, &Pickle);
                            ask++;
                            if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                        }

                    }
                    else if (die_roll >= 4 && die_roll <= 6)
                    {
                        Hooman_Action(die_roll, &heart, &stars, &ignore);
                        if (ignore == 3)
                        {
                            printf("Steal Burger from Parent #1\n");
                            meat++;
                            Burger++;
                            stars -= 2;
                        }
                        ask++;
                        if (ask > 0 && ask < 3)
                            {
                                printf("You can beg for more treatos\n");
                            }
                    }
                }
                ask = 1;
                ignore = 0;
            }


/* parent grilling */
            else if (die_roll == 5)
            {
                if (grill < 2)
                {
                    printf("Parent is busy grilling (try again later)\n");
                    grill++;
                }
                if (grill == 3)
                {
                    printf("Parent is done grilling!\n");
                    printf("And now walking towards the picnic table to sit\n");
                    grill++;
                    while(ask < 3)
                    {
                        if (ask < 3)
                        {
                            printf("How do you want to beg for treatos?\n");
                        }
                        printf("Please roll the die.\n");
                        getchar();
                        die_roll = roll_die();
                        printf("You rolled a %d\n", die_roll);
                        Doggo_Beg(die_roll);
                        if (die_roll == 6)
                        {
                            printf("Jackpot! Parent #2 gives you a Burger\n");
                            meat++;
                            Burger++;
                            break;
                        }
                        printf("Let's see how hooman reacts.\n");
                        die_roll = roll_die();
                        if (die_roll >= 1 && die_roll <= 3)
                        {
                            if (die_roll == 1 || die_roll == 2)
                            {
                                printf("Parent #2 Gives you a Burger\n");
                                stars += 5;
                                meat++;
                                Burger++;
                                ask++;
                                if (ask > 0 && ask < 3)
                                {
                                    printf("You can beg for more treatos\n");
                                }
                            }
                            else
                            {
                                printf("kid #1 gives u ");
                                Hooman_Treats(die_roll, &stars, &Doggo_Biscuit, &French_Fries, &Cheese, &Pickle);
                                ask++;
                                if (ask > 0 && ask < 3)
                                {
                                    printf("You can beg for more treatos\n");
                                }
                            }

                        }
                        else if (die_roll >= 4 && die_roll <= 6)
                        {
                            Hooman_Action(die_roll, &heart, &stars, &ignore);
                            if (ignore == 3)
                            {
                                printf("Steal Burger from Parent #2\n");
                                meat++;
                                Burger++;
                                stars -= 2;
                            }
                            ask++;
                            if (ask > 0 && ask < 3)
                                {
                                    printf("You can beg for more treatos\n");
                                }
                        }
                    }
                    ask = 1;
                    ignore = 0;
                }
            }
            /* Garden */
            else if (die_roll == 6)
            {
                printf("Please roll the die.\n");
                getchar();
                die_roll = roll_die();
                printf("You rolled a %d\n", die_roll);
                if (die_roll == 6)
                {
                    printf("Have fun playing in the garden!");
                    printf(" Bye, ");
                    check_gender(gender);
                    printf("\n\n======================================================================\n");
                    printf("You got *%d* Stars!, including *%d* hearts\n", stars, heart);
                    printf("You got *%d* Burger, *%d* Hotdog, *%d* Doggo Biscuits, *%d* FrenchFries, *%d* Cheese, *%d* Pickle \n", Burger, Hotdog, Doggo_Biscuit, French_Fries, Cheese, Pickle);
                    printf("Hope you enjoyed the *%d* minutes spent playing in the garden.\n", play_time);
                    printf("You spent *%d* minutes chasing your tail\n", chase_tail);
                    printf("You spent *%d* minutes doing zoomies\n", zoomies);
                    printf("You spent *%d* minutes rolling over and showing off some tricks\n", roll_over);
                    printf("You spent *%d* minutes checking out the neighbor's dog\n", neighbor_dog);
                    printf("You spent *%d* minutes checing out the neighbor's cat\n", neighbor_cat);
                    printf("You spent *%d* minutes sunbathing!\n", sun);
                    printf("Sounds like a lot of fun!!");
                    printf("\n======================================================================\n");
                    return 0;
                }
                Doggo_Play(die_roll, &play_time, &chase_tail, &zoomies, &roll_over, &neighbor_dog, &neighbor_cat, &sun);
            }
            // used this to count meat and garden printf("%d, %d",garden_times, meat);

    }

    printf("\n\n======================================================================\n");
    printf("You got *%d* Stars!, including *%d* hearts\n", stars, heart);
    printf("You got *%d* Burger, *%d* Hotdog, *%d* Doggo Biscuits, *%d* FrenchFries, *%d* Cheese, *%d* Pickle \n", Burger, Hotdog, Doggo_Biscuit, French_Fries, Cheese, Pickle);
    printf("Hope you enjoyed the *%d* minutes spent playing in the garden.\n", play_time);
    printf("You spent *%d* minutes chasing your tail\n", chase_tail);
    printf("You spent *%d* minutes doing zoomies\n", zoomies);
    printf("You spent *%d* minutes rolling over and showing off some tricks\n", roll_over);
    printf("You spent *%d* minutes checking out the neighbor's dog\n", neighbor_dog);
    printf("You spent *%d* minutes checing out the neighbor's cat\n", neighbor_cat);
    printf("You spent *%d* minutes sunbathing!\n", sun);
    printf("Sounds like a lot of fun!!");
    printf("\n======================================================================\n");

    printf("would you like to play again? yes[1] or no[0]\n");
    scanf("%d", &choice);
    }while(choice == 1);

    return 0;
}
/* Die Roll */
int roll_die( void )
{
    return ( int )rand()%6+1;
}
/*Check if user is girl or boy*/
void check_gender(int gender)
{
    if (gender == 1)
    {
        printf("Bailey!\n");
    }
    else
    {
        printf("Kahlua!\n");
    }
}
/*
=====================|
Doggo Actions        |
=====================|
1 = Kid #1           |
2 = Kid #2           |
3 = Kid #3           |
4 = Parent table     |
5 = Parent grilling  |
6 = Garden           |
=====================|
*/
void Doggo_Action(int die_roll)
{
    if (die_roll == 1)
    {
        printf("You ran to kid #1\n");
    }
    else if (die_roll == 2)
    {
        printf("You ran to kid #2\n");
    }
    else if (die_roll == 3)
    {
        printf("You ran to kid #3\n");
    }
    else if (die_roll == 4)
    {
        printf("Run to parent near the table\n");
    }
    else if (die_roll == 5)
    {
        printf("Run to parent grilling\n");
    }
    else if (die_roll == 6)
    {
        printf("You decided to play in the garden?\n");
    }

}
/*
=========================================|
                Doggo Beg                |
=========================================|
1 = Nudge hooman with snout              |
2 = Poke hooman with paw                 |
3 = Place paw on hooman's lap            |
4 = Place head on hooman's lap           |
5 = Climb hooman's lap                   |
6 = Sit and show hooma you're a good dog |
=========================================|
*/
void Doggo_Beg(int die_roll)
{
    switch (die_roll)
    {
        case 1:
            printf("Nudge Hooman with snout\n");
            break;
        case 2:
            printf("Poke hooman with paw\n");
            break;
        case 3:
            printf("Place paw on hooman's lap\n");
            break;
        case 4:
            printf("Place head on hooman's lap\n");
            break;
        case 5:
            printf("Climb hooman's lap\n");
            break;
        case 6:
            printf("Sit and show hooman you're a good dog!\n");
            break;
        default:
            printf("something went wrong?\n");
    }
}
/*
=====================|
Hoomans Actions      |
=====================|
1 = Give Treat       |
2 = Give Treat       |
3 = Give Treat       |
4 = pat on the head  |
5 = Play for 2 min   |
6 = Ignored :(       |
=====================|
*/
void Hooman_Action (int die_roll, int* heart, int* stars, int* ignore)
{
    if (die_roll == 4)
    {
        printf("Hooman pats you on the head\n");
        *heart += 1;
        *stars += 3;
    }
    else if (die_roll == 5)
    {
        printf("Hooman plays with you for 2 min\n");
        *heart += 1;
        *stars += 3;
    }
    else if (die_roll == 6)
    {
        printf("Hooman Ignores you\n");
        *ignore += 1;
    }
}
/*
=====================|
Hoomans Treats       |
=====================|
1 = Hotdog or Burger |
2 = Hotdog or Burger |
3 = Doggeo Biscuit   |
4 = French Fries     |
5 = Cheese           |
6 = Ignored :(       |
=====================|
*/
void Hooman_Treats (int die_roll, int* stars, int* Doggo_Biscuit, int* French_Fries, int* Cheese, int* Pickle)
{
    if (die_roll == 3)
    {
        printf("Doggo Biscuit\n");
        *stars += 3;
        *Doggo_Biscuit += 1;
    }
    else if (die_roll == 4)
    {
        printf("Fench Fries\n");
        *stars += 2;
        *French_Fries += 1;
    }
    else if (die_roll == 5)
    {
        printf("Cheese\n");
        *stars += 2;
        *Cheese += 1;
    }
    else if (die_roll == 6)
    {
        printf("Pickle\n");
        *stars += 1;
        *Pickle += 1;
    }
}
/*
==================================|
Doggo Play                        |
==================================|
1 = Chase your tail               |
2 = Do zoomies!                   |
3 = Roll over and show tricks     |
4 = Check out the neighbor's dog  |
5 = CCheck out the neighbor's cat |
6 = Bathe in the sun.             |
==================================|
*/
void Doggo_Play(int die_roll, int* play_time, int* chase_tail, int* zoomies, int* roll_over,int* neighbor_dog, int* neighbor_cat, int* sun)
{
    switch (die_roll)
    {
        case 1:
            printf("Chase your tail for 3 min.\n");
            *chase_tail += 3;
            *play_time += 3;
            break;
        case 2:
            printf("You decided to do zoomies!\nZoom! Zoom! Zoom!\n");
            *zoomies += 6;
            *play_time += 6;
            break;
        case 3:
            printf("Roll over and show tricks\n");
            *roll_over += 9;
            *play_time += 9;
            break;
        case 4:
            printf("Check out the neighbor's dog\n");
            *neighbor_dog += 12;
            *play_time += 12;
            break;
        case 5:
            printf("Check out the neighbor's cat\n");
            *neighbor_cat += 15;
            *play_time += 15;
            break;
        case 6:
            printf("Bathe in the sun\n");
            *sun += 18;
            *play_time += 18;
            break;
        default:
            printf("something went wrong?\n");
    }
}
