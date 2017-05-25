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

            if (fans <= 4)
            {
                decimal transport = budget * Convert.ToDecimal(0.75);
                decimal forATickets = budget - Convert.ToDecimal(transport);

                if (ticket == "normal")
                {
                    decimal sumForATicket = Convert.ToDecimal(fans * 249.99);

                    Console.WriteLine(forATickets > sumForATicket
                        ? $"Yes! You have {forATickets = forATickets - sumForATicket} leva left."
                        : "Not enough money! You need {0} leva.", Math.Abs(forATickets = forATickets - sumForATicket));
                }
                else if (ticket == "vip")
                {
                    decimal sumForATicket = Convert.ToDecimal(fans * 499.99);

                    Console.WriteLine(forATickets > sumForATicket
                        ? $"Yes! You have {forATickets = forATickets - sumForATicket} leva left."
                        : "Not enough money! You need {0} leva.", Math.Abs(forATickets = forATickets - sumForATicket));
                }

            }
            else if (fans > 4 && fans <= 9)
            {
                decimal transport = budget * Convert.ToDecimal(0.6);
                decimal forATickets = budget - Convert.ToDecimal(transport);

                if (ticket == "normal")
                {
                    decimal sumForATicket = Convert.ToDecimal(fans * 249.99);

                    Console.WriteLine(forATickets > sumForATicket
                        ? $"Yes! You have {forATickets = forATickets - sumForATicket} leva left."
                        : "Not enough money! You need {0} leva.", Math.Abs(forATickets = forATickets - sumForATicket));
                }
                else if (ticket == "vip")
                {
                    decimal sumForATicket = Convert.ToDecimal(fans * 499.99);

                    Console.WriteLine(forATickets > sumForATicket
                        ? $"Yes! You have {forATickets = forATickets - sumForATicket} leva left."
                        : "Not enough money! You need {0} leva.", Math.Abs(forATickets = forATickets - sumForATicket));
                }
            }
            else if (fans > 9 && fans <= 24)
            {
                decimal transport = budget * Convert.ToDecimal(0.5);
                decimal forATickets = budget - Convert.ToDecimal(transport);

                if (ticket == "normal")
                {
                    decimal sumForATicket = Convert.ToDecimal(fans * 249.99);

                    Console.WriteLine(forATickets > sumForATicket
                        ? $"Yes! You have {forATickets = forATickets - sumForATicket} leva left."
                        : "Not enough money! You need {0} leva.", Math.Abs(forATickets = forATickets - sumForATicket));
                }
                else if (ticket == "vip")
                {
                    decimal sumForATicket = Convert.ToDecimal(fans * 499.99);

                    Console.WriteLine(forATickets > sumForATicket
                        ? $"Yes! You have {forATickets = forATickets - sumForATicket} leva left."
                        : "Not enough money! You need {0} leva.", Math.Abs(forATickets = forATickets - sumForATicket));
                }
            }
            else if (fans > 24 && fans <= 49)
            {
                decimal transport = budget * Convert.ToDecimal(0.4);
                decimal forATickets = budget - Convert.ToDecimal(transport);

                if (ticket == "normal")
                {
                    decimal sumForATicket = Convert.ToDecimal(fans * 249.99);

                    Console.WriteLine(forATickets > sumForATicket
                        ? $"Yes! You have {forATickets = forATickets - sumForATicket} leva left."
                        : "Not enough money! You need {0} leva.", Math.Abs(forATickets = forATickets - sumForATicket));
                }
                else if (ticket == "vip")
                {
                    decimal sumForATicket = Convert.ToDecimal(fans * 499.99);

                    Console.WriteLine(forATickets > sumForATicket
                        ? $"Yes! You have {forATickets = forATickets - sumForATicket} leva left."
                        : "Not enough money! You need {0} leva.", Math.Abs(forATickets = forATickets - sumForATicket));
                }
            }
            else
            {
                decimal transport = budget * Convert.ToDecimal(0.25);
                decimal forATickets = budget - Convert.ToDecimal(transport);

                if (ticket == "normal")
                {
                    decimal sumForATicket = Convert.ToDecimal(fans * 249.99);

                    Console.WriteLine(forATickets > sumForATicket
                        ? $"Yes! You have {forATickets = forATickets - sumForATicket} leva left."
                        : "Not enough money! You need {0} leva.", Math.Abs(forATickets = forATickets - sumForATicket));
                }
                else if (ticket == "vip")
                {
                    decimal sumForATicket = Convert.ToDecimal(fans * 499.99);

                    Console.WriteLine(forATickets > sumForATicket
                        ? $"Yes! You have {forATickets = forATickets - sumForATicket} leva left."
                        : "Not enough money! You need {0} leva.", Math.Abs(forATickets = forATickets - sumForATicket));
                }
            }
        }
    }
}
