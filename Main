#include <stdlib.h> 
#include <stdio.h> 
#include <string.h> 
#include <time.h> 
#include "LCD1602.h" 
#include "tsi.h"

int main(void) { const int ROCK = 0; const int PAPER = 1; const int SCISSOR = 2;

TSI_Init();
LCD1602_Init();
LCD1602_Backlight(TRUE);

int human_player;
int pc_player;
int previous_slider_value = -1;

while (1) {
    // Odczyt wartosci slidera
    int slider_value = TSI_ReadSlider();

    // Sprawdzenie zmiany wartosci slidera
    if (slider_value != previous_slider_value) {
        previous_slider_value = slider_value;

        // Ustawienie wartosci gracza w zaleznosci od polozenia slidera
        if (slider_value > 0 && slider_value < 33) {
            human_player = ROCK;
            LCD1602_ClearAll();
            LCD1602_SetCursor(0, 1);
            LCD1602_Print("ROCK");
        } else if (slider_value >= 33 && slider_value < 66) {
            human_player = PAPER;
            LCD1602_ClearAll();
            LCD1602_SetCursor(0, 1);
            LCD1602_Print("PAPER");
        } else if (slider_value >= 66) {
            human_player = SCISSOR;
            LCD1602_ClearAll();
            LCD1602_SetCursor(0, 1);
            LCD1602_Print("SCISSOR");
        }

        // Losowanie
        pc_player = rand() % 3;

        // Tablica
        const char *options_names[] = { "ROCK", "PAPER", "SCISSOR" };

        LCD1602_SetCursor(8, 1);
        LCD1602_Print(options_names[pc_player]);

        // Sprawdzenie wyniku gry i wyswietlenie odpowiedniego komunikatu
        if (human_player == pc_player) {
            LCD1602_SetCursor(5, 0);
            LCD1602_Print("Tie..");
        } else if ((human_player == ROCK && pc_player == SCISSOR) ||
                   (human_player == PAPER && pc_player == ROCK) ||
                   (human_player == SCISSOR && pc_player == PAPER)) {
            LCD1602_SetCursor(5, 0);
            LCD1602_Print("!WIN!");
        } else {
            LCD1602_SetCursor(5, 0);
            LCD1602_Print("LOSE");
        }
    }
}

return 0;

}
