﻿# Menu-em-C-
 using System;

class Program
{
    static void Main()
    {
        bool exit = false;

        while (!exit)
        {
            Console.Clear();
            Console.WriteLine("Menu Inicial");
            Console.WriteLine("1 - Cadastros");
            Console.WriteLine("2 - Relatórios");
            Console.WriteLine("0 - Sair");

            Console.Write("Escolha o que deseja acessar: ");
            string mainOption = Console.ReadLine();

            switch (mainOption)
            {
                case "1":
                    Processamento_Menu();
                    break;
                case "2":
                    ProcessRelatorioMenu();
                    break;
                case "0":
                    exit = true;
                    break;
                default:
                    Console.WriteLine("Está opção é invalidade!");
                    break;
            }

            Console.WriteLine("\nPressione qualquer tecla para continuar...");
            Console.ReadKey();
        }

        Console.WriteLine("Fechando sistema.");
    }

    static void Processamento_Menu()
    {
        bool exitCadastro = false;

        while (!exitCadastro)
        {
            Console.Clear();

            Console.WriteLine("Menu Inicial");
            Console.WriteLine("1.1 - Médicos");
            Console.WriteLine("1.2 - Animais");
            Console.WriteLine("1.3 - Atendimentos");
            Console.WriteLine("1.4 - Sair");

            Console.Write("Escolha o que deseja acessar: ");
            string cadastroOption = Console.ReadLine();

            switch (cadastroOption)
            {
                case "1.1":
                    Console.WriteLine("Você selecionou Médicos");
                    break;
                case "1.2":
                    Console.WriteLine("Você selecionou Animais");
                    break;
                case "1.3":
                    Console.WriteLine("Você selecionou Atendimentos");
                    break;
                case "1.4":
                    exitCadastro = true;
                    break;
                default:
                    Console.WriteLine("Está opção é invalidade!");
                    break;
            }

            Console.WriteLine("\nPressione qualquer tecla para continuar...");
            Console.ReadKey();
        }
    }

    static void Processamento_Menu()
    {
        bool exitRelatorio = false;

        while (!exitRelatorio)
        {
            Console.Clear();

            Console.WriteLine("Menu Inicial");
            Console.WriteLine("2.1 - Animais");
            Console.WriteLine("2.2 - Atendimentos");
            Console.WriteLine("2.3 - Sair");

            Console.Write("Escolha o que deseja acessar: ");
            string relatorioOption = Console.ReadLine();

            switch (relatorioOption)
            {
                case "2.1":
                    Console.WriteLine("Você selecionou Animais");
                    break;
                case "2.2":
                    Console.WriteLine("Você selecionou Atendimentos");
                    break;
                case "2.3":
                    exitRelatorio = true;
                    break;
                default:
                    Console.WriteLine("Está opção é invalidade!");
                    break;
            }

            Console.WriteLine("\nPressione a tecla ENTER para continuar...");
            Console.ReadKey();
        }
    }
}
