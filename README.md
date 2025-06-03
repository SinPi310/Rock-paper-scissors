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

## Getting Started

1. Clone this repository to your PC.
2. Open the project in **Keil uVision 5**.
3. Connect your FRDM-KL05Z board.
4. Build and flash the program to your board.
5. Use the touch slider to play the game and view results on the LCD.

## Video Demonstration

[Watch a demonstration of Rock-Paper-Scissors on FRDM-KL05Z](https://www.youtube.com/watch?v=03m7jN7P4jI)

*(If this is not the exact board, you can find many similar FRDM-KL05Z LCD/TSI demo videos by searching "FRDM-KL05Z LCD TSI" on YouTube.)*

## Screenshots

*(You can add photos or screenshots here of your board in action!)*

---

**Author:** Wojciech Hajduk 
**Platform:** NXP FRDM-KL05Z  
**IDE:** Keil uVision 5 MDK-ARM
