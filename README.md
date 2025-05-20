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
