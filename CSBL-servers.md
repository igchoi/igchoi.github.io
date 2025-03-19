# CSBL::Computing resources

1. eevee <img src="https://www.pokewiki.de/images/thumb/a/ad/Hauptartwork_133.png/405px-Hauptartwork_133.png" height=100 width=100> 16 cores/32 threaeds + 264 GB + RStudio server
2. flareon <img src="https://www.pokewiki.de/images/thumb/2/25/Hauptartwork_136.png/500px-Hauptartwork_136.png" height=100 width=100> 24 cores/48 threads + 256 GB
3. panpyro <img src="https://www.pokewiki.de/images/thumb/4/42/Hauptartwork_391.png/500px-Hauptartwork_391.png" height=100 width=100> 32 cores/64 threads + 512 GB + GPU (GTX 1660)
4. espeon <img src="https://www.pokewiki.de/images/thumb/9/90/Hauptartwork_196.png/500px-Hauptartwork_196.png" height=100 width=100> 6 cores/6 threads + 32 GB + GPU (GTX 1660)
5. jolteon <img src="https://www.pokewiki.de/images/thumb/e/e1/Hauptartwork_135.png/441px-Hauptartwork_135.png" width=100> 16 cores/32 threads + 78 GB + RStudio server
6. leafeon <img src="https://www.pokewiki.de/images/thumb/e/e6/Hauptartwork_470.png/427px-Hauptartwork_470.png" width=100> 12 cores/24 threads + 32 GB + GPU (RTX 3090)
7. compbio - CSBL lab web page
8. panflam <img src="https://www.pokewiki.de/images/thumb/f/fb/Hauptartwork_390.png/297px-Hauptartwork_390.png" height=100> NFS file server

---
`lscpu`
`free -h`
~~~
cat /proc/cpuinfo
cat /proc/meminfo
~~~
---
## 1. eevee (manger: BHPark)

* CPU: Intel(R) Xeon(R) CPU E5-2640 v2 @ 2.00GHz x2, 16 cores, 32 threads
* Memory: Total 264 GB

Slot | Name | Size | Clock
---- | ---- | ---- | ----
P1_DIMMA1 | Samsung DDR3-1333 | 64 GB | 1333 MHz
P1_DIMMA2 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P1_DIMMB1 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P1_DIMMB2 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P1_DIMMC1 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P1_DIMMC2 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P1_DIMMD1 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P1_DIMMD2 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P2_DIMME1 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P2_DIMME2 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P2_DIMMF1 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P2_DIMMF2 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P2_DIMMG1 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P2_DIMMG2 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P2_DIMMH1 | Samsung DDR3-1333 | 16 GB | 1333 MHz
P2_DIMMH2 | Samsung DDR3-1333 | 16 GB | 1333 MHz

* Disk

Type | Size | Directory | File
---- | ---- | ---- | ----
HDD | 2 TB | / | eevee root directory, eevee ubuntu
HDD | 16 TB | /eevee/analysis2/eevee/val | fungi analysis data (B.Min) 2016-2018, analysis data(/dev/sdb2)
HDD | 4 TB | /eevee/backup1 | backup data + analysis data
HDD | 8 TB | /eevee/ala, /eevee/gly | analysis data
HDD | 4 TB | /eevee/olddisk | old eevee root directory, old eevee home data

---

## 2. flareon (manager: BGKim)

* Motherboard: Supermicro X10DRi
* CPU: Intel(R) Xeon(R) CPU E5-2670 v3 @ 2.30GHz x2, 24 cores, 48 threads
* Memory: Total 256 GB

Slot | Name | Size | Clock
---- | ---- | ---- | ----
P1_DIMMA1 | Samsung DDR4-2133 ECC/REG | 32 GB | 2133 MHz
P1_DIMMA2 | Empty | |
P1_DIMMB1 | Samsung DDR4-2133 ECC/REG | 32 GB | 2133 MHz
P1_DIMMB2 | Empty | |
P1_DIMMC1 | Samsung DDR4-2133 ECC/REG | 16 GB | 2133 MHz
P1_DIMMC2 | Empty | |
P1_DIMMD1 | Samsung DDR4-2133 ECC/REG | 16 GB | 2133 MHz
P1_DIMMD2 | Empty | |
P2_DIMME1 | Samsung DDR4-2133 ECC/REG | 16 GB | 2133 MHz
P2_DIMME2 | Empty | |
P2_DIMMF1 | Samsung DDR4-2133 ECC/REG | 16 GB | 2133 MHz
P2_DIMMF2 | Empty | |
P2_DIMMG1 | Samsung DDR4-2133 ECC/REG | 32 GB | 2133 MHz
P2_DIMMG2 | Samsung DDR4-2133 ECC/REG | 32 GB | 2133 MHz
P2_DIMMH1 | Samsung DDR4-2133 ECC/REG | 32 GB | 2133 MHz
P2_DIMMH2 | Samsung DDR4-2133 ECC/REG | 32 GB | 2133 MHz

* Disk

