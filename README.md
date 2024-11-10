# TMRXX - Terminal Timer in C

TMRXX is a simple terminal-based countdown timer written in C. It uses ANSI escape codes to clear and center the timer on the terminal screen, allowing for a focused and minimalistic countdown display.

## Features
- **Timer Display:** Shows countdown in HH:MM:SS format, centered on the screen.
- **Input Flexibility:** Set the timer duration via command-line arguments or prompt input.
- **Error Handling:** Notifies user if minutes are outside the valid range.
- **Customizable Screen Splash:** Includes a splash screen that appears at the start of the timer.

## Preview
The program clears the terminal and displays the countdown as `-- HH:MM:SS --`, centered in the terminal window. A `~ Time Over ~` message with a sound alert is shown when the timer ends.

## Usage
### Compile
```bash
gcc -o timer timer.c
```
Run
Using Command-line Arguments:
```
./timer HH MM
```

HH - Hours (0 to 23)
MM - Minutes (1 to 59)

Using Interactive Mode:
```
./timer
```

The program will prompt for timer duration (HH
) and ask for confirmation to start.
Example
```
./timer 0 25
```
This command starts a 25-minute timer in countdown mode.


Additional Notes

    Tested in Linux with a terminal emulator.
    Uses ioctl for dynamic terminal size, so it adjusts to different screen dimensions.


Happy timing! ⏳