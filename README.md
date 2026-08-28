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

# Why 16s 120A ESC?
HvX 120 is an open-source ESC hardware design provided by the Alka_Motor_32 project. It can be self-replicated with only some soldering and firmware-uploading skills, which the majority of DIY hobiest already have. if you want to make a drone that will go over 300kmph or a 12s monster of power speed car thats power demand will insanely high and you dont want to spend crazy 1000$ only for the ESC, Hvx 120 is for you. A conventional HV/I ESC will cost you around 80-130$. But if you build HvX 120 16s AM32 ESC, you can get 5 ESCs at ~170$; that's only costing around 35$ each:). Also, as you are building it, it would be very easy to fix one if damaged.

# Documentations
In this repository, you can find the Schematics, Gerber file, pick and place(if you plan to use PCBA from PCB manufacturer), and all the components you need(aka BOM) files, along with all the steps to build your own 16s 120A ESC. Also, if you want to make a small but 4IN1 2-4s 25A ESC then checkout [Nano-2-4s-AM32-ESC](https://github.com/minhazislamnafi/Nano-2-4s-AM32-ESC).

# Quick Start

## Requirements

## Components:

* MCU: Artery AT32F421G8U7 120MHz QFN-28 [link](https://s.click.aliexpress.com/e/_c4PMPWk9)
* Mosfet: AONR36366 QFN-8 package [link](https://s.click.aliexpress.com/e/_c3cixcnL)
* Gate driver: DRV8300DPWR TSSOP20 [link](https://s.click.aliexpress.com/e/_c3NqUJhL)
* 12V Buck: LM5164DDAR soic-8 [link](https://s.click.aliexpress.com/e/_c3Sop7Lp)
* 3.3v ldo: AMS1117 sot-89 [link](https://s.click.aliexpress.com/e/_c2wS5Ae7)
* current sense: INA280A2  [link](https://www.aliexpress.com/item/1005011927472126.html?)
* Shunt: 2512 3W R001 1MR [Link](https://www.aliexpress.com/item/1005010000851939.html?)
* Resistors: 10k, 1k, 10R etc 0402 size [link](https://s.click.aliexpress.com/e/_c4mdiRd3)
* Capacitors: 10uf, 1uf, 100nf, etc 0402 size [Link](https://s.click.aliexpress.com/e/_c3HHiS9r)

## For detailed part list, price, and values checkout [BOM]()

## PCB
Use JLCPCB if you're in ASIA or PCBWAY if you're in America. Also, find what manufacturer is better for you. 
If you just want to get Flight controller PCB then use this [GARBER file](https://github.com/minhazislamnafi/HvX-120-AM32-ESC/blob/main/PCB/Production/Gerber_16s_120A_am32_esc_v1.1.zip),Download it and place order.
Or if you just want to build your own PCB, then follow this [SCHEMATICS](https://github.com/minhazislamnafi/HvX-120-AM32-ESC/blob/main/PCB/Production/SCH_16s%20120A%20am32%20esc_v1.1.pdf).

## 6 Layers

<img width="1920" height="1908" alt="HvX 120A 6 layer render" src="https://github.com/user-attachments/assets/6d5c2af8-d58c-4311-b74f-704e36a03c1c" />


## PCB render

## FOLLOW THESE STEPS ##

**1. Spend some money $$ to buy the parts mentioned in [BOM]().**

**2. Order the Nano ESC PCB using this [GERBER file](https://github.com/minhazislamnafi/HvX-120-AM32-ESC/blob/main/PCB/Production/Gerber_16s_120A_am32_esc_v1.1.zip).**

**3. Solder the SMD components of the PCB by hand ;) Or just order the PCBs with PCBA services, btw it will cost a lot.**

**4. Solder 18 AWG wire with xt30 connector to the power pads.**

**5. Check with multimeter- Is mcu getting 3.3v or not, if not diagnose by yourself :)**

**6. Flash each MCU with AM32 firmware using Stlink v2 programmer ( I will add every step in details, once I have built IRL:)**

## Special thanks to-
EasyEDA-OSHWLab (sponsored by)

Hackclub 
