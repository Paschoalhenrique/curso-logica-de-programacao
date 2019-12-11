# curso-logica-de-programacao

import java.util.Scanner;

public class matriz1 {

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);

		int A = sc.nextInt();
		int N = sc.nextInt();
		
		int[][] mat = new int[A][N];
		
		for (int i=0; i<A; i++) {
			for (int j=0; j<N; j++) {
				mat[i][j] = sc.nextInt();
			}
		}
		
		System.out.println("VALORES NEGATIVOS:");
		for (int i=0; i<A; i++) {
			for (int j=0; j<N; j++) {
				if (mat[i][j] < 0) {
					System.out.println(mat[i][j]);
				}
			}
		}
		
		sc.close();
	}
}
