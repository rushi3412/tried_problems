# tried_problems
in this i have posted problems which i have tried

// print the determinent of a 2*2 matrix

InputStreanReader r = new InputStreanReader (System.in);
bufferedReader

String line1 = br.readLine();
String line2 = br.readLine();

String[] line1Arr = line1.split(regex: " " );

String[] line2Arr = line2.split(regex: " " );

int line1Arrint = new int[2];
int line2Arrint = new int[2];

for(int i=0; i<line1Arrint.length; i++){
line1Arrint[i] = Integer.parseInt();
}

for(int i=0; i<line2Arrint.length; i++){
line2Arrint[i] = Integer.parseInt();
}

int[][] arr = new int [2][2];
arr[0] = line1Arrint; 
int[][] arr = new int [2][2];
arr[1] = line2Arrint;

int ans = arr[0][0]*a[1][1] - arr[1][0]*arr[0][1];

System.out.print(ans);




// printing the elements from an 2D array 

import java.util.*;
public class twoDArr{
    public static void main(String args[]){
        
        int[][] arr = new int[2][3];
        
        int rowLength = arr.length;
        int colLength = arr[0].length;
        
        for(int row=0; row< rowLength; row++){
            for(int col= 0; col<colLength; col++){
               int value =  arr[row][col];
               
               System.out.print(value + " " + "row:" + row + " " + "col:" + col + " " + "|");
            }
            System.out.println();
        }
    }
}
output:-
0 row:0 col:0 |0 row:0 col:1 |0 row:0 col:2 |
0 row:1 col:0 |0 row:1 col:1 |0 row:1 col:2 |




/* print an 2D array of output 1 1 1 
                               1 1 1 */

import java.util.*;
public class twoDArr{
    public static void main(String args[]){
        int[][] arr = new int[2][3];
        
        int row = arr.length;
        int col = arr[0].length;
        
        for(int i=0; i<row; i++){
            for(int j=0; j<col; j++){
                arr[i][j] = 1;
                
                System.out.print(arr[i][j]+ " ");
            }
            System.out.println();
        }
    }
}
output:-
1 1 1 
1 1 1



/* print an 2D array of output 
0 1 2 3 
4 5 6 7 
8 9 10 11 
12 13 14 15
*/


import java.util.*;
public class twoDArr{
    public static void main(String args[]){
        int[][] arr = new int[4][4];
        
        int row = arr.length;
        int col = arr[0].length;
        
        int count =0;
        for(int i=0; i<row; i++){
            for(int j=0; j<col; j++){
                arr[i][j] = count;
                count++;
                
                System.out.print(arr[i][j]+ " ");
            }
            System.out.println();
        }
    }
}
output:-
0 1 2 3 
4 5 6 7 
8 9 10 11 
12 13 14 15


/* print an 2D array of output
1 2 3 
1 2 3 
1 2 3 */

import java.util.*;
public class twoDArr{
    public static void main(String args[]){
        int[][] arr = new int[3][3];
        
        int row = arr.length;
        int col = arr[0].length;
        
        int count =0;
        for(int i=0; i<row; i++){
            for(int j=0; j<col; j++){
                arr[i][j] = j+1;
                count++;
                
                System.out.print(arr[i][j]+ " ");
            }
            System.out.println();
        }
    }
}
output:-
1 2 3 
1 2 3 
1 2 3



/* print an 2D array of output
1 1 1 
2 2 2 
3 3 3

import java.util.*;
public class twoDArr{
    public static void main(String args[]){
        int[][] arr = new int[3][3];
        
        int row = arr.length;
        int col = arr[0].length;
        
        int count =1;
        for(int i=0; i<row; i++){
            for(int j=0; j<col; j++){
                arr[i][j] = i+1;
                
                System.out.print(arr[i][j]+ " ");
            }
            System.out.println();
        }
    }
}
output:-
1 1 1 
2 2 2 
3 3 3



/* print an 2D array of output
1 4 7 
2 5 8 
3 6 9

import java.util.*;
public class Arr{
    public static void main(String args[]){
        int[][] arr = new int[3][3];
        
        int count=1;
        for(int col = 0; col<arr[0].length; col++){
            for(int row=0; row<arr.length; row++){
                arr[row][col] = count;
                count++;
                
            }
            
        }
        for(int row=0; row<arr.length; row++){
            for(int col=0; col<arr[0].length; col++){
                System.out.print(arr[row][col]+ " ");
            }
            System.out.println();
        }
    }
}
output:-
1 4 7 
2 5 8 
3 6 9



/* print an 2D array of output by taking input from the user
147
258
369 */


