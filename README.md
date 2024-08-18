import pyautogui

# Coordinates of the game window
WINDOW_LEFT = 1920
WINDOW_TOP = 1080
WINDOW_WIDTH = 1280
WINDOW_HEIGHT = 720

def hack_the_game():
    # Set the focus to the game window
    pyautogui.moveTo(WINDOW_LEFT, WINDOW_TOP)
    pyautogui.click()

    # Enable invincibility
    pyautogui.typewrite(['[', '/invincible', ' ', '1'])
    pyautogui.hotkey('enter')

    # Enable god mode (unlimited health)
    pyautogui.typewrite(['[', '/god', ' ', '1'])
    pyautogui.hotkey('enter')

    # Enable flying
    pyautogui.typewrite(['[', '/fly', ' ', '1'])
    pyautogui.hotkey('enter')

    # Enable unlimited resources (e.g., infinite ammo)
    pyautogui.typewrite(['[', '/unlimited-resources', ' ', '1'])
    pyautogui.hotkey('enter')

hack_the_game()
