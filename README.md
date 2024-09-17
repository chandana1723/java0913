# java0913
package csa0913;

public class composite {
	public static boolean iscomposite(int num) {
		if(num<=1) {
			return false;
		}
		for(int i=2;i<=Math.sqrt(num);i++) {
			if(num%i==0) {
				return true;
			}
		}
		return false;
		
	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int[] array= {1,2,3,4,5,6,7,8,9,10};
		System.out.println("composite numbers in the array:");
		for(int num : array) {
			if(iscomposite(num)) {
				System.out.println(num); 
				
			}
		}

	}

}