import java.util.*;
public class Arr{
    public static void main(String args[]){
        Scanner matrix = new Scanner(System.in);
            int N = matrix.nextInt();
            int M = matrix.nextInt();
            
            int[][] arr = new int [N][M];
            int count = 0;
            for(int row = 0; row<arr.length; row++){
                for(int col = 0; col<arr[0].length; col++){
                    arr[row][col] = matrix.nextInt();
                    //count++;
                    System.out.print(arr[row][col]);
                }
                System.out.println();
            }
         
         }
    }
output:-
3 3
147
258
369 




/* simple transpose og matrix 
3
1 4 5
4 5 6
5 3 1
*/

import java.util.*;
public class Arr{
public static void main(String args[]){
Scanner tra = new Scanner(System.in);
int N = tra.nextInt();

int[][] arr = new int[N][N];

for(int i=0; i<N; i++){
for(int j=0; j<N; j++){
arr[][] = new int[i][j];
}
}
for(int i=0; i<N; i++){
for(int j=0; j<N; j++){
int storage = arr[i][j];
arr[i][j] = arr[j][i];
arr[j][i] = storage;
}
}
for(int i=0; i<N; i++){
for(int j=0; j<N; j++){
System.out.print(arr[i][j]);
}
System.out.println();
}
}
}

output:-
3
1 4 5
4 5 6
8 4 2



/*Given a matrix of size M*N, your task is to find the maximum sum of a column.
Input
*/
import java.util.*;
public class arrT{
    public static void main(String args[]){
        Scanner sum = new Scanner(System.in);
        int N = sum.nextInt();
        int M = sum.nextInt();
        
        int[][] arr = new int[N][M];
        
        for(int i=0; i<arr.length; i++){
            for(int j=0; j<arr[0].length; j++){
                arr[i][j] = sum.nextInt();
                
            }
        }
        int maxSum = maxColSum(arr);
        System.out.print(maxSum);
        
    }
    public static int maxColSum(int[][] arr){
        int maxSum = Integer.MIN_VALUE;
        
        for(int col=0; col<arr[0].length; col++){
            int colSum = 0;
            for(int row=0; row<arr.length; row++){
                colSum += arr[row][col];
            }
            if(colSum > maxSum){
                maxSum = colSum;
            }
            maxSum = (colSum > maxSum) ? colSum : maxSum;
        }
        return maxSum;
    }
}

Sample Input:-
3 3
1 2 3
4 5 6
7 8 9

Sample Output:-
18




/*Given a boolean matrix of size N*M in which each row is sorted your task is to print the index of the row containing maximum 1's. If multiple answer exist print the smallest one.
Input
*/


import java.util.*;
public class arr{
    public static void main(String args[]){
        Scanner mat = new Scanner(System.in);
        int N = mat.nextInt();
        int M = mat.nextInt();
        
        int[][] arr = new int[N][M];
        
        for(int i =0; i<arr.length; i++){
            for(int j=0; j<arr[0].length; j++){
                arr[i][j] = mat.nextInt();
            }
        }
        int value = winnerIndexs(arr);
        System.out.print(value);
    }
    
    public static int winnerIndexs(int[][] arr){
        int sum =0; 
        int winnerIndex = 0;
        for(int i=0; i<arr.length; i++){
            int rowSum =0;
            for(int j=0; j<arr[0].length; j++){
                if(arr[i][j] == 1){
                    rowSum += arr[i][j];
                }
                if(rowSum > sum){
                    sum = rowSum;
                    winnerIndex = i;
                }
            }
        }
        return winnerIndex;
    }
}

