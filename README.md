package ServiçoPet;

import java.util.Scanner;

public class Caramelo {

    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
			// Declaração de variáveis
			String Nome;
			double CPF;
			String NomePet;
			String Animal;
			int Opcao;

			// Loop infinito para reiniciar o atendimento após cada operação
			while (true) {
			    System.out.print("\nDigite seu Nome: ");
			    Nome = scanner.nextLine();

			    System.out.print("Digite seu CPF: ");
			    CPF = scanner.nextDouble();
			    scanner.nextLine(); // limpa o buffer do teclado

			    System.out.print("\nDigite o nome do seu Pet: ");
			    NomePet = scanner.nextLine();

			    System.out.print("\nDigite o tipo do seu Animal: ");
			    Animal = scanner.nextLine();

			    System.out.println("\n---------- REGISTRADO ----------");
			    System.out.println("Selecione uma Opção:");
			    System.out.println("(1) Falar com Atendente(a)?");
			    System.out.println("(2) Falar com Veterinário(a)?");
			    System.out.println("(3) Falar com Treinador(a)?");
			    System.out.println("(4) Consultar o Plano do Pet?");
			    System.out.println("(5) Comprar a Ração do Pet?");
			    System.out.print("Opção: ");

			    Opcao = scanner.nextInt();
			    scanner.nextLine(); // limpa o buffer

			    switch (Opcao) {
			        case 1:
			            System.out.println("Sou o Caramelo virtual");
			            System.out.println("\\nOk, Falar com Atendente(a).");
			            System.out.println("Aguarde um minuto, você será direcionado ao setor de Atendimento.\n");
			            System.out.println("Ajudo em Algum Mais?");
			            break;

			        case 2:
			            System.out.println("Sou o Caramelo virtual");
			            System.out.println("\nOk, Falar com o Veterinário(a).");
			            System.out.println("Aguarde um minuto, você será direcionado ao setor Veterinário.\n");
			            System.out.println("Ajudo em Algum Mais?");
			            break;

			        case 3:
			        	 System.out.println("Sou o Caramelo virtual");
			             System.out.println("\nOk, Falar com o Treinadores(a).");
			             System.out.println("Aguarde um minuto, você será direcionado ao setor do Treinadores(a).\n");
			             System.out.println("Ajudo em Algum Mais?");
			            break;

			        case 4:
			        	System.out.println("Sou o Caramelo virtual");
			            System.out.println("\nOk, Consultar o plano do Pet.");
			            System.out.println("Aguarde um minuto, você será direcionado para a Consulta do plano do Pet.\n");
			            System.out.println("Ajudo em Algum Mais?");
			            break;
			        case 5:
			        	System.out.println("Sou o Caramelo virtual");
			            System.out.println("\nOk, Compra a Ração do Pet.");
			            System.out.println("Aguarde um minuto, você será direcionado para Compra a Ração do Pet.\n");
			            System.out.println("Ajudo em Algum Mais?");
			            break;    

			            
			        default:
			            System.out.println("\nOpção Inválida.");
			            System.out.println("Atendimento Finalizado. Iniciando novo atendimento...\n");
			            break;
			    }

			    System.out.println("\n--------------------------------------\n");
			}
		}
    }
}


