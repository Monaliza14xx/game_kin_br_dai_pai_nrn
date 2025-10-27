# ກິນບໍ່ໄດ້ໄປນອນ - Web Game

This is a simple, mobile-friendly web-based version of the popular party drinking game, King's Cup (also known as Circle of Death, Ring of Fire, etc.). It's built entirely within a single HTML file using Tailwind CSS for styling and vanilla JavaScript for the game logic.

## 🍻 Features

* **Card Drawing:** Tap the card deck to draw a card.

* **Rules Popup:** Displays the rule associated with the drawn card.

* **Player Setup:** A welcome modal allows setting the number of players and their names.

* **Drink Counter:** Buttons appear for each player to track how many drinks they've taken.

  * **Tap:** Increase drink count by 1.

  * **Press & Hold (2s):** Decrease drink count by 1 (if > 0).

* **Special Rules:**

  * **10 & Jack:** Trigger a dice roll (2-12). A result of 6 or higher means the player (or their chosen friend for Jack) drinks.

  * **General Rules:** Includes reminders about keeping fists closed and the bathroom rule.

* **Multi-language Support:** Currently supports Lao (Default), English, Japanese, and Thai. Language can be changed via a dropdown menu.

* **Rule Customization:** A settings modal allows players to view and edit the text for each card's rule and description. Changes are saved locally in the browser.

* **Game Over Summary:** When the deck is empty, a summary modal shows the final drink count for each player, ranked.

* **Responsive Design:** Looks and works great on mobile devices and desktops.

* **Accessibility:** Supports keyboard navigation (Tab to focus, Enter/Space to draw).

* **No External Dependencies (besides fonts/Tailwind CDN):** Runs directly in the browser.

## ▶️ How to Play

1. **Save the Code:** Copy the entire content of the `kings-cup.html` file.

2. **Create File:** Paste the code into a new text file and save it with an `.html` extension (e.g., `kings-cup-game.html`).

3. **Open in Browser:** Open the saved HTML file in your web browser (on your computer or phone).

4. **Setup:**

   * The welcome modal will appear first.

   * Adjust the number of players using the +/- buttons.

   * Enter the names for each player.

   * Optionally check "Do not show this again" to skip setup next time (until you reset).

   * Click "Start Game".

5. **Gameplay:**

   * Tap the card (which shows the card back) to draw.

   * The card will flip, and a modal will appear showing the rule.

   * If it's a 10 or Jack, press the "Roll Dice" button.

   * Press "Got it" to close the modal and flip the card back.

   * Use the player buttons at the bottom to track drinks.

   * Use the navigation buttons (Rules, Settings, Language) as needed.

6. **End Game:** When the deck is empty, the summary modal appears. Click "Play Again" to reset the game and start over from the setup screen.

## 🛠️ Technology Used

* **HTML:** Structure of the game.

* **Tailwind CSS (CDN):** For styling and layout.

* **Vanilla JavaScript:** Game logic, DOM manipulation, event handling, and internationalization (i18n).

* **Google Fonts:** Noto Sans Lao Looped and Inter fonts.

* **LocalStorage:** To save language preference, customized rules, and the "skip welcome" setting.