Sample Input:-
3 5
0 1 1 1 1
0 0 0 1 1
0 0 0 1 1

Sample Output:-
0




/*  Given a matrix of size N*N, your task is to find the sum of the upper triangular matrix and the lower triangular matrix.

For Matrix:-
M00 M01 M02
M10 M11 M12
M20 M21 M22

Upper Triangular:-
M00 M01 M02
_____M11 M12
__________M22

Lower Triangular:-
M00__________
M10 M11_____
M20 M21 M22

*/

import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static void main (String[] args) {
        Scanner mat = new Scanner(System.in);

        int N = mat.nextInt();

        int[][] arr = new int[N][N];

        for(int i=0; i<N; i++){
            for(int j=0; j<N; j++){
                arr[i][j] = mat.nextInt();
            }
        }
        TrianglarMatrix(arr);

    }
    public static void TrianglarMatrix(int[][] arr){

        int upperMatrix = 0;
        int lowerMatrix = 0;

        for(int row =0; row<arr.length; row++){
            for(int col =0; col < arr[0].length; col++){
                if(col >= row){
                    //you are in uppermatrix
                    upperMatrix += arr[row][col];
                }
                if(row >= col){
                    // you are in lowerMatrix
                    lowerMatrix += arr[row][col];
                }
            }
        }
        System.out.print(upperMatrix + " " + lowerMatrix);
    }
}

Sample Input:-
3
1 4 2
1 5 7
3 8 1

Sample Output:-
20 19



// print the diagonal 
1 2 3 
4 5 6
7 8 9 
output 5

import java.util.*;
public class Arr{
    public static void main(String args[]){
        Scanner mat = new Scanner(System.in);
        int N = mat.nextInt();
        int M = mat.nextInt();
        
        int[][] arr = new int[N][M];
        int row = arr.length;
        int col = arr[0].length;
        
                int ans = row + col - 1;
                System.out.print(ans);
            }
        }
    
 
 /* Problem Statement
Given a matrix of size N*N, your task is to find the sum of the primary and secondary diagonal of the matrix.

For Matrix:-
M00 M01 M02
M10 M11 M12
M20 M21 M22

Primary diagonal:- M00 M11 M22
Secondary diagonal:- M02 M11 M20 */


import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static int DiagonalSum(int[][]Matrix, int N){
        int diagonal1 = 0;
        
        for(int i=0; i<N; i++){
            for(int j=0; j<N; j++){
                if(j==i){
                    diagonal1 += Matrix[i][j];
                }
            }
        }
          int diagonal2 = 0;
        for(int i=0; i<N; i++){
            for(int j=N-1; j>=0; j--){
                
                if(j + i == N-1)
                diagonal2 += Matrix[i][j];
            }
        }
    System.out.print(diagonal1 + " " + diagonal2);
    return 0;
    }

       public static void main(String[] args){
              Scanner Mat = new Scanner(System.in);
              int N = Mat.nextInt();
              int[][] Matrix = new int[N][N];
              for(int i = 0; i < N; i++){
                  for(int j = 0; j < N; j++){
                      Matrix[i][j] = Mat.nextInt();
          }
      }
            DiagonalSum(Matrix,N);
   }
}

Sample Input:-
2
1 4
2 6

Sample Output:-
7 6




// Java program to print vowels in a String


import java.util.*;
public class strr{
    public static void main(String args[]){
        Scanner vol = new Scanner(System.in);
        String str = vol.nextLine();
        
        for(int i=0; i<str.length(); i++){
            char ch = str.charAt(i);
            
            if(isVowels(ch)){
                System.out.print(ch + " ");
            }
        }
    }
    
    public static boolean isVowels(char c){
        if(c == 'a' || c == 'e' || c == 'i' || c == 'o' || c == 'u' ){
            return true;
        }else {
            return false;
        }
    }
}



/*
        Reverse the string
        Input=: america
        output=: acirem
 */
 
 import java.util.*;
