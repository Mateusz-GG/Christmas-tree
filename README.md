# Christmas-tree
{
    class Program
    {
        static void Main(string[] args)
        {
            int hight, trunk;

            Console.WriteLine("Podaj wysokość : ");
            hight = Convert.ToInt32(Console.ReadLine());
            trunk = hight / 3;

            for (int i = 0; i < hight; i++)
            {
                for (int j = 0; j < hight - i - 1; j++)
                {
                    Console.Write(" ");
                }

                for (int k = 0; k < i * 2 + 1; k++)
                {
                    Console.Write("*");
                }

                Console.WriteLine();
            }
            for (int n = 0; n < trunk; n++)
            {
                for (int m = 0; m < hight - 2; m++)
                {
                    Console.Write(" ");
                }
                Console.WriteLine("|");
            }

            if (hight == 0) 
            {
                Console.WriteLine("Can't grow.");
            }
        }
    }
}
