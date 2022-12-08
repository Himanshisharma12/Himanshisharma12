
import java.util.Scanner;

public class RemoveElement {
    public static void main(String[] args) {
        int size , loc , i;
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the Array Size : ");
        size = sc.nextInt();

        int arr[] = new int[size];
        System.out.println("Enter the Element of Array");
        for( i=0;i<size;i++){
            arr[i] = sc.nextInt();
        }
        System.out.println("Enter the Element Locaiotn You want to Remove ");
        loc = sc.nextInt();

        for(i=loc ;i<size-1;i++){
            arr[i] = arr[i+1];
        }
        size--;
        for(i=0;i<size;i++){
            System.out.print(arr[i] + " ");
        }
    }
}
