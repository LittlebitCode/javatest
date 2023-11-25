import java.util.Scanner;

public class barang {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int menu;

        do {
            System.out.println("Menu: ");
            System.out.println("1. Pinjam Barang");
            System.out.println("2. Kembalikan Barang");
            System.out.println("3. Keluar");
            System.out.print("Pilih menu: ");
            menu = input.nextInt();

            switch (menu) {
                case 1:
                    pinjamBarang(input);
                    break;
                case 2:
                    kembalikanBarang(input);
                    break;
                case 3:
                    System.out.println("Terima kasih telah menggunakan program ini.");
                    break;
                default:
                    System.out.println("Menu yang Anda pilih tidak valid.");
            }

            System.out.println();
        } while (menu != 3);

        input.close();
    }

    public static void pinjamBarang(Scanner input) {
        input.nextLine();
        System.out.print("Masukkan nama peminjam: ");
        String namaPeminjam = input.nextLine();
        System.out.print("Masukkan nama barang: ");
        String namaBarang = input.nextLine();
        System.out.print("Masukkan jumlah barang: ");
        int jumlahBarang = input.nextInt();

        System.out.println();
        System.out.println("Keterangan Peminjaman");
        System.out.println("=====================");
        System.out.println("Nama Peminjam: " + namaPeminjam);
        System.out.println("Nama Barang: " + namaBarang);
        System.out.println("Jumlah Barang: " + jumlahBarang);
    }

    public static void kembalikanBarang(Scanner input) {
        input.nextLine();
        System.out.print("Masukkan nama peminjam: ");
        String namaPeminjam = input.nextLine();
        System.out.print("Masukkan nama barang: ");
        String namaBarang = input.nextLine();
        System.out.print("Masukkan jumlah barang: ");
        int jumlahBarang = input.nextInt();
        System.out.print("Masukkan lama pinjam (dalam hitungan hari): ");
        int lamaPinjam = input.nextInt();

        int batasWaktu = 3;
        int dendaPerBarang = 100000;
        int jumlahHariKeterlambatan = lamaPinjam - batasWaktu;
        int totalDenda = 0;

        System.out.println();
        System.out.println("Keterangan Peminjaman");
        System.out.println("=====================");
        System.out.println("Nama Peminjam: " + namaPeminjam);
        System.out.println("Nama Barang: " + namaBarang);
        System.out.println("Jumlah Barang: " + jumlahBarang);

        if (jumlahHariKeterlambatan > 0) {
            totalDenda = (jumlahBarang * dendaPerBarang) * jumlahHariKeterlambatan;
            System.out.println("Denda per Barang per Hari: Rp " + dendaPerBarang);
            System.out.println("Jumlah Hari Keterlambatan: " + jumlahHariKeterlambatan);
            System.out.println("Total Denda: Rp " + totalDenda);
        } else {
            System.out.println("Barang dikembalikan tepat waktu.");
        }
    }
}
