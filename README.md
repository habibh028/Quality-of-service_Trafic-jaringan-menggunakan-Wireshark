# Quality-of-service_Trafic-jaringan-menggunakan-Wireshark

# Nama Kelompok: 
# 1.) Habib Hubaddilah
# 2.) Muh Faisal Bimantara

Yang dibutuhkan
1. Software Wireshark
2. Koneksi wifi

Memulai Praktik:
1.	Pada bagian ini saya mencoba menjalankan paket data melalui Wireshark dengan Capturing From Wi-Fi seperti gambar di bawah ini. Bagian ini saya memerlukan waktu 10 menit untuk mendapatkan paket data yang sedang berjalan. Seperti Gambar dibawah ini saya mulai pada pukul 09.25 

    ![image](https://github.com/habibh028/Quality-of-service_Trafic-jaringan-menggunakan-Wireshark/assets/126387192/3cf9f4c2-1bd1-4ddc-ba86-0c25f8b4568d)

2.	Setelah 10 menit berjalan didapatkan paket data 57553 seperti gambar dibawah ini :
 
    ![image](https://github.com/habibh028/Quality-of-service_Trafic-jaringan-menggunakan-Wireshark/assets/126387192/48cd604d-4a4f-47f6-8258-f1014ecc55bb)

3.	THROUGHPUT 
    Berikut adalah data yang didapatkan dari paket data yang berjalan pada jarigan Wi-Fi, seperti gambar di bawah ini :
 
     ![33333](https://github.com/habibh028/Quality-of-service_Trafic-jaringan-menggunakan-Wireshark/assets/126387192/3db9b1b3-b351-4f54-a81a-4d55600ce88e)


            -Throughput
        	  jumlah byte / Time Span = 58717599 Byte /  612,081 s
        				= 95931 Bytes/s
        				= 95,931 KB/s
        				= 95,931 Kb/s x 8
        				= 767,448 Kb/s

4.	PACKET LOSS 
    Dengan melakukan filtering data, didapatlah beberapa data paket yang tidak terkirim.Berikut adalah data packet loss yang terjadi :
    
            -Packet Loss 
              	((Paket Dikirim - Paket Diterima)/Paket Dikirim)x100
              	= ((57553 - 56.218)/57553)x 100
              	= (1335/57553)x 100
              	= 2,374684264826212
    

5.	DELAY 
    Convert semua packet tersebut menjadi format CSV dan lakukan analisis data melalui excel. Karna yang diperlukan hanya informasi waktu, maka hilangkan kolum informasi lain pada file csv yang sudah di export
     ![5555](https://github.com/habibh028/Quality-of-service_Trafic-jaringan-menggunakan-Wireshark/assets/126387192/6d134ea4-4ba8-4dbd-bfa1-bb42be24e0fa)

    Analisis yang didapatkan :
   
    ![6](https://github.com/habibh028/Quality-of-service_Trafic-jaringan-menggunakan-Wireshark/assets/126387192/5b52d8e1-b5a4-4580-9f01-ec8bd7e9f94f)

  
    Time 1 = Waktu awal 
    Time 2 = Waktu awal yang diulai setelah 0 
    Delay = Time 2 – Time 1

  	![55](https://github.com/habibh028/Quality-of-service_Trafic-jaringan-menggunakan-Wireshark/assets/126387192/56ffe6fd-cccc-4d0c-b4bd-8a9247dc1375)

          -Delay
          total delay : 611,521046
          rata rata delay : 0,010625355


5.	JITTER
    Analisis yang didapatkan adalah : 
    Delay 1 = Nilai Delay – Nilai Delay Setelahnya 
    Delay 2 = Semua Nilai Delay, Kecuali Delay Pertama 
    Jitter = Delay – Delay 1
    
    Jadi, Didapatkan hasil dari nilai jitter dan rata – rata jitter juga didapatkan sebagai berikut

    ![11](https://github.com/habibh028/Quality-of-service_Trafic-jaringan-menggunakan-Wireshark/assets/126387192/d12bb4a1-51da-4b30-9f2d-470af2f2c97c)


          -Jitter
          total jiter : 611,463206
          rata rata jitter : 0,01062435
