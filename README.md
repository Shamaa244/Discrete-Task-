# Discrete-Task-

namespace Prime_Numbers_From_n1_to_n2
{
    class Program
    {
        static void Main(string[] args)
        {
            int n1, n2;

            Console.Write("Input the starting number of the range: ");
            n1 = Convert.ToInt32(Console.ReadLine());

            Console.Write("Input the ending number of the range: ");
            n2 = Convert.ToInt32(Console.ReadLine());

            Console.Write("The prime numbers between {0} and {1} are: ", n1, n2);

            for (int i = n1; i <= n2; i++)  //for loop to check prime numbers from n1 to n2 
            { 
                int ctr = 0;  //counter to count the divisors of a number  

                for (int j = 1; j <= i; j++) //for loop to divide the given number from 1 to itself 
                {  
                    if (i % j == 0)   //condition for non-prime number  
                    {  
                        ctr++;   //incrementing the counter if a divisor is found  
                    }  

                }  

                if (ctr == 2)  //condition for prime number  
                {  

                    Console.Write("{0} ", i);  //printing prime numbers from n1 to n2 separated by space   

                }   

            }   

        }   

    }               //
