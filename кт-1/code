using System;

class IndexerExample
{
    private int[] intArray = new int[100];
    private double[] doubleArray = new double[100];

    public int this[int index]
    {
        get { return intArray[index]; }
        set { intArray[index] = value; }
    }

    public string this[string index]
    {
        get { return $"Строковый индекс: {index}"; }
    }

    public double this[double index]
    {
        get
        {
            int i = (int)index;
            return doubleArray[i];
        }
        set
        {
            int i = (int)index;
            doubleArray[i] = value;
        }
    }
}

class Program
{
    static void Main()
    {
        IndexerExample obj = new IndexerExample();

        obj[5] = 10;
        Console.WriteLine("Значение по индексу [5] = " + obj[5]);

        Console.WriteLine(obj["индексовый"]);

        Console.WriteLine();

        obj[4.51] = 100.5;
        obj[9.49] = 200.5;
        obj[99.9] = 300.5;

        Console.WriteLine("Значение по индексу [4.51] = " + obj[4.51]);
        Console.WriteLine("Значение по индексу [9.49] = " + obj[9.49]);
        Console.WriteLine("Значение по индексу [99.9] = " + obj[99.9]);
    }
}
