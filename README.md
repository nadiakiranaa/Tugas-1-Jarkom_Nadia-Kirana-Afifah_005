# Tugas-1-Jarkom_Nadia-Kirana-Afifah_005
# TOPOLOGI #
<img width="1318" height="367" alt="image" src="https://github.com/user-attachments/assets/dae31e0d-4029-4239-9b4f-65805550fa32" />


## Tabel Subnetting Jaringan

| **Nama Subnet**              | **Kebutuhan Sebenarnya**<br>(Host + Gateway) | **Jumlah Alamat IP**<br>(Ukuran Blok) | **Netmask** | **Netmask (Desimal)**     |
|:----------------------------:|:-------------------------------------------:|:-------------------------------------:|:-----------:|:--------------------------:|
| Sekretariat                 | 381                                         | 512                                   | /23         | 255.255.254.0              |
| Bidang Kurikulum            | 221                                         | 256                                   | /24         | 255.255.255.0              |
| Bidang Guru & Tendik        | 96                                          | 128                                   | /25         | 255.255.255.128            |
| Bidang Sarana Prasarana     | 46                                          | 64                                    | /26         | 255.255.255.192            |
| Bidang Pengawas Sekolah     | 19                                          | 32                                    | /27         | 255.255.255.224            |
| Server & Admin              | 7                                           | 16                                    | /28         | 255.255.255.240            |
| Jaringan Backbone           | 6                                           | 8                                     | /29         | 255.255.255.248            |
| Link WAN                    | 2                                           | 4                                     | /30         | 255.255.255.252            |
| **Total**                   | **778**                                     |                                       |             |                            |



# VLSM #
<img width="697" height="498" alt="image" src="https://github.com/user-attachments/assets/8fce525b-f51f-47ae-a9f3-81bc4d2b2419" />



## Tabel Konfigurasi Subnet Jaringan

| **Nama Subnet**              | **Network**   | **Mask**           | **Prefix** | **Range Host**<br>(IP Pasgan/Broadcast) | **Broadcast** | **Gateway (Contoh)** |
|:----------------------------:|:-------------:|:------------------:|:----------:|:---------------------------------------:|:-------------:|:---------------------:|
| Sekretariat                 | 10.45.2.0     | 255.255.254.0    | /23        | 10.45.2.1 - 10.45.3.254                  | 10.45.3.255    | 10.45.2.1             |
| Bidang Kurikulum            | 10.45.1.0     | 255.255.255.0    | /24        | 10.45.1.1 - 10.45.1.254                  | 10.45.1.255    | 10.45.1.1             |
| Bidang Guru & Tendik        | 10.45.0.128    | 255.255.255.128   | /25        | 10.45.0.129 - 10.45.0.254                  | 10.45.0.255    | 10.45.0.129            |
| Bidang Sarana Prasarana     | 10.45.0.64    | 255.255.255.192   | /26       | 10.45.0.65 - 10.45.0.126                  | 10.45.0.127   | 10.45.0.65            |
| Bidang Pengawas Sekolah     | 10.45.0.32     | 255.255.255.224    | /27        | 10.45.0.33 - 10.45.0.62                  | 10.45.0.63    | 10.45.0.33            |
| Server & Admin              | 10.45.0.16     | 255.255.255.240    | /28        | 10.45.0.17 - 10.45.0.30                 | 10.45.0.31    | 10.45.0.17             |
| Jaringan Backbone           | 10.45.0.8     | 255.255.255.248    | /29       | 10.45.0.9 - 10.45.0.14                 | 10.45.0.15    | 10.45.0.9            |
| Link WAN                    | 10.45.0.0    | 255.255.255.252   | /30        | 10.45.0.1 - 10.45.0.2                 | 10.45.0.3    | 10.45.0.1            |

# CIDR #
<img width="1008" height="413" alt="image" src="https://github.com/user-attachments/assets/d68178d8-9e1e-43b3-bde3-cbb2d36d09d9" />




