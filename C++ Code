// Pranav Vaddadi, Marko Rudek, Eric Zheng
// Team #24
//No Ai is used in this assignment.
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int choice(void);
int LUKEq(void);
int Utahq(void);

int main()
{
	int again=1, totalpoints=0, dice, point1, point2;
	
	do
	{
		printf("Welcome to AI Prosthetic Exploration!\n");
		
		printf("On the board, there are 2 stacks of cards: LUKE ARM and Utah Bionic Leg.\n");
		
		printf("In these stacks are filled with questions about these two primary limbs.\n");
		
		printf("The user will have to input a number between 1-6.\n");
		
		printf("If the user inputs a odd number, they will have to answer a LUKE Arm question.\n");
		
		printf("If The user inputs a even number, they will have to answer a DEKA Arm question.\n");
		
		printf("If the user answers their questions correctly, they get a point for each question.\n");
		
		printf("The game ends once the user gets 3 points\n");
		
		dice=choice();
		
		switch (dice)
		{
			case 1:
				//function 2
				point1=LUKEq();
				break;
			case 2:
				//function 3
				point2=Utahq();
				break;
		}
		
		if (dice == 1)
		{
			totalpoints=totalpoints+point1;
		}
		else if (dice == 2)
		{
			totalpoints=totalpoints+point2;
		}
		
	
		printf("\nUser's total points: %d\n", totalpoints);
	
		if (totalpoints == 3)
		{
			printf("You have won!\n");
		}
		else if (totalpoints <3)
		{
			printf("You have lost, continue play\n");
		}
		
		printf("Would you like to play again: 1 - yes, 2 - no\n");
		scanf("%d", &again);
	
	}while(again == 1);
	
	return 0;
}
//Functions

//function 1
int choice(void)
{
	int dice;
	
	do
	{
		printf("Enter a number 1-2: \n");
		scanf("%d", &dice);
	}while(dice!=1 && dice!=2);
	
	return (dice);
}
//Function 2-LUKE ARM questions

int LUKEq(void)
{
	int point1=0, ans1, ans2, ans3;
	
	//question 1
	do{
	printf("\n\nQuestion 1: The LUKE arm was named after the Star Wars character Luke Skywalker: 1=True, 2=False ");
	scanf("%d",&ans1);} while (ans1 !=1&& ans1 !=2);
	
	if(ans1==1)
	{
		point1=point1+1;
		printf("\nCongrats you earned a point!");
	};
	
	//question 2
	do{printf("\n\nQuestion 2: The LUKE arm was first made for civilian use(1=True, 2=False) :");
	scanf("%d",&ans2);} while (ans2 !=1&& ans2 !=2);
	
	if(ans2==2)
	{
		point1=point1+1;
		printf("\nCongrats you earned a point!");
	};
	
	//question 3
	do{printf("\n\nQuestion 3: The LUKE arm can be custom built for each user(1=True, 2=False) :");
	scanf("%d",&ans3);} while (ans3 !=1&& ans3 !=2);
	
	if(ans3==1)
	{
		point1=point1+1;
		printf("\nCongrats you earned a point!");
	};
	
	return(point1);

}


//Function 3-Utah bionic questions

int Utahq(void)
{
	int ans1, ans2, ans3,point2=0;
	
	//question 1
	do{printf("\n\nQuestion 1: The Utah Bionic Leg assists in balance and muscle output(1=True, 2=False) :");
	scanf("%d",&ans1);} while (ans1 !=1&& ans1 !=2);
	
	if(ans1==1)
	{
		point2=point2+1;
		printf("\nCongrats you earned a point!");
	};
	
	//question 2
	do{printf("\n\nQuestion 2: The utah Bionic Leg is currently fully on the market and able to be purchased(1=True, 2=False) :");
	scanf("%d",&ans2);} while (ans2 !=1&& ans2 !=2);
	
	if(ans2 ==2)
	{
		point2=point2+1;
		printf("\nCongrats you earned a point!");
	};
	
	//question 3
	do{printf("\n\nQuestion 3: 15400 steps can be taken on a full charge of battery(1=True, 2=False) :");
	scanf("%d",&ans3);} while (ans3 !=1&& ans3 !=2);
	
	if(ans3==1)
	{
		point2=point2+1;
		printf("\nCongrats you earned a point!");
	}
	
	return(point2);
}
