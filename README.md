package ejercicio2222;

import java.util.Scanner;

public class Ejercicio2222 {

    public static void main(String[] args) {
        
    Scanner Sc= new Scanner (System.in); // se esta declarando la libreria 
    // variable de tipo vector o arreglo 
    float[]altura;
    altura = new float[5];
    // lectura y guardar alturas
    for(int i=0;i<5;i++){
        System.out.println("Ingrese la altura de la persona");
    altura[i]=Sc.nextFloat();
    }
    
    
   // calcular promedio 
   float suma=0, promedio=0;
   for(int j=0;j<5;j++){
       suma=suma+altura[j];
   }
        System.out.println("la suma total :"+suma);
   promedio=suma/5;
        System.out.println("Promedio altura"+promedio);
        // contar los mayores y menores 
        int may, men;
        may=0;
        men=0;
        for(int j=0;j<5;j++){
            if (altura[j]>promedio){
            may++;
            } else if(altura[j]<promedio){
                men++;
            }
            
        }
        System.out.println("La cantidad mayor del promedio es:"+may);
        System.out.println("la cantidad mayor del promerio es:"+men);
    }
}