public class strin{
    public static void main(String args[]){
        Scanner name = new Scanner(System.in);
       String str = name.nextLine();
     //  String str = "america";
       String ansString = "";
       for(int i=str.length() -1; i>0; i--){
           char ch = str.charAt(i);
           ansString += ch;
         //   System.out.println(ansString);
       }
       System.out.println(ansString);

    }
}
 Input=: america
        output=: acirem
        
        

/*
        Reverse the string
        Input=: america
        output=: acirem
        but create a half reveresed triagle of reversed string
a
ac
aci
acir
acire
acirem
 */



import java.util.*;
public class strin{
    public static void main(String args[]){
        Scanner name = new Scanner(System.in);
       String str = name.nextLine();
     //  String str = "america";
       String ansString = "";
       for(int i=str.length() -1; i>0; i--){
           char ch = str.charAt(i);
           ansString += ch;
            System.out.println(ansString);
       }
      // System.out.println(ansString);

    }
}

Input=: america
output=:
a
ac
aci
acir
acire
acirem




/* Given a matrix of size N*N, your task is to find the sum of the upper triangular matrix and the lower triangular matrix.

For Matrix:-
M00 M01 M02
M10 M11 M12
M20 M21 M22

Upper Triangular:-
M00 M01 M02
_____M11 M12
__________M22

Lower Triangular:-
M00__________
M10 M11_____
M20 M21 M22
*/


import java.util.*;
public class arrTwoD {
    public static void main(String args[]) {
    
    Scanner mat = new Scanner(System.in);
    int N = mat.nextInt();
    
    int[][] arr = new int[N][N];
    
    for(int i=0; i<N; i++){
        for(int j=0; j<N; j++){
            arr[i][j] = mat.nextInt();
        }
    }
    TriangularMatrix(arr);
    
    
}
 public static void TriangularMatrix(int[][] arr){
     int upperMatrix = 0;
     int lowerMatrix = 0;
     
     for(int row =0; row<arr.length; row++) {
         for(int col =0; col<arr[0].length; col++){
            if(col >= row){
                // upperMatrix 
                upperMatrix += arr[row][col];
                
            }
            if(row >= col){
                //lowerMatrix
                lowerMatrix += arr[row][col];
            }
         }
     }
     System.out.print(upperMatrix + " " + lowerMatrix);
    }
 }
 
Sample Input:-
3
1 4 2
1 5 7
3 8 1

Sample Output:-
20 19




/* Given a boolean matrix of size N*M in which each row is sorted your task is to print the index of the row containing maximum 1's. If multiple answer exist print the smallest one.
*/

import java.util.*;
public class arrTwoD{
    public static void main(String args[]){
        Scanner mat = new Scanner(System.in);
            int N = mat.nextInt();
            int M = mat.nextInt();
            
            int[][] arr = new int[N][M];
            
            for(int i=0; i<N; i++){
                for(int j=0; j<M; j++){
                    arr[i][j] = mat.nextInt();
                }
            }
        int ans = maxOnces(arr);
        System.out.print(ans);
    }
    
    public static int maxOnces(int[][] arr){
        int sum = 0;
        int winnerIndex = 0;
        
        for(int i=0; i< arr.length; i++){
            int rowSum = 0;
            for(int j=0; j< arr[0].length; j++){
                if(arr[i][j] == 1){
                    rowSum += arr[i][j];
                    
                }
                if(rowSum > sum){
                    sum = rowSum;
                    winnerIndex = i;
                }
            }
        }
        
        return winnerIndex;
    }
}

Sample Input:-
3 5
0 1 1 1 1
0 0 0 1 1
0 0 0 1 1

Sample Output:-
0




/* You are given a string your task is to reverse the given string. */


import java.util.*;
public class arrToD{
    public static void main(String args[]){
        Scanner mat = new Scanner(System.in);
            String s = mat.next();
            
            String ans = reversString(s);
            System.out.print(ans);
    }
    
    public static String reversString(String str){
        StringBuilder ansStr = new StringBuilder();
        
        for(int i=str.length()-1; i>=0; i--){
            char ch = str.charAt(i);
            ansStr.append(ch);
            
        }
    
    return ansStr.toString();
    }
}

