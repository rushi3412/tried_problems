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




/* simple transpose of matrix 
3
1 4 5
4 5 6
5 3 1
*/

import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static void main (String[] args) {
        Scanner tran = new Scanner(System.in);
            int N = tran.nextInt();

            int[][] arr = new int[N][N];

            for(int i=0; i<N; i++){
                for(int j=0; j<N; j++){
                    arr[i][j] = tran.nextInt();
                }
            }
            for(int i=0; i<N; i++){
                for(int j=0; j<N; j++){
                    if(j>i){
                    int storage = arr[i][j];
                    arr[i][j] = arr[j][i];
                    arr[j][i] = storage;
                    } 
                }
            }
            for(int i=0; i<N; i++){
                for(int j=0; j<N; j++){
                    System.out.print(arr[i][j]+ " ");
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


/* Given an ArrayList of N lowercase characters. The task is to insert given elements in the list and count frequency of elements present in the list.

You can use some inbuilt functions as:-
add() to append element in the list
contains() to check an element is present or not in the list
collections.frequency() to find the frequency of the element in the list.
*/

public static void insert(ArrayList<Character> clist, char c){
    clist.add(c);
}
public static void freq(ArrayList<Character> clist, char c){
    if(clist.contains(c)){
        int countHowMany = Collections.frequency(clist, c);
        System.out.print(countHowMany);
    }else {
        System.out.print("Not Present");
    }
    
}
Sample Input:
2
6
i n i e i w i t i n f n
4
i c i p i p f f

Sample Output:
2
Not Present



/* Classes at NITAP is finally starting after the summer break and students have to reach the campus to avoid the late fine of Rs 500 for semester registration. Mohan, Shreya and Anuj live in the same town. They are deciding on a date to book their train ticket. Everyone has a demand each.
• Mohan wants the ticket at least on date A.
• Shreya wants the ticket at most by date B.
• Anuj wants the ticket atleast on date C.
Find if there is a date where all of them can take the ticket.
*/

import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static void main (String[] args) {
        // Your code here
        Scanner tic = new Scanner(System.in);
            int t = tic.nextInt();
            
            for(int i=0; i<t; i++){
                int A = tic.nextInt();
                int B = tic.nextInt();
                int C = tic.nextInt();

                if(B >= A && B >= C) {
                    System.out.println("YES");
                }else {
                    System.out.println("NO");
                }
            }
        }
    }
    
Sample Input
4
13 16 12
14 15 16
13 16 16
15 13 17
Sample Output
YES
NO
YES
NO


/* Given an array A of N integers, find whether there exists three consecutive same integers in the array.
*/


import java.util.*;

public class Main{
    public static void main(String args[]){
    
    Scanner lin = new Scanner(System.in);
    int n = lin.nextInt();
    int[] arr = new int[n];
    
    for(int i=0; i<n; i++){
        arr[i] = lin.nextInt();
        }
        boolean = false;
        for(int i=0; i<n-2; i++){
            if(arr[i]==arr[i+1] && arr[i]==arr[i+2]){
                ans = true;
                break;
            }
        }
        if(ans == true){
            System.out.print("Yes");
        }else{
            System.out.print("No");
      }
    }
}
Sample Input
5
1 2 2 2 4

Sample Output
Yes

Explanation: The segment [2, 2, 2] follows the criterion.

   
    
    
    
    /*Mohan was so excited to visit his college NIT Arunachal Pradesh campus after COVID along with his friends Shreya and Anuj. The Warden allocated the hostel room for him but he was curious to know about the fact that how students are getting rooms.
The warden told him that those students whose roll no are divisible by 2 they will get PAPUM HOSTEL and if it odd then they will get LOHIT HOSTEL. If the student is girl, then she will get ‘Upper Wing’ otherwise ‘Lower Wing’.
    */
    

import java.util.*;


public class Main {
    public static void main (String[] args) {
    
        Scanner hostel = new Scanner(System.in);
        int t = hostel.nextInt();
        for(int i=0; i<t; i++){
            int R = hostel.nextInt();
            char S = hostel.next().charAt(0);
        if(R % 2 == 0){
            if(S == 'G'){
                System.out.println("PAPUM U");
            }else {
                System.out.println("PAPUM L");
            }
        }
            if(R % 2 != 0){
                if(S == 'G'){
                    System.out.println("LOHIT U");
                }else {
                    System.out.println("LOHIT L");
            }
          }  
        }
    }
}
Sample Input
2
30 B
35 G
Sample Output
PAPUM L
LOHIT U
Explanation
Here 30 is evenly divisible by two and B is the boy so he gets the Papum Hostel and allocated the room at lower wing.

                          
                          
    /* coount the freqency of a element if it is greter than equal to 3 then print Yes else print No.   */                   
                          
                          
import java.util.*; 
                          
public class Main {
    public static void main (String[] args) {    
                          
        Scanner con = new Scanner(System.in);
        int N = con.nextInt();
        int[] arr = new int[N];

        for(int i=0; i<N; i++){
            arr[i] = con.nextInt();
        }

        int total = 1;
        int repeted = 0;
        for(int i=0; i<arr.length; i++){
            for(int j=i; j<arr.length; j++){
            if(arr[j] == arr[i]){
                repeted = arr[i];
                total++;
            }
        }        
     }
     if(total > 3){
            System.out.print("YES");
        }else {
            System.out.print("NO");
        }
    }     
}                         
Sample Input
5
1 2 2 2 4

Sample Output
Yes 
    
Sample Input
5
2 1 5 2 2

Sample Output
Yes     

         
/* Sara's Phone has N apps and each app takes K unit of memory. Now Sara wants to release M units of memory. Your task is to tell the minimum apps Sara needs to delete or say it is not possible.
*/

static int Phone(int N, int K, int M){
  int totalSpaceTakenByApps = N*K;

int spaceWeNeed;

if(M <= totalSpaceTakenByApps){
    spaceWeNeed = M/K;
    
    int remainingSpace = M%K;
    int appsWeNeedToDelete = spaceWeNeed + reamainingSpace;
    return appsWeNeedToDelete;
}
return -1;
}

Sample Input:-
10 3 10

Sample Output:-
4

Sample Input:-
10 3 40

Sample Output:-
-1


/* N people are standing in a queue in which A of them like apple and B of them like oranges. How many people like both apple and oranges.

Note:- It is guaranteed that each and every person likes at least one of the given two.
*/

static int LikesBoth(int N, int A, int B){
  int ans = A + B - N;

      return ans;
    }
    
Sample Input:-
5 3 4

Sample Output:-
2

Sample Input:-
5 5 5

Sample Output:-
5



/* get the sum of first n digits 
    input 4 
    output 10
 */


import java.util.*;
public class pra{
    public static void main(String args[]){
    
    Scanner sn = new Scanner(System.in);
    int n = sn.nextInt();
    int ansRecursion = sumRecursion(n);
    System.out.print(ansRecursion);
   }
   
   public static int sumRecursion(int n){
    //base case
    if(n == 0){
        return 0;
    }
   // work + faith
    int faith = sumRecursion(n-1);
    int sum = n + faith;
    return sum;
    }
 }
 input : 4 
 output: 10

                              
                              
                              
       /* to print N to 1 in decreasing order
             input 5
             output 5 4 3 2 1
                             
       */                       
                              
 import java.util.*;
  public class prac1Recur{
     public static void main(String args[]{
        Scanner sn = new Scanner(System.in);
          int n = sn.nextInt();
          decresinRecur(n);
          
      }
      public static void decresinRecur{
         // base case
     if(n == 0){
       return;
     }
        //work
     System.out.print(n+ " ");
                              
    //faith   
     decreasinRecur(n - 1);
      return;
     }
  }
   input 5
   output 5 4 3 2 1


/* to print 1 to N in incresing order 
input 4 
output 1 2 3 4 


import java.util.*;
public class praRe{
    public static void main(String args[]){
        Scanner sn = new Scanner(System.in);
        int n = sn.nextInt();
        increseRec(n);
  }
    public static void increseRec(int n){
    //base case
    if (n == 0){
        return;
        }
         // work
    increseRec(n - 1);
        // faith
    System.out.print(n+ " ");
    }  
}
input 4 
output 1 2 3 4


/* Write a recursive program to remove all tabs or spaces from a string. */

import java.util.*;
public class recurSpace{
    public static void main(String args[]){
        Scanner space = new Scanner(System.in);
        String n = space.nextLine();
        StringBuilder str1 = new StringBuilder();
        removeSpace(str1, n, 0);
        System.out.print(str1);
    }
    public static void removeSpace(StringBuilder str1, String inStr, int i){
        if(inStr.length() == i){
            return;
        }
        if(inStr.charAt(i) != ' ' && inStr.charAt(i) != '\t'){
            str1.append(inStr.charAt(i));
        }
        removeSpace(str1, inStr, ++i);
    }
}
Sample Input:
H e llo Wo r l d

Sample Output:
HelloWorld



/* Given an integer array arr[] of size N and an element X. The task is to find and print the indices of the given element if it is present in array if not then print “Not found” without quotes.

Note: The elements may be present more than once.
*/

import java.util.*;
public class findingEle{
    public static void main(String[] args){
        Scanner ele = new Scanner(System.in);
              int T = ele.nextInt();
    
         while(T-- != 0){
              int n = ele.nextInt();
              int target = ele.nextInt();
     
              int[] arr = new int[n];
                 for(int i=0; i<n; i++){
                  arr[i] = ele.nextInt();
            }
              ArrayList<Integer> ans = findEle(arr, target);
                     if(ans.size() != 0){
                         for(int i=0; i<ans.size(); i++){
                             System.out.print(ans.get(i)+ " ");
            }
             System.out.println();
         }else {
           System.out.print("Not found");
       }
     }
  }
  public static ArrayList<Integer> findEle(int[] arr, int target){
         ArrayList<Integer> list = new ArrayList<>();
              for(int i=0; i<arr.length; i++){
             if(arr[i] == target){
      list.add(i);
    }
    
                  
     }
         return list;
   }
}
Input:
2
5 6
2 3 6 5 6
4 3
2 4 6 5

Output:
2 4
Not found



/*
Problem Statement
Summer is at its peak in Australia. Freddy is planning to purchase a water cooler to keep his room cool. He has two options available:
Rent a cooler at the cost of X coins per month.
Purchase a cooler for Y coins.
Given that the summer season will last for M months in Australia, Help Freddy in deciding wether he should rent the cooler or not. Renting of cooler will be possible only when the total renting cost will be less than purchasing it. Print "YES" if he rent's it otherwise print "NO".

Sample Input :
3
5 10 1
5 10 2
5 10 3
Sample Output :
YES
NO
NO
Explanation :
Cost of renting the cooler = 5 coins. Cost of purchasing the cooler = 10 coins. So, Freddy should rent the cooler as the cost of renting the cooler for 1 month is strictly less than purchasing it.
Cost of renting the cooler = 10 coins. Cost of purchasing the cooler = 10 coins. So, Freddy should not rent the cooler as the cost of renting the cooler for 2 months is not strictly less than purchasing it.
Cost of renting the cooler = 15 coins. Cost of purchasing the cooler = 10 coins. So, Treddy should not rent the cooler as the cost of renting the cooler for 3 months is not strictly less than purchasing it.
*/


import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static void main (String[] args) {
        // Your code here
        Scanner dilemma = new Scanner(System.in);
        int T = dilemma.nextInt();
        


        while(T > 0){

                int rentPrice = dilemma.nextInt();
                int purchasePrice = dilemma.nextInt();
                int duration = dilemma.nextInt();
                
            int rentingPrice = rentPrice * duration;

            if(rentingPrice < purchasePrice){
                System.out.println("YES");
            }else {
                System.out.println("NO");
            }
            T--;
        }
    }
}

Sample Input :
3
5 10 1
5 10 2
5 10 3
Sample Output :
YES
NO
NO




/* 
print the freqency of each elements in the following array 
1, 2, 2, 2, 3, 3, 5, 20,20, 20
*/

import java.util.*;
public class Main{
    public static void main(String args[]){
    int[] arr = {1,2,2,2,3,3,5,5,10,10,19,19,19,20};
    int[] arr1 = new int[50];
    
    for(int i=0; i<arr.length; i++){
        arr1[arr[i]]++;
        
      }
   for(int i=0; i<arr1.length; i++){
        if(arr1[i] > 0){
        System.out.println(i + " " + arr1[i]);
     }
   }
 }
}
input : 1, 2, 2, 2, 3, 3, 5, 20,20, 20
output: 
1 1
2 3
3 2
5 1
20 3
       
        
/*
    Given an array of N elements, your task is to find the count of repeated elements. Print the repeated elements in ascending order along with their frequency.
Have a look at the example for more understanding.
*/
    
import java.util.*;
import java.io.*;
public class Main{
    public static void main(String args[]){
    
    Scanner freq = new Scanner(System.in);
    int N = freq.nextInt();
    
    int[] arr = new int[N];
    int[] arr1 = new int[1000000];
    
    for(int i=0; i<arr.length; i++){
       arr[i] = freq.nextInt();
     }                   
    for(int i=0; i<arr.length; i++){
        arr1[arr[i]]++;
     }
      for(int i=0; i<arr1.length; i++){
        if(arr1[i] > 1){
            System.out.println(i + " " + arr1[i]);
       }
    }
  }
}
Sample Input:-
5
3 2 1 1 2

Sample Output:-
1 2
2 2


/*
check if given string is angram or not
*/


import java.util.*;
public class jdf{
    public static void main(String args[]){
      //  Scanner fre = new Scanner(System.in);
        int[] arr = new int[26];
        
        String str = "dad";
        String str1 = "min";
        
        for(int i=0; i<str.length(); i++){
            char c = str.charAt(i);
            int index = (int)(c - 'a');
            arr[index]++;
        }
        
        for(int i=0; i<str1.length(); i++){
            char c = str1.charAt(i);
            int index = (int)(c - 'a');
            arr[index]--;
        }
        boolean ana = true;
        for(int i=0; i<arr.length; i++){
            if(arr[i] != 0){
                ana = false;
            }
        }
        if(ana == true){
            System.out.print("YES");
        }else {
            System.out.print("NO");
        }
     
    }
}
input : "dfjk" "dfjk"
output:
YES

                                   
                                   

                                   
/*
Given a binary array of size N. Count number of 1's and 0's in the array.                                  
*/                                  
                                   
 import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static void main (String[] args) {
        Scanner binar = new Scanner(System.in);
        int n = binar.nextInt();
        int[] arr = new int[n];
      //  int[] arr1 = {0,1};

        for(int i=0; i<n; i++){
            arr[i] = binar.nextInt();
        }
        int countOfOne = 0;
       // int countOfZero = 0;

        for(int i=0; i<n; i++){
            if(arr[i] == 1){
                 countOfOne++;
               //  countOfZero++;
            }
           
        }
         int countOfZero = 0;
    for(int i=0; i<n; i++){
        if(arr[i] == 0){
            countOfZero++;
        }
    }
    System.out.print(countOfOne+ " ");
      //  for(int i=0; i<arr1.length; i++){
            System.out.print(countOfZero);

    }
   
}
Input:
5
0 1 1 0 1

Output:
3 2            




/*
Given a 2D integer array matrix or size n x n, print the transpose of the given matrix.
*/

import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static void main (String[] args) {
        Scanner tran = new Scanner(System.in);
            int N = tran.nextInt();

            int[][] arr = new int[N][N];

            for(int i=0; i<N; i++){
                for(int j=0; j<N; j++){
                    arr[i][j] = tran.nextInt();
                }
            }
            for(int i=0; i<N; i++){
                for(int j=0; j<N; j++){
                    if(j>i){
                    int storage = arr[i][j];
                    arr[i][j] = arr[j][i];
                    arr[j][i] = storage;
                    } 
                }
            }
            for(int i=0; i<N; i++){
                for(int j=0; j<N; j++){
                    System.out.print(arr[i][j]+ " ");
                }
                System.out.println();
        }
    }
}
Sample input:
3
1 2 3
4 5 6
7 8 9

