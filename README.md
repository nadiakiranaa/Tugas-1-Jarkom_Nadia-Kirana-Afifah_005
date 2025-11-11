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
<img width="1002" height="380" alt="image" src="https://github.com/user-attachments/assets/b9a8c530-9b8e-4506-a4df-4c5337c07044" />


<img width="962" height="500" alt="image" src="https://github.com/user-attachments/assets/41585ae9-983b-4c70-aba8-5fbfac506bb4" />

## Tabel Subnetting Jaringan

| **Jaringan (ID)**             | **Network Address** | **Mask**           | **Prefix** | **Range Host**<br>(IP yang Dapat Digunakan) | **Broadcast** | **Gateway (Contoh)** |
|:-----------------------------:|:-------------------:|:------------------:|:----------:|:-------------------------------------------:|:-------------:|:---------------------:|
| SEKRETARIAT (A5)             | 10.45.0.0           | 255.255.254.0      | /23        | 10.45.0.1 - 10.45.1.254                      | 10.45.1.255    | 10.45.0.1             |
| BIDANG KURIKULUM (A2)        | 10.45.2.0           | 255.255.255.0      | /24        | 10.45.2.1 - 10.45.2.254                      | 10.45.2.255    | 10.45.2.1             |
| BIDANG GURU&TENDIK (A1)      | 10.45.3.0           | 255.255.255.128    | /25        | 10.45.3.1 - 10.45.3.126                      | 10.45.3.127    | 10.45.3.1             |
| BIDANG SARANA P. (A3)        | 10.45.3.128         | 255.255.255.192    | /26        | 10.45.3.129 - 10.45.3.190                    | 10.45.3.191    | 10.45.3.129           |
| SERVER & ADMIN (A4)          | 10.45.3.192         | 255.255.255.240    | /28        | 10.45.3.193 - 10.45.3.206                    | 10.45.3.207    | 10.45.3.193           |
| JARINGAN BACKBONE (A6)       | 10.45.3.208         | 255.255.255.248    | /29        | 10.45.3.209 - 10.45.3.214                    | 10.45.3.215    | 10.45.3.209           |
| BIDANG PENGAWAS (A7)         | 10.45.4.0           | 255.255.255.224    | /27        | 10.45.4.1 - 10.45.4.30                       | 10.45.4.31     | 10.45.4.1             |
| LINK WAN (A8)                | 10.45.4.32          | 255.255.255.252    | /30        | 10.45.4.33 - 10.45.4.34                      | 10.45.4.35     | 10.45.4.33            |





