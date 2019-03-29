package Permutation;

public class Permutation {
	
	public static void swap(int A[], int i, int j){
		if(A.length==0 || i<0 || j<0) return;
		
		int temp = A[i];
		A[i] = A[j];
		A[j] = temp;
	}
	
	public static void printAll(int A[], int n){
		for (int i=0; i<n; i++) {
			System.out.print(A[i] + " ");
		}
		System.out.println();
	}
	
	public static void perm(int A[], int p, int q){
		if(p == q){
			printAll(A, q+1);
		}else{
			int i;
			for(i=p; i<=q; i++){
				swap(A, p, i);
				perm(A, p+1, q);
				swap(A, p, i);
			}
		}
	}

	public static void main(String args[]){
		int A[] = {1, 2, 3, 4};
		perm(A, 0, A.length-1);
	}
}