Sample Output:
1 4 7
2 5 8
3 6 9



/*
Implement Selection Sort on a given array, and make it sorted.
*/

import java.util.*;
public class sect{
    public static void main(String args[]){
        Scanner set = new Scanner(System.in);
        int n = set.nextInt();
        
        int[] arr = new int[n];
        
        for(int i=0; i<n; i++){
            arr[i] = set.nextInt();
        }
        for(int i=0; i<n; i++){
            sel(arr);
            System.out.print(arr[i]+ " ");
        }
    }
    public static void sel(int[] arr){
        for(int i=0; i<arr.length; i++){
            int lowest = i;
            
            for(int j=i+1; j<arr.length; j++){
                if(arr[j] < arr[lowest]){
                    lowest = j;
                }
            }
            int temp = arr[lowest];
            arr[lowest] = arr[i];
            arr[i] = temp;
        }
    }
}
Sample Input:
3
3 1 2

Sample Output:
1 2 3

                                         
                                         
 /*
Given an array A[ ] of size N containing positive integers, find maximum and minimum elements from the array.
*/
                                         
                                         
import java.util.*;
public class maxMn{
    public static void main(String args[]){
        Scanner ele = new Scanner(System.in);
            int T = ele.nextInt();
            
            while(T-- > 0){
                
                int N = ele.nextInt();
                int[] arr = new int[N];
                
                for(int i=0; i<N; i++){
                    arr[i] = ele.nextInt();
                }
                int max = arr[0];
                int min = arr[0];
                for(int i=0; i<N; i++){
                    if(arr[i] > max)
                        max = arr[i];
                        if(arr[i] < min)
                            min = arr[i];
                }
                System.out.println(max + " " + min);
        }
    }
}
Sample Input:
2
5
7 3 4 5 6
4
1 2 3 4

