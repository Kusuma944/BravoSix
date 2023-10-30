<<<<<<< HEAD
# BravoSix
SEBUAH PROGRAM PEMILIHAN BARANG SYSTEM JUAL BELI
public class Senapan {
private String jenis;  // Jenis senapan (misalnya AR-14, AK, BOLTAC)
private String nama;   // Nama senapan
private double harga;  // Harga senapan dalam satuan mata uang (rubel)
=======
# BravoSix Program Penjualan Senapan
public class Senapan {
    private String jenis;  // Jenis senapan (misalnya AR-14, AK, BOLTAC)
    private String nama;   // Nama senapan
    private double harga;  // Harga senapan dalam satuan mata uang (rubel)
>>>>>>> ccf747fc180c2a5251d99fde4d1b03d10f521d1f

    /**
     * Konstruktor kelas Senapan.
     *
     * @param jenis Jenis senapan (misalnya AR-14, AK, BOLTAC).
     * @param nama  Nama senapan.
     */
    public Senapan(String jenis, String nama) {
        this.jenis = jenis;
        this.nama = nama;

        // Inisialisasi harga berdasarkan jenis senapan
        if (jenis.equalsIgnoreCase("AR-14")) {
            this.harga = 1300; // Harga AR-14 dalam rubel
        } else if (jenis.equalsIgnoreCase("AK")) {
            this.harga = 800; // Harga AK dalam rubel
        } else if (jenis.equalsIgnoreCase("BOLTAC")) {
            this.harga = 1100; // Harga BOLTAC dalam rubel
        } else {
            this.harga = 0; // Harga default jika jenis tidak dikenal
        }
    }

    /**
     * Mendapatkan jenis senapan.
     *
     * @return Jenis senapan.
     */
    public String getJenis() {
        return jenis;
    }

    /**
     * Mendapatkan nama senapan.
     *
     * @return Nama senapan.
     */
    public String getNama() {
        return nama;
    }

    /**
     * Mendapatkan harga senapan.
     *
     * @return Harga senapan dalam mata uang (rubel).
     */
    public double getHarga() {
        return harga;
    }

    /**
     * Metode ini digunakan untuk mencetak informasi senapan.
     *
     * @return Informasi senapan dalam format String.
     */
    @Override
    public String toString() {
        return "Senapan{" +
                "jenis='" + jenis + '\'' +
                ", nama='" + nama + '\'' +
                ", harga=" + harga + " rubel";
    }
}
