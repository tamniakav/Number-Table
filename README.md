using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Number_Table
{
    class Program
    {
        static void Main(string[] args)
        {
            int n = int.Parse(Console.ReadLine());
            

            for (int row = 0; row < n; row++)
            {
                for (int col = 1; col <= n; col++)
                {
                    int num = row + col;
                    if (num <= n)
                    {
                    Console.Write($"{num} ");
                    }
                    else
                    {
                        int percentige = num % n;
                        num = n - percentige;
                        Console.Write($"{num} ");
                    }

                }
                Console.WriteLine();
            }
        }
    }
}
