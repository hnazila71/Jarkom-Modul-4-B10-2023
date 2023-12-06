# Jarkom-Modul-4-B10-2023

### Nama Anggota B10
 <table>
 	<tr>
 		<td> Nama </td>
 		<td> NRP </td>
 	</tr>
 	<tr>
 		<td> Yusuf Hasan Nazila </td>
 		<td> 5025211225</td>
 	</tr>
	 <tr>
		 <td> Farhan Dwi Putra </td>
 		<td> 5025211093</td>
	 </tr>
 </table>

## Tree IP VLSM
Sebelum Pembagian IP VLSM maka terlebih dahulu membuat tree agar mempermudah untuk pembagian IP.

![Alt text](image-1.png)
 
Pertama kami mencari /19 karena paling besar atau bisa dibilang total dari seluruhnya. Mengapa diambil /19 karena total jumlah IP adalah 4255 tanpa NAT - Aura. Jadi ambil diatasnya karena untuk /20 tidak cukup dengan 4096 adresses. Setelah itu, kami menghabiskan children bagian kiri 

![Alt text](image-2.png)
        
Setelah bagian kiri habis sampai /30 paling kecil. Namun tidak ditambah IP berbeda dengan children bagian kanan

![Alt text](image-3.png)
 
Children bagian kanan akan ditambah dengan /30 jika /30 adalah children. Contoh
<table>
 	<tr>
 		<td> Awal </td>
        <td> Netmask </td>
 		<td> Akhir </td>
 	</tr>
 	<tr>
 		<td> 192.183.0.0 </td>
 		<td> /30</td>
        <td> 192.183.0.4</td>
 	</tr>
</table>

 ## Rute VLSM
 Kami membagi rute menjadi 21 A dan agar mempermudah mengingatnya kami membuat mengular A1 sampai A20. 
 
 ![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/39f70c54-1a2b-4a97-bdc4-cbf98f480ed1)

 Setelah kami bagi seperti itu kami membuat penggabungan CIDR 

 ## Penggabungan CIDR
### Penggabungan Pertama
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/c46b5362-9432-4cb6-a5ab-07bc0ccb495c)
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/0f1ca71f-857d-49e0-8ab7-d7a7bf17238d)

<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> B1 </td>
 		<td> A4 dan A5</td>
 	</tr>
	 <tr>
		 <td> B2 </td>
 		<td> A3 dan A7</td>
	 </tr>
</table>



### Penggabungan Kedua
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/e9de230e-0e28-449f-81e0-d3be3747e547)
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/3a2a6bbf-fa42-44e4-8e6a-701cb7d09cbf)

<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> C1 </td>
 		<td> B1 dan A14</td>
 	</tr>
	 <tr>
		 <td> C2 </td>
 		<td> B2 dan A2</td>
	 </tr>
</table>



### Penggabungan Ketiga
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/01bfef96-aae9-4472-a8a9-f2187388883b)
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/ed752e2f-6e53-4287-93e6-cdd226da9af8)


<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> D1 </td>
 		<td> C1 dan A15</td>
 	</tr>
	 <tr>
		 <td> D2 </td>
 		<td> C2 dan A8</td>
	 </tr>
</table>


### Penggabungan Keempat
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/1b2ec229-46c8-4e93-97c9-03a0cdc6241f)
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/e8243a72-91d0-4a04-86e3-c80aac73929a)



<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> E1 </td>
 		<td> D1 dan A13</td>
 	</tr>
	 <tr>
		 <td> E2 </td>
 		<td> D2 dan A1</td>
	 </tr>
</table>

### Penggabungan Kelima
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/ea8ed230-c0a6-45cf-a58e-2f724246f2c0)
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/7e1c395d-21f9-4c86-92db-e172d9b1da93)


<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> F1 </td>
 		<td> E1 dan A13</td>
 	</tr>
	 <tr>
		 <td> F2 </td>
 		<td> E2 dan A1</td>
	 </tr>
</table>

### Penggabungan Keenam
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/67ba732a-67ee-477a-bffb-086a46200621)
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/666a22f7-b4a6-4f31-b327-cedea5b5e8de)



<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> G1 </td>
 		<td> F1 dan A16</td>
 	</tr>
	 <tr>
		 <td> G2 </td>
 		<td> F2 dan A10</td>
	 </tr>
</table>

### Penggabungan Ketujuh
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/5e1c3045-951b-478f-af6d-092f727bef4f)
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/b6e694ee-7890-4c8d-bad6-df7185c8e414)


<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> H1 </td>
 		<td> G1 dan A21</td>
 	</tr>
	 <tr>
		 <td> H2 </td>
 		<td> G2 dan A11</td>
	 </tr>
