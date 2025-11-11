# JARKOM-1-TIARA-PUTRI

##  TOPOLOGI
<img width="1818" height="786" alt="Screenshot 2025-11-11 181208" src="https://github.com/user-attachments/assets/02470902-c4aa-4f99-9156-7562f2d9efbc" />


## SUBNETING

**IP Prefix:** `10.53.0.0/22`  
Total Host: **778** host

| Ruang / Jaringan | Kebutuhan Host | Prefix |
| :--- | :--- | :--- |
| Sekretariat | 381 | /23 |
| Bidang Kurikulum | 221 | /24 |
| Bidang Guru & Tendik | 96 | /25 |
| Bidang Sarana P. | 46 | /26 |
| Bidang Pengawas S. (Cabang) | 19 | /27 |
| Server & Admin | 7 | /28 |
| Interlink network | 6 | /29 |
| WAN Link | 2 | /30 |


# VLSM

| Ruang / Jaringan | Kebutuhan Host | Alokasi Host (Prefix) | Network | Mask | Prefix | Range Host (IP yang Bisa Dipakai) | Broadcast |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **WAN Link** | 2 | 2 | 10.53.0.0 | 255.255.255.252 | **/30** | 10.53.0.1 - 10.53.0.2 | 10.53.0.3 |
| **Interlink network** | 6 | 6 | **10.53.0.8** | 255.255.255.248 | **/29** | 10.53.0.9 - 10.53.0.14 | 10.53.1.15 |
| **Server & Admin** | 7 | 14 | 10.53.0.16 | 255.255.255.240 | **/28** | 10.53.0.17 - 10.53.0.30 | 10.53.0.31 |
| **Bidang Pengawas S.(Cabang)** | 19 | 30 | 10.53.0.32 | 255.255.255.224 | **/27** | 10.53.0.33 - 10.53.0.62 | 10.53.0.63 |
| **Bidang Sarana P.** | 46 | 62 | 10.53.0.64 | 255.255.255.192 | **/26** | 10.53.0.65 - 10.53.0.126 | 10.53.0.127 |
| **Bidang Guru & Tendik** | 96 | 126 | 10.53.0.128 | 255.255.255.128 | **/25** | 10.53.0.129 - 10.53.0.254 | 10.53.0.255 |
| **Bidang Kurikulum** | 221 | 254 | 10.53.1.0 | 255.255.255.0 | **/24** | 10.53.1.1 - 10.53.1.254 | 10.53.1.255 |
| **Sekretariat** | 381 | 510 | 10.53.2.0 | 255.255.254.0 | **/23** | 10.53.2.1 - 10.53.3.254 | 10.53.3.255 |

<img width="1662" height="680" alt="image" src="https://github.com/user-attachments/assets/5ab954ce-6f86-4667-86c9-d91e077678c6" />
<img width="881" height="836" alt="image" src="https://github.com/user-attachments/assets/4d94a2d7-483b-4137-b46b-b769c2aad353" />


# CIDR

| Nama Bidang (ID) | Network | Mask | Prefix | Range Host (IP yang Bisa Dipakai) | Broadcast | Gateway (Contoh) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **WAN Link (A8)** | 10.53.4.32 | 255.255.255.252 | **/30** | 10.53.4.33 - 10.53.4.34 | 10.53.4.35 | 10.53.4.33 |
| **Sekretariat (A1)** | 10.53.0.0 | 255.255.254.0 | **/23** | 10.53.0.1 - 10.53.1.254 | 10.53.1.255 | 10.53.0.1 |
| **Kurikulum (A2)** | 10.53.2.0 | 255.255.255.0 | **/24** | 10.53.2.1 - 10.53.2.254 | 10.53.2.255 | 10.53.2.1 |
| **Guru Tendik (A3)** | 10.53.3.0 | 255.255.255.128 | **/25** | 10.53.3.1 - 10.53.3.126 | 10.53.3.127 | 10.53.3.1 |
| **Sarana Prasarana (A4)** | 10.53.3.128 | 255.255.255.192 | **/26** | 10.53.3.129 - 10.53.3.190 | 10.53.3.191 | 10.53.3.129 |
| **Server & Admin (A5)** | 10.53.3.192 | 255.255.255.240 | **/28** | 10.53.3.193 - 10.53.3.206 | 10.53.3.207 | 10.53.3.193 |
| **Interlink Network (A7)** | 10.53.3.208 | 255.255.255.248 | **/29** | 10.53.3.209 - 10.53.3.214 | 10.53.3.215 | 10.53.3.209 |
| **Pengawas Sekolah (A6)** | 10.53.4.0 | 255.255.255.224 | **/27** | 10.53.4.1 - 10.53.4.30 | 10.53.4.31 | 10.53.4.1 |

<img width="1705" height="683" alt="image" src="https://github.com/user-attachments/assets/b0b89b1e-9083-44ff-b8e7-0f4d4fc02821" />
<img width="1313" height="498" alt="image" src="https://github.com/user-attachments/assets/f0e78101-16c1-4035-844c-d209e352b482" />


