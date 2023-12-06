# Java-program-for-Sorting-Elements-In-An-Array

Sort the array in Java
Here, in this page we will discuss the program to sort the array in java. We are given with an array and need to print the sorted array. In this page we will discuss various algorithms to sort the given input array.

Sorting element in array by frequency using C++
Method Discussed in this page are :
Method 1 : Using naive approach.
Method 2 : Using inbuilt function
Example
Input : arr[4] = [10, 40, 20, 30]
Output : 10 20 30 40
Method 1 :
Run a loop from 0 to n-1
Inside that loop run another loop from i+1 to n
Check if(arr[i]>arr[j])
Swap arr[i] with arr[j]
Method 1 : Code in Java
Run
public class Main { 
    public static void main(String[] args) { 

       //Initialize array 
       int [] arr = new int [] {10, 40, 30, 20}; 
       int temp = 0; 

       //Sort the array in ascending order 
       for (int i = 0; i < arr.length; i++) { 
           for (int j = i+1; j < arr.length; j++) { if(arr[i] > arr[j]) { 
                 temp = arr[i]; 
                 arr[i] = arr[j]; 
                 arr[j] = temp; 
              } 
           } 
       } 


    //Displaying elements of array after sorting 
    for (int i = 0; i < arr.length; i++) { 
     System.out.print(arr[i] + " "); 
   } 
  } 
}
Output
10 20 30 40
