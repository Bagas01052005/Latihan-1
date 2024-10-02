# Latihan-1
# Input Code :
# Data Pesawat
public class PesawatTempur {

    private final String warna;
    private int ketinggian; 
    private int kecepatan; 
    private int energi; 
    private String arah;
    private static final int MAX_KECEPATAN = 900;
    private static final int MAX_KETINGGIAN = 10000; 

    public PesawatTempur(String warna) {
        this.warna = warna;
        this.ketinggian = 0;
        this.kecepatan = 0;
        this.energi = 100;
        this.arah = "Utara";
    }


# Fungsi Untuk Menyalakan Mesin
public void nyalakanMesin() {
        System.out.println("Mesin pesawat dinyalakan...");
    }

# Fungsi Untuk Terbang
public void terbang() {
        if (this.kecepatan > 0) {
            if (this.energi >= 10) { 
                this.energi -= 10; // 
                System.out.println("Pesawat terbang...");
            } else {
                System.out.println("Energi tidak cukup untuk terbang.");
            }
        } else {
            System.out.println("Pesawat harus memiliki kecepatan untuk terbang.");
        }
    }
 

# Fungsi Untuk Menambahkan Kecepatan

 public void terbang() {
        if (this.kecepatan > 0) {
            if (this.energi >= 10) { 
                this.energi -= 10; // 
                System.out.println("Pesawat terbang...");
            } else {
                System.out.println("Energi tidak cukup untuk terbang.");
            }
        } else {
            System.out.println("Pesawat harus memiliki kecepatan untuk terbang.");
        }
    }

# Fungsi Untuk Belok

public void belok(String arah) {
        this.arah = arah;
        System.out.println("Pesawat berbelok ke arah " + this.arah);
    }

#  Fungsi Untuk Turun

public void turun() {
        if (this.ketinggian - 100 >= 0) {
            this.ketinggian -= 100;
            System.out.println("Pesawat turun ke ketinggian " + this.ketinggian + " meter");
        } else {
            System.out.println("Pesawat sudah berada di ketinggian minimum.");
        }
    }

# Fungsi Untuk Naik
public void naik() {
        if (this.ketinggian + 100 <= MAX_KETINGGIAN) {
            this.ketinggian += 100;
            System.out.println("Pesawat naik ke ketinggian " + this.ketinggian + " meter");
        } else {
            System.out.println("Tidak dapat naik, sudah mencapai ketinggian maksimum.");
        }
    }

