### Konsep Blockchain
dikembangkan ke narasi dari sumber
https://www.youtube.com/watch?v=R2LQa5LCRwo

thanks: 
Friends with Blockchain

#### Ilustrasi
di dalam sebuah kelas ada 2 roles utama, murids dan guru.
hari ini lagi ujian nich, dan guru ngasih pertanyaan kira-kira 5 soal.
gampang kok, soalnya cuma pertambahan aja, kamu pasti bisa.

#### Aturan
untuk setiap siswa ikuti aturan ini ya,
untuk setiap pertanyaan penjumlahan di jawab dan dihitung seperti biasa.
setiap jawaban disimpan ke lembar jawab (ledger)
cuma sebagai catatan, hasil perhitungan juga ditambah dengan hasil perhitungan soal sebelumnya (aturan hash chain).

misal, soal sebagai berikut
1. 1+1 ?
2. 2+2 ?
...

maka kalian harus menghitung dengan cara
1. (1+1) = 2 => jawaban normal
2. (2+2) + (hasil 1.) = (2+2) + 2 = 6 => dijumlahkan dengan hasil soal sebelumnya
... => begitupun seterusnya

jadi sampai sini paham kan ?

nah kalau udah paham kita mulai ujiannya ya,

#### Desentralisasi
konsep desentralisasi artinya,
data jawaban boleh dimiliki semua orang, dan semua jawaban harus sama.

jadi misal ada 5 murids di kelas, (A, B, C, D, E)
soal dari guru
1. 2+2 ?

A: 4!
B: ?
C: ?
D: ?
E: ?

nah si A bisa ngitung duluan nih.
dan karena ada konsep DESENTRALISASI,
maka murids lain harus mengecek jawaban dan mencatat hal yang sama.

jadi kurang lebih sekarang jawabannya

A: 4
B: 4
C: 4
D: 4
E: 4

nah jadi sama semua kan.
intinya gitu deh kalau DESENTRALISASI :)

#### Konsensus
lanjut ke konsep KONSENSUS
langsung ke soal aja ya,
o iya sekarang fokus ke soal 2 ya
soalnya soal 1 kan udah kejawab

1. 2+2 = 4
2. 3+3 ?

ayo murids, dijawab ya

A: 5 + (4), 9!
B: ?
C: ?
D: 6 + (4), 10!
E: ?

waduh, kali ini ada 2 jawaban beda nich
tapi gpp, murids akhirnya tetep ikut konsep DESENTRALISASI

si B yang deket sama si A,
nyatet jawaban yang sama kayak A

sementara si C dan E,
karena lebih deket ke D,
dia nyatet jawaban kayak jawaban si D,

jadi kurang lebih jadi kayak gini

A: 9	->	pemilik jawaban
B: 9
C: 10
D: 10	->	pemilik jawaban
E: 10

haha makin runyam ya,
nah kalau kondisinya kayak gini gimana nich?

untuk mengatasi hal tersebut,
pemilik jawaban berbeda akan beradu,
karena ada 2 jawaban berbeda dan yang paling deket adalah
posisi B (10) dan C (9),

maka mereka akan voting
dan ngeliat jawaban mana yang voters nya paling banyak
berarti didapat

9	=>	2 orang
10	=>	3 orang

nah dari solusi itu akhirnya semua sepakat
kalau jawabannya adalah 10

dan semua jawaban murids akan jadi kayak gini

A: 10
B: 10
C: 10
D: 10
E: 10

nah proses voting tadi tuh yang dinamakan KONSENSUS,
jadi semua murids harus memiliki persetujuan yang sama,
tujuannya agar data yang mereka record juga selalu sama,
gitu.

lanjut ya

#### Immutable dan Transparansi
immutable artinya
data yang sudah masuk tidak dapat diubah

contoh ilustasi sebagai berikut

emm, sebagai contoh
kita pakai jawaban nomor 1 dan 2

A:	4
	10
B:	4
	10
C:	4
	10
D:	4
	10
E:	4
	10

nah, tiba-tiba si B jail nih
dia pengen ngubah jawaban nomor 1 jadi 3 misalnya,
maka jawaban B akan menjadi

B:	3
	9*

* nah, kenapa jawaban kedua jadi 9 ?
karena jawaban nomor 1 berubah
dan ada aturan hash chain (penambahan dengan record sebelumnya)
maka jawanan nomor 2 menjadi (6 + 3) = 9

nah dari situ,
si B sadar nih kalau jawaban dia dengan jawaban si A beda.

maka B akan mengecek jawaban murids lainnya,
dan karena jawabannya sama dengan murids C, D, dan E
maka dia memaksa si A untuk mengganti jawabannya
agar tetap bisa ikutan di kelas Blockchain.

itulah kelebihan dari blockchain,
dimana data yang sudah disimpan tidak dapat diubah (immutable)
dan semua data bersifat transparan,
yang berarti data dapat dilihat, dimiliki dan divalidasi setiap orang

#### Kasus Tambahan

- penambahan murid baru

gimana ya kalau tiba-tiba,
ada murid baru yang mau ikutan join ke kelas ?
misal namanya si X

karena syarat untuk mengikuti kelas adalah
data jawaban yang ditulis semua siswa sama,
maka si X harus mencatat semua jawaban dari murids
dari soal pertama sampai soal saat dia join

nah kalau si X udah menulis semuanya,
dia baru boleh join ke kelas