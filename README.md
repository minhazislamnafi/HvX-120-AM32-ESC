# HvX-120-AM32-ESC

![License](https://img.shields.io/badge/license-OHL_v2-green.svg)
![Alka motor 32](https://img.shields.io/badge/Firmwire-AM32-red)
![pcb](https://img.shields.io/badge/HvX_120-v1-blue)
![in Volt](https://img.shields.io/badge/120A-4~16S-cyan)


An ESC that will run on AM32 firmware. Specs: up to 120A, 16s (65v).Supports ESC telemetry. 6-layer PCB design, that's it.

<img width="4000" height="5657" alt="NEW ON THE MENU" src="https://github.com/user-attachments/assets/508059e6-d283-49a0-885e-32ecdc676270" />


# Specification

* Firmwire: AlkaMotor32(AM32) 

* ESC: Single high power

* MCU: Artery AT32F421 120MHz(QFN28)

* Mosfet: FDBL0200N100  from Onsemi

* Gate Driver: DRV8300DPWR  (TSSOP20)

* Input voltage: 4-16s Lipo/Lipohv (12-68v)

* Output current: ~100A continuous (140A brust for 5s)

* Mounting size: none (frame-mounted)

* Regulator : Onboard 12V buck converter (LM5164DDAR)

* MCU 3.3V? : LDO(AMS1117-3.3VS) from onboard 12v

* Current sensing: INA280A2 

* Shunt : 3 2512 1 mOhm 3W in parallel to get 0.33mOhm and 9W
