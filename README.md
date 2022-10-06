using System;
namespace ConsoleApp20
{
    class Program
    {
        static void Main(string[] args)
        {
            float peso, altura, imc;
            Console.Write("Insira um valor para o peso: ");
            peso = Convert.ToSingle(Console.ReadLine());
            Console.Write("insira um valor para a altura (em metros ex.: 1,76) :  ");
            altura = Convert.ToSingle(Console.ReadLine());
            imc = peso / (altura * altura);
            if (imc < 18.5)
                Console.WriteLine("Magreza");
            else
                if (imc >= 18.5 && imc < 25)
                Console.WriteLine("Normoponderal");
            else
                if (imc >= 25 && imc < 30)
                Console.WriteLine("Pre-obesidade");
            else
                if (imc >= 30 && imc < 40)
                Console.WriteLine("Obesidade");
            else
                Console.WriteLine("Obesidade morbida");
        }
    }
}
