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




// simple transpose og matrix 
3
1 4 5
4 5 6
5 3 1


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



//Given a matrix of size M*N, your task is to find the maximum sum of a column.
Input

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
