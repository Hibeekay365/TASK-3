using System;
using System.Collections.Generic;
using System.Linq;

namespace C_TASK3
{
    class Program
    {
        static void Main(string[] args)
        {
var numberRandom = new Random();
            Console.WriteLine(" Welcome to my number guessing game");
            Console.WriteLine("\nLevels of difficulty available: E- Easy, M- Medium, H- Hard");
            Console.Write("Which level of difficulty do you prefer: ");
            string userGuess = Console.ReadLine();

             if (userGuess == "E")
            {
                Console.WriteLine("\nYou have selected easy: You have to guess a number between 1 to 10");
                 int i = 0;
                int a;
                while (i <= 5)
                {
                numberRandom.Next(1, 11);
                    Console.WriteLine("\nYou have {0} chances left", a = 6- i);
                     Console.Write("Guess a number: ");
                    int guessNumber =Convert.ToInt32(Console.ReadLine());
                    if (guessNumber==numberRandom.Next(1, 11))
                    {
                        Console.WriteLine("You're correct!");
                    }
                    else
                    {
                        Console.WriteLine("You're Wrong!");
                    }
                    i++;
                    }
                Console.WriteLine("\nGame Over!");
            }
            if (userGuess == "M")
            {
                Console.WriteLine("\nYou have selected medium: You have to guess a number between 1 to 20");
                int i = 0;
                int a;
                while (i <= 3)
                {
                    numberRandom.Next(1, 11);
                    Console.WriteLine("\nYou have {0} chances left", a = 4 - i);
                    Console.Write("Guess a number: ");
                    int guessNumber = Convert.ToInt32(Console.ReadLine());
                    if (guessNumber == numberRandom.Next(1, 21))
                    {
                        Console.WriteLine("You're Right!");
                    }
                    else
                    {
                        Console.WriteLine("You're Wrong!");
                    }
                    i++;
                }
                Console.WriteLine("\nGame Over!");
            }
            if (userGuess == "H")
            {
                Console.WriteLine("\nYou have selected easy: You have to guess a number between 1 to 50");
                int i = 0;
                int a;
                while (i <= 2)
                {
                    numberRandom.Next(1, 11);
                    Console.WriteLine("\nYou have {0} chances left", a = 3 - i);
                    Console.Write("Guess a number: ");
                    int guessNumber = Convert.ToInt32(Console.ReadLine());
                    if (guessNumber == numberRandom.Next(1, 51))
                    {
                        Console.WriteLine("You're Right!");
                    }
                    else
                    {
                        Console.WriteLine("You're Wrong!");
                    }
                    i++;
                }
                Console.WriteLine("\nGame Over!");
            }

        }


    }
}



PS C:\Users\user\C#TASK3> dotnet run
 Welcome to my number guessing game

Levels of difficulty available: E- Easy, M- Medium, H- Hard
Which level of difficulty do you prefer: M

You have selected medium: You have to guess a number between 1 to 20

You have 4 chances left
Guess a number: 18
You're Wrong!

You have 3 chances left
Guess a number: 5
You're Wrong!

You have 2 chances left
Guess a number: 11
You're Wrong!

You have 1 chances left
Guess a number: 16
You're Wrong!

Game Over!
PS C:\Users\user\C#TASK3> dotnet run
 Welcome to my number guessing game

Levels of difficulty available: E- Easy, M- Medium, H- Hard
Which level of difficulty do you prefer: E

You have selected easy: You have to guess a number between 1 to 10

You have 6 chances left
Guess a number: 5
You're Wrong!

You have 5 chances left
Guess a number: 2
You're Wrong!

You have 4 chances left
Guess a number: 6
You're Wrong!

You have 3 chances left
Guess a number: 8
You're Wrong!

You have 2 chances left
Guess a number: 1
You're Wrong!

You have 1 chances left
Guess a number: 7
You're correct!

Game Over!
PS C:\Users\user\C#TASK3> dotnet run
 Welcome to my number guessing game

Levels of difficulty available: E- Easy, M- Medium, H- Hard
Which level of difficulty do you prefer: H

You have selected easy: You have to guess a number between 1 to 50

You have 3 chances left
Guess a number: 50
You're Wrong!

You have 2 chances left
Guess a number: 40
You're Wrong!

You have 1 chances left
Guess a number: 10
You're Wrong!

Game Over!
PS C:\Users\user\C#TASK3>