Sample Input
abc

Sample Output
cba





/* You are given two binary strings of length N. You have to output a resultant string. The resultant string will be calculated in the following way:

- > For every position i, if the ith character of the first string is '1' and the second string is '0', the resultant string will have '1'. Also, for every position i, if the ith character of the first string is '0' and the second string is '1', the resultant string will have '1'. Rest, all the characters of the resultant string will be '0'. Find the resultant string;

*/


import java.util.*;
public class strj{
    public static void main(String arg[]){
        Scanner stre = new Scanner(System.in);
        int n = stre.nextInt();
        
        String firstStr = stre.next();
        String secondStr = stre.next();
        
        for(int i=0; i<n; i++){
            char ch1 = firstStr.charAt(i);
            char ch2 = secondStr.charAt(i);
            
            boolean b1 = ch1 == '0';
            boolean b2 = ch2 == '0';
            
            System.out.print(b1 ^ b2 ? '1' : '0');
        }
    }
}


Sample Input:
5
10110
01101

Sample Output:
11011



/* Given an n-digit large number in form of string, check whether it is divisible by 7 or not. Print 1 if divisible by 7, otherwise 0
        */
import java.util.*;
public class strj{
    public static void main(String args[]){
        Scanner divi  = new Scanner(System.in);
        String n = divi.next();
        
        int rem = 0;
        for(int i=0; i<n.length(); i++){
            int num = n.charAt(i);
            int d = rem * 10 + num;
            rem = d % 7;
        }
        
        System.out.print(rem == 0 ? '1' : '0');
    }
}

Sample Input:
8955795758

Sample Output:
1


/* There is a robot starting at the position (0, 0), the origin, on a 2D plane. Given a sequence of its moves, judge if this robot ends up at (0, 0) after it completes its moves.

You are given a string moves that represents the move sequence of the robot where moves[i] represents its ith move. Valid moves are 'R' (right), 'L' (left), 'U' (up), and 'D' (down).

Return true if the robot returns to the origin after it finishes all of its moves, or false otherwise.

Note: The way that the robot is "facing" is irrelevant. 'R' will always make the robot move to the right once, 'L' will always make it move left, etc. Also, assume that the magnitude of the robot's movement is the same for each move.  */
dificulty level = **meadium**

import java.util.*;
public class strk{
    public static void main(String args[]){
        Scanner robot = new Scanner(System.in);
        String directions = robot.next();
        
        int x = 0;
        int y = 0;
        for(int i=0; i<directions.length(); i++){
            char dire = directions.charAt(i);
            if(dire == 'U'){
                y++;
            }else if(dire == 'D'){
                y--;
            }else if(dire == 'R'){
                x++;
            }else if(dire == 'L'){
                x--;
            }
        }
        System.out.print(x == 0 && y == 0 ? "True" : "False");
    }
}

Sample Input:
UD

Sample Output:
True



/* sum of all elements using arraylist */

import java.util.ArrayList;
import java.util.Collections;
import java.util.Scanner;

public class practicePro{
    public static void main(String args[]){
        ArrayList<Integer> all = new ArrayList<>();
        
        Scanner li = new Scanner(System.in);
        int n = li.nextInt();
        
        for(int i=0; i<n; i++){
            all.add(li.nextInt());
        }
        
        int ans = sumOfElements(all);
        System.out.print(ans);
    }
    
    public static int sumOfElements(ArrayList<Integer> all){
        int sum = 0;
        for(int i=0; i<all.size(); i++){
            sum += all.get(i);
        }
        
        return sum;
    }
}

input: 5 12 45 78 90 1
output: 226
                                   
                                   
                                   
  /* sum of all elements using arraylist(with different varible name in funcions */                                                                    
                                   
import java.util.ArrayList;
import java.util.Collections;
import java.util.Scanner;

public class proPra{
    public static void main(String args[]){
        ArrayList<Integer> nu = new ArrayList<>();
        
        Scanner el = new Scanner(System.in);
        int n = el.nextInt();
        for(int i=0; i<n; i++){
            nu.add(el.nextInt());
        }
        int ans = sumOfEl(nu);
        System.out.print(ans);
    }
    