</table>

### Penggabungan Kedelapan
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/f4840c2d-e9a4-4b07-84e7-645459bf56cb)
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/9546d6e9-ad31-416a-b342-f6708239d8c8)


<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> I1 </td>
 		<td> H1 dan A20</td>
 	</tr>
	 <tr>
		 <td> I2 </td>
 		<td> H2 dan A12</td>
	 </tr>
</table>

### Penggabungan Kesimbilan
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/58fb9302-2145-429f-b405-245d76266f32)
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/867a2202-c6ad-4aed-96c1-39677f47a2d5)




<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> J1 </td>
 		<td> I1 dan A17</td>
 	</tr>
	 <tr>
		 <td> J2 </td>
 		<td> I2 dan A18</td>
	 </tr>
</table>

### Penggabungan Kesepuluh
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/c86815f3-c28d-4e07-b656-afe6773ba99c)

<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> K2 </td>
 		<td> J1 dan A19</td>
 	</tr>
</table>

### Penggabungan Kesebelas
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/13c754f7-aa6c-404b-be2f-bec40163643e)


<table>
 	<tr>
 		<td> Subnet Baru </td>
 		<td> Subnet Gabungan </td>
 	</tr>
 	<tr>
 		<td> L2 </td>
 		<td> J2 dan K2</td>
 	</tr>
</table>

