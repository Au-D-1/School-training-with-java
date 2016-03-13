# School-training-with-java
This contains most school java mini programs

//function description : Fills an prefixed table

// Used library

import java.util.Scanner;

/**
 *
 * @author audi_
 */
public class Week2op1 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        
     //Declares an Scanner named input to input values
    Scanner input = new Scanner(System.in);
    
    //Declaring an integer //
    
    int optie=0;
    
    //Declares an array with an fixed size of 10 by 10
    
    int array[][] = new int[10][10];
    
    // Calls the method named menu and obtains its value
    
     optie = menu(optie);
        
     //While loop checking the value of the optie variable
     
        while( optie < 3){ 
            
        if(optie ==1){
            
        System.out.println("Vul in rij lokatie");
        //gets value for rij
        int rij = input.nextInt();//gets value for rij
        
        System.out.println("Vul in kollom lokatie");
        //gets value for kollom
        int kollom = input.nextInt();
        
        System.out.println("Vul in de waarde");
        //gets value for value
         int waarde = input.nextInt();
    
        array [rij][kollom]= waarde;
        optie = menu(optie);
        
        
        
            
        }
         if(optie == 2){
            //Prints Table until it matches arrays length
         for(int a = 0; a < array.length; a++){
          for(int b = 0; b < array[a].length; b++){
            System.out.print(array[a][b] + " ");
            
          
        }System.out.println();}
            
         optie = menu(optie);
         }
        if(optie == 3){
        
            System.out.println("Goodbye");
        
        }
        
        }}
    
    
        //Method named menu
        public static int menu (int optie){
        Scanner input = new Scanner(System.in);
        
        System.out.println("Kies een optie");
        System.out.println("1.	Cijfer invoer.");
        System.out.println("2.	Array tonen.");
        System.out.println("3.	Afsluiten.");
        
        //gets value for optie
        optie = input.nextInt();
        
        
        //Returns value for optie
        return optie;};
        }