    public static int sumOfEl(ArrayList<Integer> al){
        int sum =0; 
        for(int i=0;i<al.size(); i++){
            sum += al.get(i);
        }
        return sum;
    }
}                                   
input: 5 12 45 78 90 1
output: 226                                  
                                   



/* pascal triagle give last line of it */



import java.util.*;
public class pascaArr{
    public static void main(String args[]){
        Scanner tri = new Scanner(System.in);
        int n = tri.nextInt();
        int[] arr = pasclTriangle(n);
        for(int item : arr){
            System.out.print(item + " ");
        }
    }

public static int[] pasclTriangle(int n){
   n = n-1;
    if(n<0){
        return new int[0];
    }
    int[] prevArr = new int[1];
    prevArr[0] = 1; 
    while(n != 0){
        int[] nextRowArray = new int[prevArr.length + 1];
        nextRowArray[0] = 1;
        nextRowArray[nextRowArray.length -1] = 1;
        for(int i=1; i<prevArr.length; i++){
            nextRowArray[i] = prevArr[i] + prevArr[i-1];  
        }
        prevArr = nextRowArray;
        n--;
    }
    return prevArr;
}
}

input: 4
output: [1,3,3,1]
            Explanation: what is a pascal triangle ....
                       1
                      1 1
                     1 2 1
                    1 3 3 1


/* sum of Arraylist elements given by the user (2nd time i did only this time i did it on my own)  */


import java.util.ArrayList;
import java.util.Collections;
import java.util.Scanner;

public class arrLit{
    public static void main(String args[]){
    
    ArrayList<Integer> al = new ArrayList<>();
    Scanner num = new Scanner(System.in);
    int n = num.nextInt();
    
    for(int i=0; i<n; i++){
        al.add(num.nextInt());
     }
     int ans = sumOfArrayList(al);
        System.out.print(ans);
   }
   public static int sumOfArrayList(ArrayList<Integer> al){
   int sum = 0;
   for(int i=0; i<al.size(); i++){
// for(int i=1; i<al.size(); i++){   
        sum += al.get(i);
      }
      return sum; 
    }
 }



*/ pascal Triangle print the row given by the user  (2nd time i did only this time i did it on my own) */

import java.util.*;
public class pastR{
    public static void main(String args[]){
    
        Scanner tri = new Scanner(System.in);
    
        int n = tri.nextInt();
        int[] arr = pascalTriangle(n);
        for(int item: arr){
         System.out.print(item);
         }
    }
        public static int[] pascalTriangle(int n){
                  n = n-1;
              if(n<0){
                  return new int[0];
      }
                  int[] prevArr = new int[1];
                              prevArr[0] = 1;
                  while(n != 0){
              int[] nextRowArr = new int[prevArr.length +1];
                     nextRowArr[0] = 1;
                      nextRowArr[nextRowArr.length - 1] = 1;
               for(int i=1; i<prevArr.length; i++){
          nextRowArr[i] = prevArr[i] + prevArr[i-1];
      }
            prevArr = nextRowArr;
            n--;
    }
          return prevArr;
   }
}
input: 4
output: [1,3,3,1]
            Explanation: what is a pascal triangle ....
                       1
                      1 1
                     1 2 1
                    1 3 3 1  
    

/* Array List In Java

There are n integers are given.

Create an ArrayList

Add elements

Print the elements of arraylist.
*/

import java.util.ArrayList;
import java.util.Scanner;

public class arrList{
    public static void main(String args[]){
        Scanner imp = new Scanner(System.in);
        int n = imp.nextInt();
        ArrayList<Integer> list = new ArrayList<>();
            for(int i=0; i<n; i++){
            list.add(imp.nextInt());
            }
            for(int i=0; i<list.size(); i++){
            System.out.print(list.get(i)+ " ");
            }
    }
}
Sample Input:
5
1 2 3 4 5

Sample Output:
1 2 3 4 5
