# TP-calculatrice-en-java-
package Programme;

import java.util.Scanner;
public class Etapevi {
	public static void main(String[] args) {
		do {
		Scanner scanner = new Scanner(System.in);
System.out.println("Quelle est votre nom ");
	String nom;
	nom = scanner.nextLine();
	System.out.println("Hello "+nom+" Quelle operation voulez vous effectuer");
	
	System.out.println(" Menu des operations");
	System.out.println(" 1- Addition ");
	System.out.println(" 2- Soustraction ");
	System.out.println(" 3- Multiplication ");
	System.out.println(" 4- Division ");
	
	System.out.println(" Veuillez choisir une operation ");
	int choixOperation = scanner.nextInt();

	float nombre1, nombre2, resultat;
	System.out.println(" Veuillez entrer le premier nombre : ");
	nombre1=scanner.nextFloat();
	System.out.println(" Veuillez entrer le deuxieme nombre : ");
	nombre2=scanner.nextFloat();
	
	switch (choixOperation ) {
	case 1:
		resultat = nombre1 + nombre2;
		System.out.println(" La somme est " + resultat);
		break;
	case 2:
		resultat = nombre1 - nombre2;
		System.out.println(" La soustraction est " + resultat);
		break;
	case 3:
		resultat = nombre1 * nombre2;
		System.out.println(" La multiplication est " + resultat);
		break;
	case 4:
		resultat = nombre1 / nombre2;
		System.out.println(" La division est " + resultat);
		break;
	}
		System.out.println(" Voulez vous effectuer une nouvelle operation ? (o/n) ");
		char reponse = scanner.next().charAt(0);
		if(reponse != 'o') {
			System.out.print(" Au revoir");
//		}else {
//
//			System.out.println(" Veuillez choisir une operation ");
//			
//			System.out.println(" Menu des operations");
//			System.out.println(" 1- Addition ");
//			System.out.println(" 2- Soustraction ");
//			System.out.println(" 3- Multiplication ");
//			System.out.println(" 4- Division ");
//			
////			int choixOperation = scanner.nextInt();
//
//			
//		}
		}	
}	
		while (true);
	}
}
