package pattern;

public class SquareHallow {

	public static void main(String[] args) {
		int r = 4;
		int c = 4;
		for(int i=0;i<4;i++) {
			for(int j=0;j<4;j++) {
				if(i==0 || i==r-1 || j==0 || j==c-1) 
					System.out.print("*");				
				else
					System.out.print(" ");
		}
			System.out.println(" ");

	}

}
}

Output: 
        **** 
        *  * 
        *  * 
        **** 

Method used:
            Decide the size of the square:
                  The variables r and c represent the number of rows and columns. Both are 4
            Use two for loops to go through each position in the square:
                  The outer loop (i) goes from the first row to the last row.
                  The inner loop (j) goes from the first column to the last column in each row.
            Check each position:
                  If the position is on the edge of the square (i.e., first row, last row, first column, last column), print a *.
                  Otherwise, print a space to make it look empty inside.
                  After finishing each row, the program moves to a new line using System.out.println();.
            Specify edges:
                  Top row: i == 0
                  Bottom row: i == r - 1
                  Left column: j == 0
                  Right column: j == c - 1
                  If any of these conditions are true for a position, it's part of the border → print *.


