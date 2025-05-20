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
