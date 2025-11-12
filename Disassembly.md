# 🧩 Disassembly of the Kasa Pan/Tilt/Zoom Security Camera

This document details the full disassembly process of my personally owned Kasa PTZ security camera for educational and hardware research purposes.  
All actions were performed carefully to avoid damage to the components and to document internal architecture for analysis.

> ⚠️ **Disclaimer:**  
> This process was performed on a personally owned device for research, interoperability, and educational study.  
> Do **not** attempt to disassemble devices you do not own. Disassembly may void warranties.

---

## 🔍 1. Initial Overview

The disassembly process was challenging to initiate due to the device’s compact structure and hidden clips.  
Two potential entry points were identified:

1. A **connection point** visible within the dome section.  
2. The **rotational joint** where the motor base connects to the camera assembly.

`![Initial Overview](pics/Assembled_Camera.jpeg)`

---

## 🔧 2. First Attempt — Base (Motor Rotation Section)

The first approach focused on the **motor rotation base**, as it also housed the power cable connection.  
I initially assumed the **PCB (main board)** would be located in this section since there appeared to be ample space and a direct power route.

Despite multiple careful attempts to separate this section, the base did not come apart easily, and no visible clips or screws were accessible.  
After confirming it was not the correct entry point, I decided to shift focus to the upper dome.

*(Insert image of motor base attempt here)*  
`![Motor Base Disassembly Attempt](images/base_attempt.jpg)`

---

## 🧰 3. Second Attempt — Dome Section

With the base proving difficult, I turned attention to the **camera dome**.

The **white outer dome** and **black internal casing** were visibly separate components.  
Using a small flathead screwdriver, I carefully pried between the two pieces.  
This revealed a series of internal clips securing the dome in place.  

With steady pressure, each clip released one by one until the white dome detached completely.

*(Insert image of dome separation process here)*  
`![Dome Separation](images/dome_separation.jpg)`

---

## ⚙️ 4. Internal Components & PCB Access

After removing the white dome, the **black inner housing** was exposed.  
This section contained the **motor assembly** and **axle system** that control camera rotation and tilt.

- The **axles** were gently shifted from their slots to free the motor assembly.  
- A few **small screws** were removed to separate the motor from the dome.  
- The **PCB** was located within the black dome, attached via an **8-pin connector**.

The PCB was disconnected by slowly wiggling it loose from the connector, allowing complete removal without damage.

*(Insert image of exposed PCB here)*  
`![Exposed PCB](images/pcb_exposed.jpg)`

---

## 🧠 5. Final Result & Observations

The disassembly successfully isolated the **main PCB** and associated wiring.  
Several key observations were noted:

- The board layout and connector design suggest modular assembly for easy manufacturing.  
- The **motor and power systems** are separate from the camera control board.  
- Some **wiring was intentionally left intact** for later power testing and functionality verification.

The isolated PCB can now be safely analyzed for further research, including pin mapping, firmware reading, and system identification.

*(Insert image of final disassembled components here)*  
`![Final Disassembly](images/final_result.jpg)`

---

## 🧾 Summary

| Component | Description |
|------------|-------------|
| **White Dome** | External shell protecting the lens assembly |
| **Black Housing** | Contains rotation motor and PCB |
| **PCB** | Main logic board with 8-pin connector |
| **Motor Assembly** | Provides pan/tilt functionality |
| **Power Cable** | Connects through base; routed to PCB |

---

## 🧩 Next Steps

- Document PCB pinout and connector layout  
- Identify the microcontroller and flash memory  
- Test power delivery and UART interface  
- Analyze firmware dump for system structure  

---

*Prepared by Jacob Suveges*  
*Date: 11/11/2025*  
