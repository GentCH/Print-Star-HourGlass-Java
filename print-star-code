
import java.util.Scanner;

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

/**
 *
 * @author user
 */
public class Solution {
    
    Solution(){
        
    }
    
    public static void main (String[] args){
        System.out.print("Enter width: ");
        Scanner scan = new Scanner(System.in);
        int starWidth = scan.nextInt();
        System.out.println("");
        printStar(starWidth);
    }
    
    public static void printStar(int width){
        //r = row
        //c = column
        int r, c;
        double totalRow;
        
        //check odd or even number width
        if(width % 2 == 0){
            //+1 to round up if even number width
            width = width + 1;
        }
        
        //calculate total rows to print star
        totalRow = ( ((double)width) / 2) + 0.5;
        
        //print from maximum to minimum star
        for(r=(int)totalRow; r>0; r--){
            //print space before the star
            for(c=(width/2)-r+1;c>0;c--){
                System.out.print(" ");
            }
            //odd number = 2n-1
            for(c=((2*r)-1);c>0;c--){
                System.out.print("*");
            }
            System.out.println("");
        }
        //start to print star from the row after the minimum star
        //r=1 to skip first row(minimum star), since it already printed
        for(r=1; r<(int)totalRow; r++){
            //print space before the star
            for(c=(width/2)-r; c>0; c--){
                System.out.print(" ");
            }
            //use even number formula, because r start from 1
            //even number = 2n
            for(c=0; c<=((2*r)); c++){
                System.out.print("*");
            }
            System.out.println("");
        }
    }
}
