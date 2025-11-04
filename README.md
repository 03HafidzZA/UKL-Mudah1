import java.util.Scanner;

public class SoalMudah1 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Masukkan berat paket (kg): ");
        double berat = input.nextDouble();

        System.out.print("Masukkan jarak tempuh (km): ");
        double jarak = input.nextDouble();

        System.out.print("Masukkan panjang paket (cm): ");
        double panjang = input.nextDouble();

        System.out.print("Masukkan lebar paket (cm): ");
        double lebar = input.nextDouble();

        System.out.print("Masukkan tinggi paket (cm): ");
        double tinggi = input.nextDouble();

        double volume = panjang * lebar * tinggi;
        double biayaPerKg;

        if (jarak <= 10) {
            biayaPerKg = 4250;
        } else {
            biayaPerKg = 6000;
        }

        double totalBiaya = berat * biayaPerKg;

        if (volume > 100) {
            totalBiaya += 50000;
        }

        System.out.println("\nVolume paket: " + volume + " cm^3");
        System.out.println("Total biaya pengiriman: Rp " + totalBiaya);
    }
}


Program ini menghitung biaya pengiriman berdasarkan berat, jarak, dan volume paket.
Jika volume paket lebih dari 100 cm³, maka akan dikenakan biaya tambahan sebesar Rp 50.000.
