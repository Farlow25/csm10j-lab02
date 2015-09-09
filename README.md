# csm10j-lab02
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package ch3_prexercise1;
import java.io.FileNotFoundException;
import java.util.Scanner;
import java.io.FileReader;
import java.io.PrintWriter;
import java.util.logging.Level;
import java.util.logging.Logger;

/**
 *
 * @author Cody
 */
public class CH3_PrExercise1 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner inFile = null;
        PrintWriter outFile = null;
        try {
            inFile = new Scanner(new FileReader("inData.txt"));
        } catch (FileNotFoundException ex) {
            System.out.println("Oops, I couldn't find the file");
        }
        try {
            outFile = new PrintWriter("outData.txt");
        } catch (FileNotFoundException ex) {
            System.out.println("Oops, you dun goofed");
            
        }
        String str;
        double numr = 10.20;
        double numa = 5.35;
        double numb;
        numb = numr * numa;
        double ttl;
        ttl = numr + numr + numa + numa;
        outFile.print("Rectangle: " + "\n");
        outFile.println((" Length = ") + numr + (", width = ") + numa + (", area = ") + numb + (", parameter = ") + ttl + "\n");
        double r1 = 45.60;
        double p1 = 3.1416;
        double ar = p1 * (r1 * r1);
        double cir1 = 2 * p1 * r1;
        char A = 'A';
        
        
                
        outFile.print("Circle: " + "\n");
        outFile.println(" Radius = " + r1 + ", area = " + ar + ", circumference = " + cir1 + "\n");
        
        double beginingBalance;
        //double grossAmount;
        double beginningBalance = 18500;
        double percentInterest = 3.5;
        double grossAmount;
        char letter = 'A' + 1;
        grossAmount = beginningBalance + (beginningBalance * (percentInterest / 100));
        outFile.println("Beginning Balance = $" + beginningBalance + ", interest rate = " + percentInterest + "\n");
        outFile.println("Balance at the end of the month = $" + grossAmount + "\n");
        outFile.println(letter);
        
        outFile.close();
        
        System.out.println("Rectangle: ");
        System.out.println(("Length = ") + numr + (", width = ") + numa + (", area = ") + numb + (", parameter = ") + ttl + "\n");
        System.out.println("Circle: ");
        System.out.println("Radius = " + r1 + ", area = " + ar + ", circumference = " + cir1 + "\n");
        System.out.println("Randy" + " Gill" + " age: 31");
        grossAmount = beginningBalance + (beginningBalance * (percentInterest / 100));
        System.out.println("Beginning Balance = $" + beginningBalance + ", interest rate = " + percentInterest);
        System.out.println("Balance at the end of the month = $" + grossAmount + "\n");
        System.out.println(letter);
//System.out.println(("Name: Randy Gill, ")
               // + ("age: 31"));
        
       
                
    }
    
}
