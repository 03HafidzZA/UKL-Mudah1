import java.util.Scanner;

public class SoalMudah2 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Masukkan bilangan: ");
        int angka = input.nextInt();

        if (angka % 2 == 0) {
            System.out.println(angka + " adalah bilangan genap.");
        } else {
            System.out.println(angka + " adalah bilangan ganjil.");
        }
    }
}
Program ini menghitung biaya pengiriman berdasarkan berat, jarak, dan volume paket.
Jika volume paket lebih dari 100 cm³, maka akan dikenakan biaya tambahan sebesar Rp 50.000.