Sample Output:
7 3
4 1 





/*
Given an array of N integers, give the number with maximum frequency. If multiple numbers have maximum frequency print the maximum number among them.
*/


import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static void main (String[] args) {
        Scanner maxFre = new Scanner(System.in);
        int N = maxFre.nextInt();
        int[] arr = new int[N]; // {1 2 9 1 9 3 2 9 4 2}
        int[] countArray = new int[10000]; // [0 2 3 1 1 0 0 0 0 3]
        int maxcount = 0;
        int element = 0;

        for(int i=0; i<N; i++){
            arr[i] = maxFre.nextInt();
        }
        for(int i=0; i<N; i++){ // i = 10
           /* max =*/ countArray[arr[i]]++;    //        -->  countArray[arr[9]]++; --> countArray[2]++
        }  
        // maxcount = 3        element = 2
        for(int i=0; i<countArray.length; i++){ // i = 9

            if(countArray[i] > maxcount){ //   3 > 3
                maxcount = countArray[i];
                element = i;
    
            }else if(countArray[i] == maxcount && i > element){ // 3 == 3  && 9 > 2 
                element = i; 
            }
        }
        System.out.print(element);
    }
    
}
Sample Input
5
1 4 2 4 5

Sample Output
4

Explanation:-4 has max frequency=2


/*
Maruti is having an array nums having n integers in it. the first element of the array is the leader of it but Maruti doesn't like that so he wants to remove that element and make the second element as a leader.
Now print the elements of array nums modified by Maruti.
*/

import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static void main (String[] args) {
        // Your code here
        Scanner firstEle = new Scanner(System.in);
        int n = firstEle.nextInt();
        int[] arr = new int[n];

        for(int i=0; i<n; i++){
            arr[i] = firstEle.nextInt();
        }
        boolean removeFirst = false;
        for(int i=0; i<n; i++){
            if(arr[i] != 0){
               removeFirst = true;
            }
        }
        if(removeFirst == true){
            for(int i= 1; i<n; i++){
                System.out.print(arr[i]+ " ");
            }
        }
    }
}
Sample Input:
6
1233 1324 545 23 656 76
Sample Output:
1324 545 23 656 76



/*
Question: Median of an array
        Input: [7 ,5, 1, 8, 3, 6, 0, 9, 4,2]
        Output: 4.5
        explanation: after sorting take numers which are in the middle...
*/


import java.util.*;
public class searched{
    public static void main(String args[]){
        Scanner mead = new Scanner(System.in);
        
        int N = mead.nextInt();
        
        int[] arr = new int[N];
        
        for(int i=0; i<N; i++){
            arr[i] = mead.nextInt();
        }
        double ans = meadian(arr);
        System.out.print(ans);
    }
    
    public static double meadian(int[] arr){
        Arrays.sort(arr);
            if(arr.length % 2 == 0){
                int meadian1 = arr.length/2;
                int meadian2 = (arr.length/2) - 1;
                
                return (arr[meadian2] + arr[meadian1]) /2.0;
            }else {
               return arr[arr.length/2];
            }
        }
}

Input: [7 ,5, 1, 8, 3, 6, 0, 9, 4,2]
Output: 4.5

                            
                            
/*
    Question: Mean of an array
    Input: [10, 90, 100]
    Output: 200 /3 = 66.666;
    Explanation: average. Add all the marks and divide it to number of subjects.....
*/                            
                            
import java.util.*;
public class searched{
    public static void main(String args[]){
        Scanner mead = new Scanner(System.in);
        
        int N = mead.nextInt();
        
        int[] arr = new int[N];
        
        for(int i=0; i<N; i++){
            arr[i] = mead.nextInt();
        }
        double ans = meadian(arr);
        System.out.printf("%.2f", ans);
    }
    
    public static double meadian(int[] arr){
       double sum = 0.0;
       for(int i=0; i<arr.length; i++){
           sum += arr[i];
       }
       return sum / arr.length;
    }
}                            
Input: [10, 90, 100]
Output: 200 /3 = 66.666;                            




/*
1. Two Sum
Easy

Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.
You can return the answer in any order.
*/
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].

class Solution {
    public int[] twoSum(int[] nums, int target) {
       
        for(int i=0; i<nums.length; i++){
             for(int j=i+1; j<nums.length; j++){
                 if(nums[i] + nums[j] == target){
                     return new int[] {i, j};
                 }
             }
        }
         return new int[] {};
    }
}
Input: nums = [2,7,11,15], target = 9
Output: [0,1]

                            
                            
/*
1920. Build Array from Permutation
Easy
Given a zero-based permutation nums (0-indexed), build an array ans of the same length where ans[i] = nums[nums[i]] for each 0 <= i < nums.length and return it.
A zero-based permutation nums is an array of distinct integers from 0 to nums.length - 1 (inclusive).

Input: nums = [0,2,1,5,3,4]
Output: [0,1,2,4,5,3]
Explanation: The array ans is built as follows: 
ans = [nums[nums[0]], nums[nums[1]], nums[nums[2]], nums[nums[3]], nums[nums[4]], nums[nums[5]]]
    = [nums[0], nums[2], nums[1], nums[5], nums[3], nums[4]]
    = [0,1,2,4,5,3]                            
*/
                            
