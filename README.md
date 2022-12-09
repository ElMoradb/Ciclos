# Ciclos
package ciclos;

import java.util.Scanner;

public class Ciclos {

   
    public static void main(String[] args) { 
        
       //ciclo1();
       //ciclo002();
       //ciclo3();
       ciclo4();
    } 
    
    
      // 1. Solicitar una cantidad determinada de numeros secuenciales y calcular la suma total de estos.
    public static void ciclo1(){
        Scanner scanner = new Scanner (System.in);
        
        System.out.println("Introduce la cantidad de elementos que quieres sumar ");
        int numE = scanner.nextInt(), elemento, suma=0;
        
        for(int i = 0; i<numE;i++){
            System.out.println("Introduce un elemento ");
            elemento = scanner.nextInt();
            
            suma = suma+elemento;
            
        }
        
        System.out.println("la suma de los elementos es " + suma);
    }
    
    // 2. Pedir los primero 10 numeros impares y calcular el producto.
    public static void ciclo002(){
        long producto = 1;
        
        for(int i=1; i<=20; i+=2){
            producto = producto * i;
        }
        
        System.out.println("El producto es " + producto);
    } 
    
    // 3. Registrar una cantidad determinada de trabajadores: nombre y salario. 
    //Luego, calcular el promedio de los salarios
    
    public static void ciclo3(){ 
        
        
        Scanner scanner = new Scanner(System.in);
        
        String nombre;
        int salario;
        
        for (int i = 0; i < 5; i++){
        System.out.println("Ingrese su nombre ");
        nombre = scanner.nextLine();
        System.out.println("Ingrese su salario ");
        salario = scanner.nextInt();
        
    
        System.out.println("Bienevenido " + nombre + ", su salario es de " + salario + " pesos.");
        }
    } 
    
    // 4. Dadas las edades y alturas de 5 alumnos, mostrar la edad y la estatura media, la cantidad de alumnos mayores de 18,
    // y la cantidad de alumnos que miden mas de 1.75.
    
    public static void ciclo4(){
        
        Scanner scanner = new Scanner(System.in);
        
        int edad;
        int mayorDe18 = 0; 
        int mayorDe175 = 0;
        float estatura, SumaEstatura;
        double promedioEstatura;
        
        for (int i = 0; i < 5; i++){ 
            System.out.print("Edad: ");
            edad = scanner.nextInt();
            
            if (edad > 18){
                mayorDe18++;
            }
            
            System.out.println("Estatura: ");
            estatura = scanner.nextFloat();
            
            if (estatura > 1.75){
                mayorDe175++;
            }
            
            estatura += estatura;
            //promedioEstatura = estatura/5;
        }
        
        System.out.print("Mayor de 18 años: " + mayorDe18);
        System.out.print(" Mayor de 1.75: " + mayorDe175);
        
    }
        
        
    }
