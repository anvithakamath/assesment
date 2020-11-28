# assesment
assesment
package com.jspiders.first;

import java.io.File;
import java.io.FileInputStream;
import java.io.FileNotFoundException;
import java.io.FileWriter;
import java.lang.reflect.Array;
import java.util.ArrayList;
import java.util.Arrays;

import java.util.Scanner;



class Item {
	  String name;
	  int price;

	  public Item(String name, int price) {
	    this.name = name;
	    this.price = price;
	  }

	  public String toString() { 
	      return this.name + ": " + this.price;
	  }
	}

	public class Main {
	  public static void main(String[] args) throws Exception {
	    FileInputStream a=new FileInputStream("C:\\Users\\Anvitha\\Desktop\\REPORTS\\1.html");       
	    Scanner sc=new Scanner(a);
	    int number_of_employees = Integer.parseInt(sc.nextLine().split(": ")[2]);
	    sc.nextLine();sc.nextLine(); sc.nextLine(); 
	    
	   
		Arrays[] a1 = new Arrays[number_of_employees];
		
		
		for(Arrays s : a1) {
	        String[] s2 = ((String) s).split(" ");
	        for(String results : s2) {
	            System.out.println(results);
	        }
	    }

	    while(sc.hasNextLine())  
	    {
	      String current[] = sc.nextLine().split(": ");
	      Arrays.sort(a1);
	      for (int i = 0; i < a1.length; i++) {
	      System.out.println(a1[i]);
	      };
	      
	      
	      
		  
	    sc.close();
	    FileWriter fw = new FileWriter("C:\\\\Users\\\\Anvitha\\\\Desktop\\\\REPORTS\\\\2.html");
	    fw.write("The goodies selected for distribution are:\n\n");
	    

	    fw.write("\nAnd the difference between the chosen goodie with highest price and the lowest price is ");
		  fw.close();

	    
	  
	  }
	  }
	}
	