class Solution {
    public int[] buildArray(int[] nums) {
       // int n = nums.length;
        int[] ansAr = new int[nums.length];
        for(int i=0; i<nums.length; i++){
            ansAr[i] = nums[nums[i]];
        }
        return ansAr;
    } 
Input: nums = [0,2,1,5,3,4]
Output: [0,1,2,4,5,3]                           

                            
                            
/*
1572. Matrix Diagonal Sum
Easy
1.8K
25
Companies
Given a square matrix mat, return the sum of the matrix diagonals.
Only include the sum of all the elements on the primary diagonal and all the elements on the secondary diagonal that are not part of the primary diagonal.

Input: mat = [[1,2,3],
              [4,5,6],
              [7,8,9]]
Output: 25
Explanation: Diagonals sum: 1 + 5 + 9 + 3 + 7 = 25
Notice that element mat[1][1] = 5 is counted only once.
*/
                            
class Solution {
    public int diagonalSum(int[][] mat) {
       int sum = 0;
       for(int i=0; i<mat.length; i++){
           sum += mat[i][i];
           if(i != mat.length - i - 1){
               sum += mat[i][mat.length - i - 1];
           }
       }
       return sum;
    }
}  
Input: mat = [[1,2,3],
              [4,5,6],
              [7,8,9]]
Output: 25                            



/*
implementing mergeSort
input:  4
        8 5 6 90
output: 5 6 8 90 
*/


import java.util.*;
public class mer{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        mergeSort(arr, 0, arr.length - 1);
        for(int i=0; i<n; i++){
            System.out.print(arr[i] + " ");
        }
    }
    public static void mergeSort(int[] arr, int left, int right){
        if(left >= right){
            return;
        }
        int mid = left + (right - left)/2;
        mergeSort(arr, left, mid);
        mergeSort(arr, mid + 1, right);
        mergeArray(arr, left, mid, right);
    }
    public static void mergeArray(int[] arr, int left, int mid, int right){
        int p1 = left;
        int p2 = mid + 1;
        int[] ansArr = new int[right - left + 1];
        int iter = 0;
        
        while(p1 <= mid && p2 <= right){
            if(arr[p1] < arr[p2]){
                ansArr[iter] = arr[p1];
                iter++;
                p1++;
            }else {
                ansArr[iter] = arr[p2];
                iter++;
                p2++;
            }
        }
        while(p1 <= mid){
            ansArr[iter] = arr[p1];
            iter++;
            p1++;
        }
        while(p2 <= right){
            ansArr[iter] = arr[p2];
            iter++;
            p2++;
        }
        for(int i=left; i<= right; i++){
        arr[i] = ansArr[i - left];
      }
   }
}
input:  4
        8 5 6 90
output: 5 6 8 90 

                            
                            
/*
35. Search Insert Position
Easy
Given a sorted array of distinct integers and a target value, return the index if the target is found. If not, return the index where it would be if it were inserted in order.
You must write an algorithm with O(log n) runtime complexity.
Example 1:
Input: nums = [1,3,5,6], target = 5
Output: 2                            
*/                            
                            
                                                        
class Solution {
    public int searchInsert(int[] nums, int target) {
        int left = 0;
        int right = nums.length- 1;
        while(left <= right){
            int mid = left + (right - left)/2;

        if(nums[mid] == target){
            return mid;
        }else if(nums[mid] > target){
            right = mid - 1;
        }else {
            left = mid + 1;
        }
        
    }
    return left;
   }
}           
Input: nums = [1,3,5,6], target = 5
Output: 2                             



/* 
implementing the buble sort 
*/



import java.util.*;
public class jg{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        for(int i=0; i<n; i++){
            bub(arr);
            System.out.print(arr[i] + " ");
        }
    }
    public static void bub(int[] arr){
        for(int i=0; i<arr.length; i++){
            for(int j=0; j<arr.length - 1 - i; j++){
                if(arr[j] > arr[j + 1]){
                    int temp = arr[j];
                    arr[j]  = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }
    }
}
input : 3 
3 1 2
output : 1 2 3 



/*
implement insert sort
*/



import java.util.*;
public class kldf{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        for(int i=0; i<n; i++){
            insertSort(arr);
            System.out.print(arr[i] + " ");
        }
    }
    public static void insertSort(int[] arr){
        for(int i=0; i<arr.len; i++){
            for(int j=i; j>=1; j--){
                if(arr[j] < arr[j- 1]){
                    int temp = arr[j];
                    arr[j] = arr[j - 1];
                    arr[j - 1] = temp;
                }
            }
        }
    }
}
input : 
4 
9 3 5 6
output :
3 5 6 9 


/*
implement the selection Sort
*/


import java.util.*;
public class skdf{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        for(int i=0; i<n; i++){
            selectionSort(arr);
            System.out.print(arr[i] + " ");
        }
    }
    public static void selectionSort(int[] arr){
        for(int i=0; i<arr.length; i++){
            int lowest = i;
            for(int j=0; j<arr.length; j++){
                if(arr[j] > arr[lowest]){
                    lowest = j;
                }
            }
            int temp = arr[lowest];
            arr[lowest] = arr[i];
            arr[i] = temp;
        }
    }
}
input :
4 
9 3 5 6
input :
3 6 5 9 





/*
Given an array of N integers, give the number with maximum frequency. If multiple numbers have maximum frequency print the maximum number among them
*/


import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static void main (String[] args) {
        Scanner maxFre = new Scanner(System.in);
        int N = maxFre.nextInt();
        int[] arr = new int[N];
        int[] arr1 = new int[10000];
        int maxcount = 0;
        int maxFreEle = 0;

        for(int i=0; i<N; i++){
            arr[i] = maxFre.nextInt();
        }
        for(int i=0; i<N; i++){
           /* max =*/ arr1[arr[i]]++;           
        }

        for(int i=0; i<arr1.length; i++){

            if(arr1[i] > maxcount && arr1[i] > arr[i]){
                maxcount = arr1[i];
                maxFreEle = i;

                System.out.print(maxFreEle);
            }
        }
    }
}

    
    
    
    
    
    
    
/*    
Maximum and Minimum in an Array
*/
    
    
import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework

// don't change the name of this class
// you can add inner classes if needed
class Main {
    public static void main (String[] args) {
        Scanner eleme = new Scanner(System.in);
        int T = eleme.nextInt();
        int N = eleme.nextInt();
        int[] arr = new int[N];
        int max = 0;
        int min = 0;

        while(T-- > 0){

            for(int i=0; i<N; i++){
            arr[i] = eleme.nextInt();
            // int ans = fidMax()
        }

      //  int max = 0;
//public static int fidMax(int[] arr, int N){
    for(int i=0; i<N; i++){
      max = arr[0];
      if(arr[i] > max){
        max = arr[i];
      }
          // int  max = arr[0];
          //   max = Math.max(max, arr[i]);
          //  if(arr[i] >= max){
               // max = arr[i];
          //  }   

        }
        // return max;

}
public static int fidMin(int[] arr, int N) {
      //int min = 0;
        for(int i=1; i<N; i++){
          int   min = arr[0];
            min = Math.min(min, arr[i]);
               //min = arr[i];
           // }
        }
        return min;

}
       
            // System.out.print(max);
            // System.out.print(min);        
        }
    }
}    



/*
taking input from ArrayList 
*/


import java.util.*;
import java.util.ArrayList;
public class df{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        ArrayList<Integer> al = new ArrayList<>(n);
        
