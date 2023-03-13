import java.util.Scanner;

public class Logicabasica {
public static void main(String[] args) {
	Scanner input = new Scanner(System.in);
	
	System.out.println("Escreva um numero");
	float num1 = input.nextInt();
	
	char operacao;
	do {
		System.out.println("Digite uma operação (+ - x /):");
		operacao = input.next().charAt(0);
	} while (operacao != '+' && operacao != '-' && operacao != 'x' && operacao != '/');
	
	System.out.println("Digite outro numero");
	float num2 = input.nextInt();
	
	float resultado = 0;
	switch (operacao) {
	
	case '+':
		resultado = num1 + num2;
		break;
	case '-':
		resultado = num1 - num2;
		break;
	case 'x':
		resultado = num1 * num2;
		break;
	case '/':
		resultado = num1 / num2;
	}
	System.out.println("O resultado é: " + resultado);
	//∴
}
}
