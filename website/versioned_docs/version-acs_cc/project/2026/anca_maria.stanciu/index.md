# Claw Machine

An arcade claw machine that lets players grab prizes using a custom claw.

:::info

**Author**: Anca-Maria Stanciu \
**Github Project Link**: https://github.com/Anca04/pm-proiect

:::

## Description

The project is an interactive **Claw Machine** designed to grab and move objects. The claw is controlled by the user and can move in three directions: left-right (OX axis), front-back (OY axis) and up-down (OZ axis).

Using a set of buttons, the player moves the claw over a prize, lowers it to grab the object, and then moves it to a special drop area. To make the experience more engaging, the machine includes a custom design with interactive LEDs and a buzzer that provide light and sound feedback during the game. The system automatically detects when a prize is successfully dropped, signaling the end of the round.

## Motivation

The idea for this project started during a brainstorming session with a colleague. It brought back a personal memory from the end of high school when, after finishing my university entrance exam, I played at a claw machine to celebrate. I chose to build this project to recreate that experience.

## Architecture

## Log

### Week 16 - 20 March

Defining the concept of the project and the list of the components.\
Establishing the movement logic for the OX, OY, and OZ axes.\
Researching the necessary limit switches for axis safety and prize detection.\
Creating the initial hardware architecture.

### Week 23 - 27 March

Researching and selecting the stepper motors to ensure the movement of the claw.\
Deciding to use a belt-driven system for precise and smooth axis movement.\
Selecting the appropiate servo motor for the claw's opening and closing mechanism.\
Choosing a button-based interface instead of a joystick to avoid misalignment and ensure precise directional control.\
Finalizing the win-detection logic using a limit switch triggered by the weight of the dropped object.

### Week 30 March - 3 April
Ordering the hardware components and finalizing the Bill of Materials.

## Hardware

### Bill of Materials
 Device                                                                                 | Usage                            | Price                                                                                                                                                             |
| -------------------------------------------------------------------------------------- | -------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Raspberry Pi Pico 2W](https://datasheets.raspberrypi.com/rp2350/rp2350-datasheet.pdf) | The microcontroller | [35 RON ] |
| Stepper Motor and Drivers | Used for precise movement of the claw on the OX, OY, and OZ axes | [16.97 RON](https://www.optimusdigital.ro/ro/motoare-motoare-pas-cu-pas/101-driver-uln2003-motor-pas-cu-pas-de-5-v-.html?search_query=stepper&results=48) x 3 |
| SG90 Servo Motor | Operates the claw's gripping mechanism (opening and closing) | [13.99 RON](https://www.optimusdigital.ro/ro/motoare-servomotoare/26-micro-servomotor-sg90.html?search_query=servo+motor&results=123) |
| Micro Limit Switch | Acts as an endstop for axis safety and detects when a prize is dropped | [5.23 RON](https://sigmanortec.ro/Endstop-mecanic-SS-5GL2-p136284192) x 5 |
| GT2 Timing Belt (6mm) | Transmission belt that converts the stepper motor's rotation into linear movement | [6.70 RON](https://sigmanortec.ro/Curea-GT2-6mm-p125814436) |
| GT2 Timing Pulley - 20 Teeth, 5mm Bore | Mounted on the stepper motors to drive the timing belt precisely | [4.67 RON](https://sigmanortec.ro/Fulie-dintata-GT2-20-dinti-ax-5mm-p125814315) x 5 |
| WS2812B LED Strip | Provides visual feedback and light effects during the game | [3.25 RON](https://sigmanortec.ro/Banda-LED-adresabila-RGB-WS2812-60led-m-IP67-10cm-p166125661) x 2 |
|                                                                                        | Total                            | 222.63 RON                                                                                                                                                        |


## Links

1. https://embedded-rust-101.wyliodrin.com/docs/acs_cc/category/lab
2. https://ai.thestempedia.com/project/diy-candy-claw-machine/
3. https://www.hackster.io/TechGuru/amazing-diy-robotic-gripper-0ead3c
4. https://www.youtube.com/watch?v=xJyjdwXrtXc