        for(int i=0; i<n; i++){
           al.add(in.nextInt());
        }
         System.out.print(al);
    }
}
input:
3
1 3 4
output:
[1, 3, 4]

                                                 
                                                 
/*
insert an integer at given position
*/                                                 
                                                 
import java.util.*;
import java.util.ArrayList;
public class dfk{
    public static void main(String args[]){
        
        ArrayList<Integer> al = new ArrayList<>();
        
        al.add(2);
        al.add(3);
        al.add(4);
        al.add(0, 1);
        
        System.out.print(al);
    }
}                                                
output :
[1, 2, 3, 4]    
    


    
/*
insert an integer in an given any number of array
*/    
    
import java.util.*;
import java.util.ArrayList;
public class dk{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        ArrayList<Integer> al = new ArrayList<>();
        for(int i=0; i<n; i++){
            al.add(in.nextInt());
        }
        al.add(1,3);
        System.out.print(al);
    }
}    
input :
5
1 3 4 5 6                                                 
output:
[1, 3, 3, 4, 5, 6]
                                                 
                                                 
                                                 
/*
insert an given element at any given position in an array given by the user
*/
                                                 
                                                 
                                                 
import java.util.*;
import java.util.ArrayList;
public class kd{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int a = in.nextInt();
        int nu = in.nextInt();
        
        ArrayList<Integer> al = new ArrayList<>();
        for(int i=0; i<n; i++){
            al.add(in.nextInt());
        }
        al.add(a,nu);
        System.out.print(al);
    }
} 
input :                                                 
5 0 9
1 3 4 5 6                                                 
output :                                                 
[9, 1, 3, 4, 5, 6]                                                 
                                                 

                                                 
                                                 
/*
            fill an array list, sum of all the integers inside it ...
            Input = : [12,45,78,90,1]
            output: sum of above no...
     */                                                 
                                                 
import java.util.*;
import java.util.ArrayList;
public class dj{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        
        ArrayList<Integer> al = new ArrayList<>();
        
        for(int i=0; i<n; i++){
            al.add(in.nextInt());
            
        }
        int ans = sumOfInt(al);
        System.out.print(ans);
    }
    public static int sumOfInt(ArrayList<Integer> al){
        int sum =0; 
            for(int i=0; i<al.size(); i++){
                sum += al.get(i);
            }
            return sum;
    }
}                 
input :
5
1 2 3 4 5
output :
15                                      
                                      
  
/*
print fizzbuzz if integer is divisible by 3 nd 5 print fizz if it is divisible by 3 only                                      
print buzz if it is divisible by 5 only else print the interger                                      
*/                                      
                                      
import java.util.*;
public class dk{
    public static void main(String args[]){
        int n = 15;
        
        for(int i=1; i<=n; i++){
            if(i % 3 == 0 && i % 5 == 0){
                System.out.println("fizzbuzz");
            }else if(i % 3 == 0){
                 System.out.println("fizz");
            }else if(i % 5 == 0){
                 System.out.println("buzz");
            }else {
                System.out.println(i);
            }
        }
    }
}                                      
input :
3 
ouput :    
1 2 fizz    


/*
implement quick sort
*/



import java.util.*;
public class dk{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        quickSort(arr, 0, arr.length - 1);
        for(int i=0; i<n; i++){
            System.out.print(arr[i]+ " ");
        }
    }
    public static int partision(int[] arr, int low, int high){
        int pivot = arr[high];
        int i = low - 1;
        for(int j=low; j<high; j++){
            if(arr[j] < pivot){
                i++;
                int temp = arr[i];
                 arr[i] = arr[j];
                 arr[j] = temp;
            }
        }
        int temp = arr[i + 1];
        arr[i + 1] = arr[high];
        arr[high] = temp;
        
        return i + 1;
    }
    public static void quickSort(int[] arr,int low, int high){
        if(low > high){
            return;
        }
        int pi = partision(arr, low, high);
        quickSort(arr, low, pi - 1);
        quickSort(arr, pi + 1, high);
    }
}
input :
9
1 5 6 90 3 8 2 70 64
ouput :
1 2 3 5 6 8 64 70 90 




/*
You are given two integer arrays nums1 and nums2, sorted in non-decreasing order, and two integers m and n, representing the number of elements in nums1 and nums2 respectively.

Merge nums1 and nums2 into a single array sorted in non-decreasing order.

The final sorted array should not be returned by the function, but instead be stored inside the array nums1. To accommodate this, nums1 has a length of m + n, where the first m elements denote the elements that should be merged, and the last n elements are set to 0 and should be ignored. nums2 has a length of n.

 

Example 1:

Input: nums1 = [1,2,3,0,0,0], m = 3, nums2 = [2,5,6], n = 3
Output: [1,2,2,3,5,6]
Explanation: The arrays we are merging are [1,2,3] and [2,5,6].
The result of the merge is [1,2,2,3,5,6] with the underlined elements coming from nums1.
*/

class Solution {
    public void merge(int[] nums1, int m, int[] nums2, int n) {
        int i =m-1;
        int j= n - 1;
        int emptyArr = nums1.length - 1;
        
        while(j>= 0){
            if(i>= 0 && nums1[i] > nums2[j]){
                nums1[emptyArr] = nums1[i];
                emptyArr--;
                i--;
            }else {
                nums1[emptyArr] = nums2[j];
                emptyArr--;
                j--;
            }
        }
    }
}
Input: nums1 = [1,2,3,0,0,0], m = 3, nums2 = [2,5,6], n = 3
Output: [1,2,2,3,5,6]

    
    
    
    
/*
Given a non-empty array of integers nums, every element appears twice except for one. Find that single one.

You must implement a solution with a linear runtime complexity and use only constant extra space.

 

Example 1:

Input: nums = [2,2,1]
Output: 1
*/
    
    
class Solution {
    public int singleNumber(int[] nums) {
    Arrays.sort(nums);
    for(int i=0; i<nums.length - 1; i++){
        if(nums[i] != nums[i + 1]){
            return nums[i];
        }
        i++;
    }
    return nums[nums.length - 1];
    }
}
Input: nums = [2,2,1]
Output: 1                               
    



print dkd if a number is divisible by both 3 nd 5 
nd print dk if it is divisible by 3 nd dd for 5


import java.util.*;
public class dk{
    public static void main(String args[]){
        int n= 20;
        
        for(int i=0; i<n; i++){
            if(i % 3 == 0 && i % 5 == 0){
                System.out.println("dkd");
            }else if(i % 3 == 0){
                  System.out.println("dd");
            }else if( i % 5 == 0){
                System.out.println("dk");
            }else {
                System.out.println(i);
            }
        }
    }
}



/*
insert the index of a missing number
input :
4 4
1 3 5 6
output :
2
*/



