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
QUES 2
import java.util.Scanner;

public class Multiples {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int[] arr = new int[10];
        int[] multiples = new int[10];
        int j = 0;

        System.out.println("Enter 10 numbers:");
        for (int i = 0; i < 10; i++) {
            arr[i] = sc.nextInt();
        }

        for (int i = 0; i < 10; i++) {
            if (arr[i] % 9 == 0 && arr[i] % 3 == 0) {
                multiples[j] = arr[i];
                j++;
            }
        }

        System.out.print("The numbers that are multiples of both 9 and 3: ");
        for (int i = 0; i < j; i++) {
            System.out.print(multiples[i]);
            if (i < j - 1)
                System.out.print(",");
        }
        sc.close();
    }
}

