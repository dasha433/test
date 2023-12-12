void Main()
    {
        Console.WriteLine("Введите элементы массива (разделяйте их пробелом):");

       
        string input = Console.ReadLine();

        // Разделяем введенную строку на элементы по пробелу
        string[] values = input.Split(' ');

        string result = "Массив из элементов, содержащих меньше 3 символов: ";

        for (int i = 0; i < values.Length; i++)
        {
           if(values[i].Length<=3)
           {
            // Console.WriteLine(values[i]);
            result +=  values[i]+ " ";
           }
        }
        Console.WriteLine(result);
    }
Main();