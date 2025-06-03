# Rock-Paper-Scissors on FRDM-KL05Z

This project implements a simple "Rock, Paper, Scissors" game using the NXP FRDM-KL05Z development board, a touch slider for user input, and an LCD1602 display for output. The project is designed for the **Keil uVision 5 MDK-ARM** development environment.

## How It Works

- **User Input:** The player selects Rock, Paper, or Scissors by moving their finger across the capacitive touch slider.
- **Display:** The LCD1602 displays both the user's choice and the computer's randomly-selected choice.
- **Result:** The game result ("WIN", "LOSE", or "Tie..") is shown on the LCD screen.

### Hardware

- **Board:** NXP FRDM-KL05Z
- **Display:** LCD1602 (16x2 character LCD)
- **Touch Input:** Onboard TSI (Touch Sensing Input) slider

### Software

- **IDE:** Keil uVision 5 (MDK-ARM)
- **Language:** C
- **Libraries:** LCD1602 and TSI drivers (included in the project)

---

**Author:** Wojciech Hajduk 
**Platform:** NXP FRDM-KL05Z  
**IDE:** Keil uVision 5 MDK-ARM
