# ejercicio6
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package ejercicio6;

import java.util.Scanner;

/**
 *
 * @author sale7
 */
public class Ejercicio6 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner sn=new Scanner(System.in);
    boolean creciente=true;
   int array[]=new int[10];

  do{ 
for(int i=0;i<10;i++){
      System.out.println("digite un numero");   
      array[i]=sn.nextInt();
    }
    
    for(int i=0;i<9;i++){
     if(array[i]<array[i+1]){
       creciente =true;  
     }
     if(array[i]>array[i+1]){
         creciente=false;
         break;
     }
    }
    if(creciente==false){
        System.out.println("\nEl arreglo no esta ordenado en fornma creciente,vuelva a digitar ");
        
    }
    
  }while(creciente==false); 
 
  System.out.println("Los numero en desorden:");         
   System.out.println(array[5]);
   System.out.println(array[2]);     
   System.out.println(array[0]);
   System.out.println(array[9]);
   System.out.println(array[3]);
   System.out.println(array[1]);
   System.out.println(array[4]);
   System.out.println(array[8]);
   System.out.println(array[7]);
   System.out.println(array[6]);
 
    }
    
}
