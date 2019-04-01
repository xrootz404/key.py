# - * - coding: utf-8 - * -
impor os
impor sys
waktu impor
dari waktu tidur impor

g = "\ 033 [32; 1 m"
gt = "\ 033 [0; 32m"
bt = "\ 033 [34; 1m"
b = "\ 033 [36; 1 m"
m = "\ 033 [31; 1 m"
c = "\ 033 [0m"
p = "\ 033 [37; 1 m"
u = "\ 033 [35; 1 m"
M = "\ 033 [3; 1m"
k = "\ 033 [33; 1 m"
kt = "\ 033 [0; 33m"
a = "\ 033 [30; 1m"

W = "\ x1b [0m"
R = "\ x1b [31m"
G = "\ x1b [1; 32m"
O = "\ x1b [33m"
B = "\ x1b [34m"
P = "\ x1b [35m"
C = "\ x1b [36m"
GR = "\ x1b [37m"
def slowprints (s):
    untuk c dalam s + '\ n':
        sys.stdout.write (c)
        sys.stdout.flush ()
        time.sleep (2.0 / 90)

os.system ("clear")
semut = (gt + "" "
 ##### ####### # # # ######## 
# # # ## ## # # #    
# # # # # # # # #    
 ##### ##### # # # # # #    
      # # # # # # #    
# # # # # # # #    
 ##### ####### # # ##### #    
 =================================
"" ")
slowprints (semut)
cetak (gt + "")
masukan ('\ nTekan enter untuk melanjutkan ...')
tidur (2)
slowprints ("[!] Membuat direktori Properti Termux ...")
tidur (4)
mencoba:
      os.mkdir ("/ data / data / com.termux / file / home / .termux")
kecuali:
      lulus
slowprints ("[!] Sukses Membuat direktori Properti Termux!")
tidur (3)
slowprints ("[!] Membuat file Pengaturan ...")
tidur (1)

shortcutkey = "extra-keys = [['ESC', '/', '-', 'HOME', 'UP', 'END', 'PGUP'], ['TAB', 'CTRL', 'ALT' , 'KIRI', 'BAWAH', 'KANAN', 'PGDN']] "
script = open ('/ data / data / com.termux / file / home / .termux / termux.properties', 'w')
script.write (shortcutkey)
script.close ()
tidur (1)
slowprints ("[!] Berhasil Membuat File Pengaturan ...")
tidur (2)
slowprints ("\ n [!] Menyiapkan file pengaturan ...")
tidur (2)
os.system ("termux-reload-settings")
slowprints ("[!] Berhasil !! Membuat Kunci Pintas Termux, Terimakasih sudah memakai skrip ini untuk membantu Anda :)")
os.system ("rm -f key.py")
os.system ('keluar')