Type | Size | Directory | File
---- | ---- | ---- | ----
HDD | 4 GB | / | root directory, ubuntu
HDD | 4 TB | /flareon/analysis2 | DNA/RNA-seq, analysis data (B. Min) 2016-2018
HDD | 4 TB | /flareon/analysis3 | DNA/RNA-seq, analysis data (B. Min) 2016-2018
HDD | 8 TB | /flareon/analysis5 | Miseq 20150121-20151203<br>Miseq 20191101-<br>Minion 20200612-
HDD | 16 TB | /flareon/analysis4<br>/flareon/analysis6| TCR SRA data<br>-

---
 
## 3. panpyro (manager: BGKim)

* Motherboard: ASUS KRPA-U16
* CPU: AMD EPYC 7452, 32 cores, 64 threads
* Memory: Total 512 GB
* GPU: GTX 1660

Slot | Name | Size | Clock
---- | ---- | ---- | ----
DIMM_A1 | Empty | |
DIMM_A2 | Samsung DDR4-2933 ECC/REG | 64 GB | 2933 MHz
DIMM_B1 | Empty | |
DIMM_B2 | Samsung DDR4-2933 ECC/REG | 64 GB | 2933 MHz
DIMM_C1 | Empty | |
DIMM_C2 | Samsung DDR4-2933 ECC/REG | 64 GB | 2933 MHz
DIMM_D1 | Empty | |
DIMM_D2 | Samsung DDR4-2933 ECC/REG | 64 GB | 2933 MHz
DIMM_E1 | Empty | |
DIMM_E2 | Samsung DDR4-2933 ECC/REG | 64 GB | 2933 MHz
DIMM_F1 | Empty | |
DIMM_F2 | Samsung DDR4-2933 ECC/REG | 64 GB | 2933 MHz
DIMM_G1 | Empty | |
DIMM_G2 | Samsung DDR4-2933 ECC/REG | 64 GB | 2933 MHz
DIMM_H1 | Empty | |
DIMM_H2 | Samsung DDR4-2933 ECC/REG | 64 GB | 2933 MHz

* Disk

Type | Size | Directory | File
---- | ---- | ---- | ----
SSD | 1 TB | / | root directory, ubuntu
HDD | 8 TB | /panpyro/alfa | ONT base calling data
HDD | 16 TB | /panpyro/bravo | empty
HDD | 4 TB | /panpyro/charlie | empty

---

## 4. espeon
* Motherboard: ASUS PRIME B360M-K
* CPU: Intel(R) Core(TM) i5-8400 CPU @ 2.80GHz, 6 cores, 6 threads
* Memory: Total 32 GB
* GPU: GTX 1660

Slot | Name | Size | Clock
---- | ---- | ---- | ----
ChannelA-DIMM1 | Samsung DDR4-2400 | 16 GB | 2400 MHz
ChannelB-DIMM1 | Samsung DDR4-2666 | 16 GB | 2666 MHz

* Disk

Type | Size | Directory | File
---- | ---- | ---- | ----
SSD | 250 GB | / | espeon root directory, espeon ubuntu
HDD | 4 TB | /espeon/analysis1 | ONT basecalling

---
## 5. jolteon 
* CPU: Intel(R) Xeon(R) CPU E5520 @ 2.27GHz, 16 cores, 32 threads
* Memory: Total 88 GB ([SAMSUNG DDR3](https://www.samsung.com/semiconductor/dram/module/M393B1K70CH0-CH9/) 8G x 11/1 empty slot)

----
## 6. leafeon 
* Motherboard: MSI MAG B550M Mortar WiFi
* CPU: AMD Ryzen 9 5900X, 12 cores, 24 threads
* Memory: Total 32 GB
* GPU: GIGABYTE AORUS GeForce RTX 3090 D6X 24GB

Slot | Name | Size | Clock
---- | ---- | ---- | ----
DIMM_A0 | Empty | |
DIMM_A1 | Samsung DDR4-2933 | 16 GB | 2933 MHz
DIMM_B0 | Empty | |
DIMM_B1 | Samsung DDR4-2933 | 16 GB | 2933 MHz

* Disk

Type | Size | Directory | File
---- | ---- | ---- | ----
SSD | 1 TB | / | leafeon root directory, leafeon ubuntu
HDD | 4 TB | /leafeon/analysis1 | AlphaFold data

---
## 7. compbio
* CPU: Intel(R) Core(TM) i7-3820 CPU @ 3.60GHz, 4 cores, 8 threads
* Memory: 32 GB ([SAMSUNG DDR3](https://www.samsung.com/semiconductor/dram/module/M393B1K70QB0-CK0/) 8G x 4)

---
## 8. free equipments

* DDR4 2933MHz(PC4-23400) ECC/REG 서버용 RAM 64GB x2
* DDR3 1333MHz(PC3-10600U) 2GB x1
* DDR2 800MHz(PC2-6400U) RAM 2GB x4
* Stored at R306

----
* GTX 1060 GPU (originally espeon) - __installed on PC (R319)__
