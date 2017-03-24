# Terminado-Por
import java.util.Scanner;

public class TerminadoPor {

	public static void main(String[] args) {
		Scanner in = new Scanner(System.in);

		System.out.println("Digite numeros nao negativos (zero termina): ");
		int cont = 0;
		//double soma = 0; // para funcionar com numeros reais
		int soma = 0;
		
		int num = in.nextInt();

		while(num>0){
			cont++; // Contador				
			
			soma = soma + num; // Acumulador
			num = in.nextInt();
		}

		System.out.println("Foram digitados "+cont+" numeros pares...");
		System.out.println("O total da soma dos numeros eh: "+soma);
		
		System.out.println("A media eh: "+(soma/cont));
		
		in.close();
	}

}
