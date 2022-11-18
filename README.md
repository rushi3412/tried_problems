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
