XT Keyboard Project:

This repo is for all the files used in designing and manufacturing a mechanical keyboard that I made from scratch.
The keyboard itself is a modified XT layout, which was a very popular layout for 1980's keyboards.

The case is inspired by the IBM Model F77, Cherry G80-0418 and the modern NCR80.
Later angularity and side-bezel thickness was inspired by the Pravetz 16 from the Soviet Union and various NCR G80 varieties, for example the NCR G80-0478.

The pcb is designed with Kailh Hotswap Sockets (Although I just soldered my switches directly), all of which are south facing to avoid Cherry profile interference. 
The layout is a mix of various layout types, such as the ISO left side 1.25u shift, split right shift, split backspace, which are not changeable.
It does however support stepped caps lock as well as a regular caps lock.
The PCB was originally designed with using the ATMega32u4, but after a failed iteration, it was replaced with an RP2040 PCB design instead.
Using the RP2040 enabled QMK firmware compatibility + VIA.
Due to the case dimensions, the main intended I/O for the keyboard is not the USB type C Receptible., rather using a 4-pin Molex Pico EZmate connector and a daughterboard,
in this instance the UDB (Unified Daughterboard) C4. However, a full USB type C receptible + ESD protection diode has been added 
due to the troubleshooting utility (makes diagnosing issues with PCB and/or daughterboard easier).
The new RP2040 based pcb introduces new quality of life features, such as readily available GND, 3V, RESET, SWD and SWC pins for ISP programming, making troubleshooting a lot simpler
should there be need to program the chip's bootloader.

1. Layout

![Capture2](https://github.com/user-attachments/assets/e3e69016-4f0c-4fa5-b3fa-685c7375eff4)

The layout is a mix of the standard HHKB for the Alphanumerical section, XT-esque left side F-row and a 3x5 1U grid inspired by the IBM Model F-77


2. Schematics

Early visualization of switch matrix (This layout was changed tremendously due to later solutions for multiple layouts)
![switch_matrix](https://github.com/user-attachments/assets/95c27249-d844-417f-8f49-6b42e8cd5660)

Switch matrix translated to Kicad schematics
![image](https://github.com/user-attachments/assets/7596c16a-e567-44c9-9e53-6f9ca3beb4c7)

Full schematics of the board
<img width="1585" height="1108" alt="bilde" src="https://github.com/user-attachments/assets/77a6be75-2840-4389-ac78-cb80268a3433" />

Routed pcb
<img width="2634" height="851" alt="bilde" src="https://github.com/user-attachments/assets/10958409-800d-4fe8-b5ec-53f38484b790" />
<img width="2599" height="838" alt="bilde" src="https://github.com/user-attachments/assets/83303975-92e7-427c-95ac-b508fcf2fe02" />
<img width="2624" height="813" alt="bilde" src="https://github.com/user-attachments/assets/355dc0bd-2a98-4654-b808-0ef46eac364d" />

3D render (front)
<img width="3140" height="992" alt="bilde" src="https://github.com/user-attachments/assets/2c651051-5751-4e92-a2b0-3074f3beebcd" />

3D render (back)
<img width="3090" height="948" alt="bilde" src="https://github.com/user-attachments/assets/05d28440-9243-46b1-96df-ae4bc6170f0a" />

RP2040, Crystal and Debug pins
<img width="1599" height="1226" alt="bilde" src="https://github.com/user-attachments/assets/62eb9494-7fab-4bb0-9ab0-2d8cfe1dd27f" />

USB Type C Recepticle, ESD Protection Diode and 4-pin Molex Connector
<img width="1071" height="1217" alt="bilde" src="https://github.com/user-attachments/assets/8655463c-627f-442e-9d40-b0e63d6718fa" />


3. Case

Top case w/ plate
![image](https://github.com/user-attachments/assets/9f860870-c5fe-4c5c-9853-4eb4e035fadd)

Top and Bottom case side profile
![image](https://github.com/user-attachments/assets/20adbc17-2f2d-4fc6-b934-0e6ee397a117)
![image](https://github.com/user-attachments/assets/dd33151b-3cc4-4977-9c6c-7f1deee1dfd3)

Back view including slit for UDB implementation
![image](https://github.com/user-attachments/assets/30c8c7ed-502e-4187-ba88-faa97b426f0f)

Inside view of Top case, showing plate top mount + UDB implementation
![image](https://github.com/user-attachments/assets/522249ea-5ca1-4010-b5e6-2631f98cf70f)

Inside view of Bottom case
![image](https://github.com/user-attachments/assets/adb34f13-e858-492b-97dc-4f97b93c774f)

Bottom
![image](https://github.com/user-attachments/assets/43b9d7e2-eea3-4b82-b5ae-db989650cbc5)


To be posted:
Manufactured PCBA and Aluminium case



