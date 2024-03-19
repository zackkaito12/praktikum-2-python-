# praktikum-2-python-
print("Bus PT.ANS Lintas Sumatera")
print("TUJUAN\n1.Medan     : RP90000\n2.Padang    : RP20000\n3.Palembang : RP75000\n4.Aceh      : RP80000\n5.Jambi     : RP160000\n6.Riau      : RP120000\n")
tj = int(input("Tujuan yang dipilih: "))
tujuan = ""
if tj == 1:
    tujuan = "Medan"
    tj = 90000
elif tj == 2:
    tujuan = "Padang"
    tj = 20000
elif tj == 3:
    tujuan = "Palembang"
    tj = 75000
elif tj == 4:
    tujuan = "Aceh"
    tj = 80000
elif tj == 5:
    tujuan = "Jambi"
    tj = 160000
elif tj == 6:
    tujuan = "Riau"
    tj = 120000
else:
    print("ERROR")
    exit()

#print("\n-------------------------------------------------------------------------------------------------------------------------------------\n")

print("KELAS\n1.Ekonomi Class : Rp 10000\n2.Bisnis Class  : Rp 20000\n3.First Class   : Rp 30000\n")
kl = int(input("Pilih kelas: "))
jt = int(input("Jumlah Tiket: "))
nama_kelas = ""
if kl == 1:
    nama_kelas = "Ekonomi Class"
    kl = 10000
elif kl == 2:
    nama_kelas = "Bisnis Class"
    kl = 20000
elif kl == 3:
    nama_kelas = "First Class"
    kl = 30000
else:
    print("ERROR")
    exit()

#print("\n-------------------------------------------------------------------------------------------------------------------------------------\n")

ds = 0
if jt >= 3 and jt <= 5:
    ds = 0.05
elif jt > 5:
    ds = 0.1

total = jt * (tj + kl)
totald = total * (1 - ds)

print("\n-------------------------------------------------------------------------------------------------------------------------------------\n")
print("Tujuan         :", tujuan)
print("Kelas          :", nama_kelas)
print("Jumlah Tiket   :", jt)
print("Total          : Rp", total)
print("Diskon         :", ds * 100, "%")
print("Total Setelah Diskon         : Rp", totald)
print("-------------------------------------------------------------------------------------------------------------------------------------\n")