import java.util.*;
public class op{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int target = in.nextInt();
        int[] arr = new int[n];
        
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
            
        }
        int ans = searchInsert(arr, target);
        System.out.print(ans);
    }
    public static int searchInsert(int[] arr, int target){
        int left = 0;
        int right = arr.length - 1;
        
        while(left <= right){
            int mid = left + (right - left)/ 2;
            
            if(arr[mid] == target){
                return mid;
            }else if(arr[mid] > target){
                right = mid - 1;
            }else {
                left = mid + 1;
            }
        }
         return left;
    }
}
input :
4 4
1 3 5 6
output :
2

    
    
    
/*
153. Find Minimum in Rotated Sorted Array
Medium
    
Suppose an array of length n sorted in ascending order is rotated between 1 and n times. For example, the array nums = [0,1,2,4,5,6,7] might become:

[4,5,6,7,0,1,2] if it was rotated 4 times.
[0,1,2,4,5,6,7] if it was rotated 7 times.
Notice that rotating an array [a[0], a[1], a[2], ..., a[n-1]] 1 time results in the array [a[n-1], a[0], a[1], a[2], ..., a[n-2]].

Given the sorted rotated array nums of unique elements, return the minimum element of this array.

You must write an algorithm that runs in O(log n) time.

 

Example 1:

Input: nums = [3,4,5,1,2]
Output: 1
Explanation: The original array was [1,2,3,4,5] rotated 3 times.    
*/    
    
    
import java.util.*;
public class op{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
            
        }
        int ans = findMin(arr);
        System.out.print(ans);
    }
    public static int findMin(int[] nums) {
        int left = 0;                   // left = 0
        int right = nums.length - 1;    // right = 4 - 1 = 3
        
        while(left < right){            // 0 < 0 ? F
            int mid = left + (right - left)/2;  // mid = 0 + (1 - 0)/ 2 --> 1/2 --> 0 

            if(nums[mid] > nums[right]){       // nums[mid] --> nums[0] --> 1 > nums[right] --> nums[1] --> 3 ? F
                left = mid + 1;                // 
            }else {
                right = mid;                  // right = 0
            }
        }
        return nums[right];                  // nums[right] --> nums[0] --> 1
    }
}    
Input: nums = [3,4,5,1,2]
Output: 1    

    
    
/*
240. Search a 2D Matrix II
Medium
9.9K
165
Companies
Write an efficient algorithm that searches for a value target in an m x n integer matrix matrix. This matrix has the following properties:

Integers in each row are sorted in ascending from left to right.
Integers in each column are sorted in ascending from top to bottom.
 

Example 1:
1,4,7,11,15
2,5,8,12,19
3,6,9,16,22
10,13,14,17,24
18,21,23,26,30    
Input: matrix = [[1,4,7,11,15],[2,5,8,12,19],[3,6,9,16,22],[10,13,14,17,24],[18,21,23,26,30]], target = 5
Output: true    
    
    
public Class Solution {
    public static int searchMatrix(int[] matrix, int target){
        int row = 0;
        int col = matrix[0].length- 1;
        
        while(row < matrix.length && col >= 0){
            int item = matrix[row][col];
            
            if(item == target){
                return true;
            }
            if(item > target){
                col--;
            }else {
                row++;
            }
        }
        return false;
    }
}    
Input: matrix = [[1,4,7,11,15],[2,5,8,12,19],[3,6,9,16,22],[10,13,14,17,24],[18,21,23,26,30]], target = 5
Output: true     
    

    
    
/*
segrigate one nd zero 
input :
5
1 0 1 0 0
output :
0 0 0 1 1 
*/    
    
import java.util.*;
public class fj{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        oneS(arr);
        for(int i=0; i<n; i++){
            System.out.print(arr[i] + " ");
        }
    }
    public static void oneS(int[] arr){
        int left = 0;
        int right = arr.length - 1;
        
        while(left < right){
            
            while(left < arr.length && arr[left] == 0){
                left++;
            }
            while(right >= 0 && arr[right] == 1){
                right--;
            }
            if(left < right){
                arr[left] = 0;
                arr[right] = 1;
                left++;
                right--;
            }
        }
    }
}    
input :
5
1 0 1 0 0
output :
0 0 0 1 1     
    


/*
create Create LinkedList in Java (add).

import java.util.LinkedList;
public class Main {
    public static void main(String args[]){
        
        LinkedList<String> animals = new LinkedList<>();
        LinkedList<Integer> lifeSpan = new LinkedList<>();
        
        animals.add("dog");
        lifeSpan.add(20);
        animals.add("cat");
        lifeSpan.add(15);
        
        System.out.println("name Of Animal --" + animals);
        System.out.println("its lifeSpan--" + lifeSpan);
    }
}
ouput :
name Of Animal --[dog, cat]
its lifeSpan--[20, 15]




/*
876. Middle of the Linked List
Easy
8.6K
249
Companies
Given the head of a singly linked list, return the middle node of the linked list.

If there are two middle nodes, return the second middle node.

 

Example 1:


Input: head = [1,2,3,4,5]
Output: [3,4,5]
Explanation: The middle node of the list is node 3.
*/

/**
 * Definition for singly-linked list.
 * public class ListNode {
 *     int val;
 *     ListNode next;
 *     ListNode() {}
 *     ListNode(int val) { this.val = val; }
 *     ListNode(int val, ListNode next) { this.val = val; this.next = next; }
 * }
 */
class Solution {
    public ListNode middleNode(ListNode head) {
        ListNode fastPointer = head;
        ListNode slowPointer = head;

        while(fastPointer != null && fastPointer.next != null){
            fastPointer = fastPointer.next.next;
            slowPointer = slowPointer.next;
        }
        return slowPointer;
    }
}



/*
implementing mergeSort (redone)
input:  4
        8 5 6 90
output: 5 6 8 90 
*/


import java.util.*;
public class mer{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        mergeSort(arr, 0, arr.length - 1);
        for(int i=0; i<n; i++){
            System.out.print(arr[i] + " ");
        }
    }
    public static void mergeSort(int[] arr, int left, int right){
        if(left >= right){
            return;
        }
        int mid = left + (right - left)/2;
        mergeSort(arr, left, mid);
        mergeSort(arr, mid + 1, right);
        mergeArray(arr, left, mid, right);
    }
    public static void mergeArray(int[] arr, int left, int mid, int right){
        int p1 = left;
        int p2 = mid + 1;
        int[] ansArr = new int[right - left + 1];
        int iter = 0;
        
        while(p1 <= mid && p2 <= right){
            if(arr[p1] < arr[p2]){
                ansArr[iter] = arr[p1];
                iter++;
                p1++;
            }else {
                ansArr[iter] = arr[p2];
                iter++;
                p2++;
            }
        }
        while(p1 <= mid){
            ansArr[iter] = arr[p1];
            iter++;
            p1++;
        }
        while(p2 <= right){
            ansArr[iter] = arr[p2];
            iter++;
            p2++;
        }
        for(int i=left; i<= right; i++){
        arr[i] = ansArr[i - left];
      }
   }
}
input:  4
        8 5 6 90
output: 5 6 8 90 



/*
implement selection sort (redone)
*/

import java.util.*;
public class kd{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        for(int i=0; i<n; i++){
            selectionSort(arr);
            System.out.print(arr[i] + " ");
        }
    }
    public static void selectionSort(int[] arr){
        for(int i=0; i<arr.length; i++){
            int lowest = i;
            
            for(int j=i+ 1; j<arr.length; j++){
                if(arr[j] < arr[lowest]){
                    lowest = j;
                }
            }
            int temp = arr[lowest];
            arr[lowest] = arr[i];
            arr[i] = temp;
        }
    }
}
input :
4
4 3 5 1
output :
1 3 4 5

                                         
/*
implement bubleSort (redone)
*/                                         
                                                                            
import java.util.*;
public class kd{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
       
            for(int i=0; i<n; i++){
                bubleSort(arr);
                System.out.print(arr[i] + " ");
        }
    }
    public static void bubleSort(int[] arr){
        for(int i=0; i<arr.length; i++){
            for(int j=0; j<arr.length - 1 - i; j++){
                if(arr[j] > arr[j + 1]){
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }
    }
}      
input :    
4
4 3 5 1    
output :    
1 3 4 5     

    
/*
implement insertSort (redo)
*/    
import java.util.*;
public class kd{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        for(int i=0; i<n; i++){
            insertSort(arr);
            System.out.print(arr[i] + " ");
        }
    }
    public static void insertSort(int[] arr){
        for(int i=0; i<arr.length; i++){
            for(int j=i; j>=1; j--){
                if(arr[j] < arr[j - 1]){
                    int temp = arr[j];
                    arr[j] = arr[j - 1];
                    arr[j - 1] = temp;
                }
            }
        }
    }
}   
input : 
4
4 3 5 1                                 
output :    
1 3 4 5     
    
    

