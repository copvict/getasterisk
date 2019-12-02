# getasterisk

Module that takes in user input with a prompt (Sounds similar? Inspired from getpass). TWIST HERE is that, instead of not echoing the input, they are hidden using Asterisk (*). Suitable for inputting passwords on terminal (Linux/macOS) and command prompt (Windows).

## Working

For every character inputted by the user, an asterisk is printed. When any non character key is pressed, the input is ignored and when the backspace is pressed, the asterisk displayed, overwritten with a empty string. When the enter key is pressed, the module returns a string of the user input.

## Known Issues

1. Instance when there is more than one line of input user, when backspace is pressed, it glithes.
2. Once the delete, insert, tab or any of the arrow keys is pressed, it does not take any more inputs. Backspacing works.

## Demo

[![demo](https://asciinema.org/a/QPYNfGscOGxUXWdjCrjtEh98P.svg)](https://asciinema.org/a/QPYNfGscOGxUXWdjCrjtEh98P?autoplay=1)

## Built Using

* [Python](https://www.python.org/)

## Usage

**Download module using pip:**

*Open Terminal(Linux/macOS):*
```
pip3 install getasterisk
```
*Open Command Prompt(Windows):*
```
py -m pip install getasterisk
```

**Install module using pip:**

*getasterisk() takes 1 argument which is the question to be prompt:*
```
import getasterisk

prompt="Password: "
userInput=getasterisk(prompt)

print(userInput)
```
###### Variable "userInput" will have input from user.

## Author

* **Dhivakar Chelladurai** - <img src="https://dhivakar.xyz/images/logo.png" width=12px height=12px > <a href="https://dhivakar.xyz">dhivakar.xyz</a>

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