## Pembagian IP CIDR
<table>
    <thead>
        <tr>
            <th>Subnet</th>
            <th>Network ID</th>
            <th>Netmask</th>
            <th>Broadcast</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>A1</td>
            <td>192.199.16.0</td>
            <td>255.255.248.0</td>
            <td>192.199.23.255</td>
        </tr>
        <tr>
            <td>A2</td>
            <td>192.199.0.0</td>
            <td>255.255.252.0</td>
            <td>192.199.3.255</td>
        </tr>
        <tr>
            <td>A3</td>
            <td>192.199.4.0</td>
            <td>255.255.255.248</td>
            <td>192.199.4.7</td>
        </tr>
        <tr>
            <td>A4</td>
            <td>192.183.0.0</td>
            <td>255.255.252.0</td>
            <td>192.183.3.255</td>
        </tr>
        <tr>
            <td>A5</td>
            <td>192.183.4.0</td>
            <td>255.255.255.192</td>
            <td>192.183.4.63</td>
        </tr>
        <tr>
            <td>A6</td>
            <td>192.183.64.0</td>
            <td>255.255.255.248</td>
            <td>192.183.64.7</td>
        </tr>
        <tr>
            <td>A7</td>
            <td>192.199.4.8</td>
            <td>255.255.255.252</td>
            <td>192.199.4.11</td>
        </tr>
        <tr>
            <td>A8</td>
            <td>192.199.8.0</td>
            <td>255.255.255.252</td>
            <td>192.199.8.3</td>
        </tr>
        <tr>
            <td>A9</td>
            <td>192.199.32.0</td>
            <td>255.255.255.252</td>
            <td>192.199.32.3</td>
        </tr>
        <tr>
            <td>A10</td>
            <td>192.199.64.0</td>
            <td>255.255.255.224</td>
            <td>192.199.64.31</td>
        </tr>
        <tr>
            <td>A11</td>
            <td>192.199.128.0</td>
            <td>255.255.255.252</td>
            <td>192.199.128.3</td>
        </tr>
        <tr>
            <td>A12</td>
            <td>192.200.0.0</td>
            <td>255.255.255.252</td>
            <td>192.200.0.3</td>
        </tr>
        <tr>
            <td>A13</td>
            <td>192.183.32.0</td>
            <td>255.255.255.252</td>
            <td>192.183.32.3</td>
        </tr>
        <tr>
            <td>A14</td>
            <td>192.183.8.0</td>
            <td>255.255.255.252</td>
            <td>192.183.8.3</td>
        </tr>
        <tr>
            <td>A15</td>
            <td>192.183.16.0</td>
            <td>255.255.255.128</td>
            <td>192.183.16.127</td>
        </tr>
        <tr>
            <td>A16</td>
            <td>192.183.128.0</td>
            <td>255.255.255.252</td>
            <td>192.183.128.3</td>
        </tr>
        <tr>
            <td>A17</td>
            <td>192.187.0.0</td>
            <td>255.255.255.252</td>
            <td>192.187.0.3</td>
        </tr>
        <tr>
            <td>A18</td>
            <td>192.201.0.0</td>
            <td>255.255.255.252</td>
            <td>192.201.0.3</td>
        </tr>
        <tr>
            <td>A19</td>
            <td>192.191.0.0</td>
            <td>255.255.255.0</td>
            <td>192.191.0.255</td>
        </tr>
        <tr>
            <td>A20</td>
            <td>192.185.12.0</td>
            <td>255.255.252.0</td>
            <td>192.185.15.255</td>
        </tr>
	    <tr>
            <td>A21</td>
            <td>192.184.22.0</td>
            <td>255.255.255.0</td>
            <td>192.184.22.255</td>
        </tr>
	         <tr>
            <td>B1</td>
            <td>192.183.0.0</td>
            <td>255.255.248.0</td>
            <td>192.183.7.255</td>
        </tr>
        <tr>
            <td>B2</td>
            <td>192.199.4.0</td>
            <td>255.255.255.240</td>
            <td>192.199.4.15</td>
        </tr>
        <tr>
            <td>C1</td>
            <td>192.183.0.0</td>
            <td>255.255.240.0</td>
            <td>192.183.15.255</td>
        </tr>
        <tr>
            <td>C2</td>
            <td>192.199.0.0</td>
            <td>255.255.248.0</td>
            <td>192.199.7.255</td>
        </tr>
        <tr>
            <td>D1</td>
            <td>192.183.0.0</td>
            <td>255.255.224.0</td>
            <td>192.183.31.255</td>
        </tr>
        <tr>
            <td>D2</td>
            <td>192.199.0.0</td>
            <td>255.255.240.0</td>
            <td>192.199.15.255</td>
        </tr>
        <tr>
            <td>E1</td>
            <td>192.183.0.0</td>
            <td>255.255.192.0</td>
            <td>192.183.63.255</td>
        </tr>
        <tr>
            <td>E2</td>
            <td>192.199.0.0</td>
            <td>255.255.224.0</td>
            <td>192.199.31.255</td>
        </tr>
        <tr>
            <td>F1</td>
            <td>192.183.0.0</td>
            <td>255.255.128.0</td>
            <td>192.183.127.255</td>
        </tr>
        <tr>
            <td>F2</td>
            <td>192.199.0.0</td>
            <td>255.255.192.0</td>
            <td>192.199.63.255</td>
        </tr>
        <tr>
            <td>G1</td>
            <td>192.183.0.0</td>
            <td>255.255.0.0</td>
            <td>192.183.255.255</td>
        </tr>
        <tr>
            <td>G2</td>
            <td>192.199.0.0</td>
            <td>255.255.128.0</td>
            <td>192.199.127.255</td>
        </tr>
        <tr>
            <td>H1</td>
            <td>192.183.0.0</td>
            <td>255.254.0.0</td>
            <td>192.183.255.255</td>
        </tr>
        <tr>
            <td>H2</td>
            <td>192.199.0.0</td>
            <td>255.255.0.0</td>
            <td>192.199.255.255</td>
        </tr>
        <tr>
            <td>I1</td>
            <td>192.183.0.0</td>
            <td>255.252.0.0</td>
            <td>192.183.255.255</td>
        </tr>
        <tr>
            <td>I2</td>
            <td>192.199.0.0</td>
            <td>255.254.0.0</td>
            <td>192.199.255.255</td>
        </tr>
        <tr>
            <td>J1</td>
            <td>192.183.0.0</td>
            <td>255.248.0.0</td>
            <td>192.183.255.255</td>
        </tr>
        <tr>
            <td>J2</td>
            <td>192.199.0.0</td>
            <td>255.252.0.0</td>
            <td>192.199.255.255</td>
        </tr>
        <tr>
            <td>K1</td>
            <td>192.183.0.0</td>
            <td>255.240.0.0</td>
            <td>192.183.255.255</td>
        </tr>
        <tr>
            <td>L1</td>
            <td>192.183.0.0</td>
            <td>255.224.0.0</td>
            <td>192.183.255.255</td>
        </tr>
    </tbody>
</table>
![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/e60f4543-3004-4acf-bb04-65cfcd8ff999)


## Tree CIDR
Kami membuat tree dengan penjelasan 
1. Kami membuat parent awal 192.183.0.0/11 itu IP paling awal jika di tabel adalah L1 paling bawah. Jadi pembacaannya dari bawah ke atas
2. Setelah parent terbuat ip akan diturunkan pada kedua anaknya dengan awal ip sama tetapi Netmask yang berbeda
   ![image](https://github.com/hnazila71/Jarkom-Modul-4-B10-2023/assets/114125438/9fb25a49-1caf-43f9-a55a-3f7c5fd2b784)
3. Jika sudah diturunkan ipnya, dapat dibandingan. Jika netmasknya lebih besar ( /12 > /14 ) maka ip bagian /14 akan (192.183.0.0/14) + (0.0.16.0) ditambah SubnetMask /12

    ![Alt text](image.png)

 