/*
implement quickSort(redone)                                 
*/                                 
    
import java.util.*;
public class dk{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        qui(arr, 0, arr.length - 1);
        for(int i=0; i<n; i++){
            System.out.print(arr[i] + " ");
        }
    }
    public static int part(int[] arr, int low, int high){
        int piv = arr[high];
        int i = low - 1;
        for(int j=low; j<high; j++){
            if(arr[j] < piv){
                i++;
                int temp = arr[i];
                arr[i] = arr[j];
                arr[j] = temp;
            }
        }
        int temp = arr[i + 1];
        arr[i + 1] = arr[high];
        arr[high] = temp;
        
        return i + 1;
    }
    public static void qui(int[] arr, int low, int high){
        if(low > high){
            return;
        }
        int pi = part(arr, low, high);
        qui(arr, low, pi - 1);
        qui(arr, pi + 1, high);
    }
}
input : 
4
4 3 5 1    
output :
1 3 4 5     
    




/*
check if given string is angram or not (redone)
*/


import java.util.*;
public class jdf{
    public static void main(String args[]){
      //  Scanner fre = new Scanner(System.in);
        int[] arr = new int[26];
        
        String str = "dad";
        String str1 = "min";
        
        for(int i=0; i<str.length(); i++){
            char c = str.charAt(i);
            int index = (int)(c - 'a');
            arr[index]++;
        }
        
        for(int i=0; i<str1.length(); i++){
            char c = str1.charAt(i);
            int index = (int)(c - 'a');
            arr[index]--;
        }
        boolean ana = true;
        for(int i=0; i<arr.length; i++){
            if(arr[i] != 0){
                ana = false;
            }
        }
        if(ana == true){
            System.out.print("YES");
        }else {
            System.out.print("NO");
        }
     
    }
}
input : "dfjk" "dfjk"
output:
YES





/*
print fizzbuzz if integer is divisible by 3 nd 5 print fizz if it is divisible by 3 only                                      
print buzz if it is divisible by 5 only else print the interger  in arraylist using arrray                                  
*/ 

import java.util.*;
import java.util.ArrayList;
public class kd{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        
        ArrayList<Integer> list = new ArrayList<>();
        
        for(int i=0; i<n; i++){
            list.add(in.nextInt());
        }
        for(int i=0; i<n; i++){
            if(list.get(i) % 3 == 0 && list.get(i) % 5 == 0){
                System.out.println("fizzBuzz");
            }else if(list.get(i) % 3 == 0){
                System.out.println("Fizzz");
            }else if(list.get(i) % 5 == 0){
                System.out.println("Buzz");
            }else{
                System.out.println(list.get(i));
            }
        }
    }
}
input: 
3 
15 5 3
output :
fizzBuzz
Buzz
Fizzz

    
    
    
/*
    Given an array of N elements, your task is to find the count of repeated elements. Print the repeated elements in ascending order along with their frequency.
Have a look at the example for more understanding.(redone)
*/    
    
 import java.util.*;
public class kd{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        int[] arr1 = new int[100000];
        
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        for(int i=0; i<n; i++){
            arr1[arr[i]]++;
        }
        for(int i=0; i<arr1.length; i++){
            if(arr1[i] > 0){
                System.out.println(i + " " + arr1[i]);
            }
        }
    }
}
input:
5
15 15 3 4 4    
output:    
3 1
4 2
15 2    

    
/*
Given a binary array of size N. Count number of 1's and 0's in the array.(updated, redone)                                  
*/    

import java.util.*;
public class dk{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
            int n  = in.nextInt();
            int[] arr = new int[n];
            for(int i=0; i<n; i++){
                arr[i] = in.nextInt();
            }
            int onsCount = 0;
            for(int i=0; i<n; i++){
                if(arr[i] == 1){
                    onsCount++;
                }
            }
            int zeroCount = 0;
            for(int i=0; i<n; i++){
                if(arr[i] == 0){
                    zeroCount++;
                }
            }
            System.out.print(onsCount + " " + zeroCount);
        }
}    
input :
5
0 1 1 0 1                              
output :    
3 2                              



/*
inset target at the correct postion nd returnt the index
*/


import java.util.*;
public class dk{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int target = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
       int ans =  sear(arr, target);
        System.out.print(ans);
    }
    public static int sear(int[] arr, int target){
        int left = 0;
        int right = arr.length - 1;
        
        while(left <= right){
            int mid = left + (right - left)/ 2;
            
            if(arr[mid] == target){
                return mid;
            }else if(arr[mid] > target){
                right = mid - 1;
            }else {
                left = mid + 1;
            }
        }
         return left;
    }
}
input :
3 1
1 4 5
output :
0



    /*
        Question: Frequency of items inside the array
        Input: [1,2,3,5,1,2,5,6,1,1,2]
        Output:
     */
     
import java.util.*;
import java.util.HashMap;
public class kd{
    public static void main(String args[]){
        HashMap<Integer, Integer> map = new HashMap();
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        for(int i=0; i<n; i++){
            int key = arr[i];
            
            if(!map.containsKey(key)){  // what it ask is that if there is an element which already exists in the 
                map.put(key, 1);         // list or not if NO then execuete the if condition else do the else condition
            }else {
                int oldVal = map.get(key);
                    map.put(key, oldVal + 1);
                }
        }
        System.out.print(map);
    }
}
input :
11
1 2 3 5 1 2 5 6 1 1 2
output :
{1=4, 2=3, 3=1, 5=2, 6=1}

    

    
  /*
        Question: Frequency of items inside the array(shroter method )
        Input: [1,2,3,5,1,2,5,6,1,1,2]
        Output:
     */    
    
    
import java.util.*;
import java.util.HashMap;
public class kd{
    public static void main(String args[]){
    HashMap<Integer, Integer> map = new HashMap();
    Scanner in = new Scanner(System.in);
    int n = in.nextInt();
    int[] arr = new int[n];
    for(int i=0; i<n; i++){
        arr[i] = in.nextInt();
    }
    for(int i=0; i<n; i++){
        int key = arr[i];
        
     map.put(key, map.getOrDefault(key, 0)+ 1);
    }
    System.out.print(map);
    
   }
}    
input :
11
1 2 3 5 1 2 5 6 1 1 2
output :
{1=4, 2=3, 3=1, 5=2, 6=1}
    

    
  /*
           Question: Find out the duplicate in list
           Input: [1,2,3,4,5,6,89,90,3,12,15,17,1000,123];
           Output: 3
     */    
    
    
    
 import java.util.*;
import java.util.HashSet;
public class dk{
    public static void main(String args[]){
        HashSet set = new HashSet();
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
        for(int i=0; i<n; i++){
            if(set.contains(arr[i])){
                System.out.println(arr[i] + " ");
            }else if(!set.contains(arr[i])){
                set.add(arr[i]);
            }else {
                 System.out.println("-1");
            }
        }
       
    }
}   
Input: [1,2,3,4,5,6,89,90,3,12,15,17,1000,123];
Output: 3    




/*
taking input from ArrayList (redone)
*/


import java.util.*;
import java.util.ArrayList;
public class df{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        ArrayList<Integer> al = new ArrayList<>(n);
        
        for(int i=0; i<n; i++){
           al.add(in.nextInt());
        }
         System.out.print(al);
    }
}
input:
3
1 3 4
output:
[1, 3, 4]



/*
inset target at the correct postion nd returnt the index
*/


