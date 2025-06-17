// Online Java Compiler
// Use this editor to write, compile and run your Java code online

import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner teclado = new Scanner(System.in);
        
        int n1 = 0;
        int somatorio = 0;
        int maior = 0;
        int contador = 1;
        int menor = 1000000;
        
        while (contador<=10){
            System.out.print("digite o numero "+ contador + ": ");
            n1 = teclado.nextInt();
            if (menor>n1) {
                menor = n1;
            }
            
            if (maior<n1) {
                maior = n1;
            }
            
            somatorio += n1;
            
            
            contador++;
        }
        
        
        
        
        
        System.out.println("menor: "+ menor);
        System.out.println("maior: "+ maior);
        System.out.println("somatorio: " + somatorio/10);
        
        
        
    
        
        
    }
}



--------------------------


import java.util.Scanner;
class Main {
    public static void main(String[] args) {
        Scanner teclado = new Scanner(System.in);

        System.out.print("Informe sua velocidade: ");
        int vel = teclado.nextInt();
            
        if(vel <= 40){
            System.out.print("Voce estava a " + vel +"km/h e voce recebera R$ 00,00 reais de multa!");
        }else if(vel > 41 & vel <= 60){
            System.out.print("Voce estava a " + vel + "km/h e voce recebera R$ 50,00 reais de multa!");
        }else if(vel > 61 & vel <= 80){
            System.out.print("Voce estava a " + vel + "km/h e voce recebera R$ 100,00 reais de multa!");
        }else if(vel > 81 & vel <= 100){
            System.out.print("Voce estava a " + vel + "km/h e voce recebera R$ 200,00 reais de multa!");
        }else{
            System.out.print("Voce estava a " + vel + "km/h e voce recebera R$ 400,00 reais de multa!");
        }
    }
}



--------------------
mesmo exercicio acima mas outro codigo 

import java.util.Scanner;

public class MultaVelocidade {
    public static void main(String[] args) {
        Scanner teclado = new Scanner(System.in);

        System.out.print("Digite a velocidade: ");
        int velocidade = teclado.nextInt();

        int multa;

        if (velocidade >= 0 && velocidade <= 40) {
            multa = 00;
        } else if (velocidade >= 41 && velocidade <= 60) {
            multa = 50;
        } else if (velocidade >= 61 && velocidade <= 80) {
            multa = 100;
        } else if (velocidade >= 81 && velocidade <= 100) {
            multa = 200;
        } else {
            multa = 00; 
        }

        System.out.println("Valor da multa: R$ " + multa);
        
     
    }
}




-----------------------------------------

outro metodo 


import java.util.Scanner;

public class MultaVelocidade {
    public static void main(String[] args) {
        Scanner teclado = new Scanner(System.in);

        System.out.print("Digite a velocidade: ");
        int velocidade = teclado.nextInt();

        int multa;

        if ( velocidade <= 40) {
            multa = 00;
        } else
        if ( velocidade <= 60) {
            multa = 50;
        } else
        if ( velocidade <= 80) {
            multa = 100;
        } 
        else if (velocidade <= 100) {
            multa = 200;
        } else {
            multa = 00; 
        }

        System.out.println("Valor da multa: R$ " + multa);
        
     
    }
}




---------------------------



// Online Java Compiler
// Use this editor to write, compile and run your Java code online

import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner teclado = new Scanner(System.in);
        
    
    
    int maiorSalario = 0;
    int salarioAlto = 0;
        
    System.out.print("pessoa 1 \n digite o salario: ");
    int salario = teclado.nextInt();
    System.out.print("informe a quantidade de filhos: ");
    int filhos = teclado.nextInt();
     System.out.print("informe a quantidade de filhos: ");
    int filhos = teclado.nextInt();
        
        
    }
}



-------------------------------------------------------------------------


urna com contagem de votos ate 10


import java.util.Scanner;
public class Urna {

	public static void main (String[] args) {
		
		Scanner teclado = new Scanner(System.in);
		
		int candA = 0;
		int candB = 0;
		int candC = 0;
		int candD = 0;
		
		System.out.println("escolha seu candidato !");
		System.out.println("para o candidato A digite 1");
		System.out.println("para o candidato B digite 2");
		System.out.println("para o candidato C digite 3");
		System.out.println("para o candidato D digite 4");
		
		
		int c = 0;
		
		
		while (c<=10) {
		    System.out.println("escohla o candidato");
		    int escolha = teclado.nextInt();
		    
		if (escolha==1) {
			candA+=1;
		} else if (escolha==2) {
			candB+=1;
		} else if (escolha==3) {
			candC+=1;
		} else if (escolha==4) {
			candD+=1;
		} else {
		    System.out.print("nenhum voto debitado !");
		}
		 c++;
		}
		
		System.out.println("votos do A: "+ candA);
		System.out.println("votos do B: "+ candB);
		System.out.println("votos do C: "+ candC);
		System.out.println("votos do D: "+ candD);
		
		
		
	}
	
}


--------------------------------------------------------------------

urna eletronica com um botao para encerrar ! fiz para encerrar pressionando 5 

import java.util.Scanner;
public class Urna {

	public static void main (String[] args) {
		
		Scanner teclado = new Scanner(System.in);
		
		int candA = 0;
		int candB = 0;
		int candC = 0;
		int candD = 0;

		int escolha = 0;
		
		while (escolha!=5) {
		System.out.println("escolha seu candidato !");
		System.out.println("para o candidato A digite 1");
		System.out.println("para o candidato B digite 2");
		System.out.println("para o candidato C digite 3");
		System.out.println("para o candidato D digite 4");
  
		     escolha = teclado.nextInt();
		    
		if (escolha==1) {
			candA+=1;
		} else if (escolha==2) {
			candB+=1;
		} else if (escolha==3) {
			candC+=1;
		} else if (escolha==4) {
			candD+=1;
		} 
		
		
		}
		
		System.out.println("votos do A: "+ candA);
		System.out.println("votos do B: "+ candB);
		System.out.println("votos do C: "+ candC);
		System.out.println("votos do D: "+ candD);
	
	}
	
}


------------------------------------------------------------------






