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
??? Mohan wants the ticket at least on date A.
??? Shreya wants the ticket at most by date B.
??? Anuj wants the ticket atleast on date C.
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
The warden told him that those students whose roll no are divisible by 2 they will get PAPUM HOSTEL and if it odd then they will get LOHIT HOSTEL. If the student is girl, then she will get ???Upper Wing??? otherwise ???Lower Wing???.
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
     decreasinRecur(n -1);
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



/* Given an integer array arr[] of size N and an element X. The task is to find and print the indices of the given element if it is present in array if not then print ???Not found??? without quotes.

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