import java.util.*;
public class dk{
    public static void main(String args[]){
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();
        int target = in.nextInt();
        int[] arr = new int[n];
        for(int i=0; i<n; i++){
            arr[i] = in.nextInt();
        }
       int ans =  sear(arr, target);
        System.out.print(ans);
    }
    public static int sear(int[] arr, int target){
        int left = 0;
        int right = arr.length - 1;
        
        while(left <= right){
            int mid = left + (right - left)/ 2;
            
            if(arr[mid] == target){
                return mid;
            }else if(arr[mid] > target){
                right = mid - 1;
            }else {
                left = mid + 1;
            }
        }
         return left;
    }
}
input :
3 1
1 4 5
output :
0




/* 1. Two Sum(redone)
Easy
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.
You can return the answer in any order.

Example 1:
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].
*/

class Solution {
    public int[] twoSum(int[] nums, int target) {
        for(int i=0; i<nums.length; i++){
            for(int j=i+1; j<nums.length; j++){
                if(nums[i] + nums[j] == target){
                    return new int[] {i,j};
                }
            }
        }
        return new int[] {};
    }
}

    
    
/*
1920. Build Array from Permutation(redone)
Easy
Given a zero-based permutation nums (0-indexed), build an array ans of the same length where ans[i] = nums[nums[i]] for each 0 <= i < nums.length and return it.
A zero-based permutation nums is an array of distinct integers from 0 to nums.length - 1 (inclusive).

Example 1:

Input: nums = [1,2,0]
Output: [2,0,1]
Explanation: The array ans is built as follows: 
1 2 0 
ans = (i = 0; i < 3; i++)
nums[nums[i]] =            
nums[nums[0]] , nums[nums[1]], nums[nums[2]]
nums[1], nums[2], nums[0]
2 0 1 
                    
class Solution {
    public int[] buildArray(int[] nums) {
        int[] ansArr = new int[nums.length];
        for(int i=0; i<nums.length; i++){
            ansArr[i] = nums[nums[i]];
        }
        return ansArr;
    }
}                    

    
    
/*
1572. Matrix Diagonal Sum (redone, Time taken: 26 m 40 s)
Easy
Given a square matrix mat, return the sum of the matrix diagonals.
Only include the sum of all the elements on the primary diagonal and all the elements on the secondary diagonal that are not part of the primary diagonal.
    
Example 1:

Input: mat = [[1,2,3],
              [4,5,6],
              [7,8,9]]
Output: 25
Explanation: Diagonals sum: 1 + 5 + 9 + 3 + 7 = 25
Notice that element mat[1][1] = 5 is counted only once.    
*/    
    
class Solution {
    public int diagonalSum(int[][] mat) {
        int sum = 0;
        int n = mat.length;
        for(int i=0; i<mat.length; i++){
            sum += mat[i][i] + mat[i][n - i - 1];
        }
        return n%2 == 0 ? sum : sum - mat[n/2][n/2];
    }
}    
    
    

                                   
/*
35. Search Insert Position(redone,Time taken: 8m53s)
Easy
Given a sorted array of distinct integers and a target value, return the index if the target is found. If not, return the index where it would be if it were inserted in order.
You must write an algorithm with O(log n) runtime complexity.

Example 1:
Input: nums = [1,3,5,6], target = 5
Output: 2                                   
*/      

class Solution {
    public int searchInsert(int[] nums, int target) {
        int left = 0;
        int right = nums.length - 1;

        while(left <= right){

            int mid = left + (right - left)/2;

            if(nums[mid] == target){
                return mid;
            }else if(nums[mid] < target){
                left = mid + 1;
            }else {
                right = mid - 1;
            }
        }
        return left;
   }
}                                   




/*
27. Remove Element(redone,Time taken: 14m )
Easy
Given an integer array nums and an integer val, remove all occurrences of val in nums in-place. The relative order of the elements may be changed.
Since it is impossible to change the length of the array in some languages, you must instead have the result be placed in the first part of the array nums. More formally, if there are k elements after removing the duplicates, then the first k elements of nums should hold the final result. It does not matter what you leave beyond the first k elements.
Return k after placing the final result in the first k slots of nums.
Do not allocate extra space for another array. You must do this by modifying the input array in-place with O(1) extra memory.

Example 1:
Input: nums = [3,2,2,3], val = 3
Output: 2, nums = [2,2,_,_]
Explanation: Your function should return k = 2, with the first two elements of nums being 2.
It does not matter what you leave beyond the returned k (hence they are underscores).

class Solution {
    public int removeElement(int[] nums, int val) {
        int ans = 0;
        for(int i=0; i<nums.length; i++){
            if(nums[i] != val){
                int temp = nums[ans];
                nums[ans] = nums[i];
                nums[i] = temp;
                ans++;
            }
        }
        return ans;
    }
}

    
    
    
/*
153. Find Minimum in Rotated Sorted Array(redone,Time taken: 16 m 57 s) 
Medium
Suppose an array of length n sorted in ascending order is rotated between 1 and n times. For example, the array nums = [0,1,2,4,5,6,7] might become:
[4,5,6,7,0,1,2] if it was rotated 4 times.
[0,1,2,4,5,6,7] if it was rotated 7 times.
Notice that rotating an array [a[0], a[1], a[2], ..., a[n-1]] 1 time results in the array [a[n-1], a[0], a[1], a[2], ..., a[n-2]].
Given the sorted rotated array nums of unique elements, return the minimum element of this array.
You must write an algorithm that runs in O(log n) time.
    
Example 1:
Input: nums = [3,4,5,1,2]
Output: 1
Explanation: The original array was [1,2,3,4,5] rotated 3 times.

    
class Solution {
    public int findMin(int[] nums) {
        int left = 0;
        int right = nums.length - 1;

        while(left < right){

            int mid = left + (right - left)/2;
            
            if(nums[mid] > nums[right]){
                left = mid + 1;
            }else {
                right = mid;
            }
        }
        return nums[right];
    }
}    
    
    


/*
136. Single Number(redone, Time taken: 7 m 22 s)
Easy
Given a non-empty array of integers nums, every element appears twice except for one. Find that single one.
You must implement a solution with a linear runtime complexity and use only constant extra space.

Example 1:
Input: nums = [2,2,1]
Output: 1


class Solution {
    public int singleNumber(int[] nums) {
        Arrays.sort(nums);
        int ans = 0;
        for(int i=0; i<nums.length - 1; i++){
            if(nums[i] != nums[i+1]){
                return nums[i];
            }
            i++;
        }
        return nums[nums.length - 1];
    }
}

/*
169. Majority Element(Time taken: 16 m 54 s)
Easy
Given an array nums of size n, return the majority element.
The majority element is the element that appears more than ⌊n / 2⌋ times. You may assume that the majority element always exists in the array.

Example 1:
Input: nums = [3,2,3]
Output: 3
*/

class Solution {
    public int majorityElement(int[] nums) {
        int cnt = 0;
        int ans = 0;
        for(int i=0; i<nums.length; i++){ // i = 1
            if(cnt == 0){
                ans = nums[i]; // ans = nums[i] = 2 --> ans = 2
            }
            if(nums[i] == ans){
                cnt += 1;
            }else {
                cnt -= 1;
            }
        }
        return ans;
    }
}

    
    
    
/*
217. Contains Duplicate(Time taken: 19 m 54 s)
Easy
Given an integer array nums, return true if any value appears at least twice in the array, and return false if every element is distinct.
    
Example 1:
Input: nums = [1,2,3,1]
Output: true

    
class Solution {
    public boolean containsDuplicate(int[] nums) {
        Arrays.sort(nums);
        for(int i=0; i<nums.length - 1; i++){
            if(nums[i] == nums[i+ 1]){
                return true;
            }
        }
        return false;
    }
}    
