# Reverse-Number-using-java
I have reversed number in java

Program:

import java.util.*;
public class Main
{
  public static void main (String args[])
  {
	Scanner sc = new Scanner (System.in);
	int n=sc.nextInt();
	int[] arr=new int[n];
	int temp,i;
	for (i=0;i<n;i++){
	arr[i]=sc.nextInt();
  }
  for (i=0;i<n/2;i++){
      temp =arr[i];
      arr[i]=arr[n-i-1];
      arr[n-i-1]=temp;
  }
  System.out.println("Reversed array:");
  for (i=0;i<arr.length;i++){
      System.out.print(arr[i]+" ");
  }
  }
}
