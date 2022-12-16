# BEECROWD-2344
EXERCÍCIO 2344 - Notas da Prova ( RESOLVIDO EM JAVA)

#Entrada
A entrada contém um único conjunto de testes, que deve ser lido do dispositivo de entrada padrão (normalmente o teclado). A entrada contém uma única linha com um número inteiro N (0 ≤ N ≤ 100), representando uma nota de prova no sistema numérico.#

#Saída
Seu programa deve imprimir, na saída padrão, uma letra (A, B, C, D, ou E em maiúsculas) representando o conceito correspondente à nota dada na entrada.#


import java.util.Locale;
import java.util.Scanner;
public class Main {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		sc.useLocale(Locale.ENGLISH);
		Locale.setDefault(new Locale("en", "US"));
		
		int notaNum = sc.nextInt();
		if (notaNum == 0) System.out.println('E');
		else if (notaNum>=1 && notaNum<=35) System.out.println('D');
		else if (notaNum>=36 && notaNum<=60) System.out.println('C');
		else if (notaNum>=61 && notaNum<=85) System.out.println('B');
		else if (notaNum>=86 && notaNum<=100) System.out.println('A');
				
		sc.close();
	}
}
