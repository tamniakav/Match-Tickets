using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Match_Tickets
{
    class Program
    {
        static void Main(string[] args)
        {
            decimal budget = decimal.Parse(Console.ReadLine());
            string ticket = Console.ReadLine().ToLower();
            int fans = int.Parse(Console.ReadLine());
            decimal moneyForTrprt = 0;
            if (fans < 5)
            {
                moneyForTrprt = budget * 0.75m;
            }
            else if (fans < 10)
            {
                moneyForTrprt = budget * 0.60m;
            }
            else if (fans < 25)
            {
                moneyForTrprt = budget * 0.50m;
            }
            else if (fans < 50)
            {
                moneyForTrprt = budget * 0.40m;
            }
            else
            {
                moneyForTrprt = budget * 0.25m;
            }

            decimal moneyForTicket = budget - moneyForTrprt;
            decimal neededMoney = 0;

            if (ticket == "normal")
            {
                neededMoney = fans * 249.99m;
            }
            else if (ticket == "vip")
            {
                neededMoney = fans * 499.99m;
            }

            if (neededMoney > moneyForTicket)
            {
                decimal lessMoney = neededMoney - moneyForTicket;
                Console.WriteLine($"Not enough money! You need {lessMoney:f2} leva.");
            }
            else
            {
                decimal moneyOver = moneyForTicket - neededMoney;
                Console.WriteLine($"Yes! You have {moneyOver:f2} leva left.");
            }
        }
    }
}
