import java.util.Scanner;
public class ex2_2 
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.print("Enter a size of a array :");
		int size = sc.nextInt();
		int[] arr = new int[size];
		for(int i = 0; i < size;i++) {
			System.out.printf("enter a array value %d : ",i+1);
			int value = sc.nextInt();
			arr[i] = value;
		}
		System.out.print("Enter a number : ");
		int number = sc.nextInt();
		int count = 0;
		System.out.print("Numbers are = ");
		for(int i = 0; i < arr.length;i++) {
			if(number > arr[i]) {
				count+= 1;
				System.out.print(arr[i] + " ");
			}
		}
		System.out.println("\nCount = "+count);
	}
}
