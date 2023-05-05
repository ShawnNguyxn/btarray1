# btarray1
Tổng âm dương trong mảng
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Nhap chieu dai mang N= ");
        int n = scanner.nextInt();
        int[] a = new int[n];
        System.out.println("Cac gia tri trong mang la ");

        int countMinus = 0;
        int countPlus = 0;
        for (int i = 0; i < n; i++) {
            a[i] = scanner.nextInt();
            if (a[i] >= 0) {
                countPlus += a[i];
            } else {
                countMinus += a[i];
            }
        }
        System.out.println("Tong so duong trong mang la " + countPlus);
        System.out.println("Tong so am trong mang la " + countMinus);
    }
}
