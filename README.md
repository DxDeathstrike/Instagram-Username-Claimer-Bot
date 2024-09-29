
# Instagram Username Claimer Bot

**Overview:** This Python script automates the login process, checks for the availability of specific usernames, and claims them before proceeding to the next account. It utilizes Selenium to interact seamlessly with the Instagram and Meta web pages.

**Note:** The source code for this script will not be made publicly available; however, it can be requested upon direct contact.

![Instagram Username Claimer](https://github.com/user-attachments/assets/bd1b7072-da22-4fd6-95fb-8bb9d1da6332)

## Table of Contents
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [How the Code Works](#how-the-code-works)
- [ChromeDriver Installation](#chromedriver-installation)
- [Contributing](#contributing)
- [Disclaimer](#disclaimer)

## Requirements
- Python 3.x
- Selenium library
- JSON files containing logins and usernames

## Installation

1. **Sharing or Selling without Permission:**
   The selling or sharing of this code without direct permission is prohibited and will be met with concequences

2. **Install required Python libraries:**
   ```bash
   pip install selenium
   pip install pyautogui
   pip install colorama
   pip install keyboard
   pip install pillow
   ```

3. **Download ChromeDriver:**
   - Visit the [ChromeDriver download page](https://chromedriver.chromium.org/downloads).
   - Select the version that matches your installed Chrome version (you can check your Chrome version by going to `chrome://settings/help`).
   - Download the appropriate executable for your OS (Windows, Mac, Linux).
   - Place the `chromedriver.exe` file in the root directory of the project.

## Usage
1. Ensure you have the `usernames.json` and `logins.json` files in the `data` directory, containing usernames you wish to claim and the login details to claim the username respectively.
2. Enter the usernames you wish to claim in `usernames.json`
2. Enter the logins for the accounts to be used to claim usernames in `logins.json`
3. Run the script:
   ```bash
   python main.py
   ```
4. The script will run in a loop,loging into accounts and attempting the usernames and saves any login and usernames claimed to `account_details.txt` in the `data/accounts` directory.
5. Depending on how your computer is set up, it may require some fine-tuning to work such as adjusting the px colour detection and clicking or the xpath values.

## How the Code Works
- The script starts by importing necessary libraries and defining functions.
- It loads usernames and logins from JSON files and sets up a Chrome browser instance using Selenium.
- automating the login, redirection, detection and applying new usernames.
- The script navigates to the meta account page to apply new usernames.
- Once an account claims one of the usernames, it saves the login details and what username it claimed to the account_details.txt .
- Account details are saved in a text file for you to use and see.

## What To Do
To make the script work fully and claim the correct usernames and work, follow these steps:

1. Open the `logins.json` file in a text editor.
2. You will need to enter the account logins in this format, this has to be account email not the username. It will look something like this:
   ```json
   {
    "users": [
        {
            "email": "test@outlook.com",
            "password": "test$"
        },
        {
            "email": "test@outlook.com",
            "password": "test$"
        },
        {
            "email": "test@outlook.com",
            "password": "test$"
        },
        {
            "email": "test@outlook.com",
            "password": "test$"
        },
        {
            "email": "test@outlook.com",
            "password": "test$"
        },
        {
            "email": "test@outlook.com",
            "password": "test$"
        },
        {
            "email": "test@outlook.com",
            "password": "test$"
        },
        {
            "email": "test@outlook.com",
            "password": "test$"
        },
        {
            "email": "test@outlook.com",
            "password": "test$"
        },
        
        {
            "email": "test@outlook.com",
            "password": "test$"
        }
    ]
   }
   ```
3. If you are using only 1 account remove the `,` at the end, If using multiple accounts you should keep the `,` other than the last account.
4. Save the file.
5. Open the `logins.json` file in a text editor.
6. You will need to enter the usernames you wish to claim in this format. It will look something like this:
   ```json
   {
    "users": [
      {"username": "username1"},
      {"username": "username2"},
      {"username": "username3"},
      {"username": "username4"},
      {"username": "username5"},
      {"username": "username6"},
      {"username": "username7"}
    ]
   }

5. Remove the `,` at the end, If using multiple usernames you should keep the `,` other than the last username.
4. Save the file.

## ChromeDriver Installation
To install ChromeDriver for your specific version of Chrome:

1. **Check your Chrome version:**
   - Open Chrome and go to `chrome://settings/help` to find your version number.

2. **Download the matching ChromeDriver:**
   - Visit the [ChromeDriver downloads page](https://chromedriver.chromium.org/downloads).
   - Click on the version that matches your Chrome version.
   - Download the appropriate file for your operating system.

3. **Extract and place the executable:**
   - Extract the downloaded file (if compressed) and place the `chromedriver.exe` in the root directory of your project.

## Contributing
Contributions are welcome! If you have suggestions for improvements or encounter any issues, please open an issue or submit a pull request.

---
## Disclaimer
**Disclaimer:** This bot is intended for educational purposes only. We do not encourage or endorse the misuse of this tool. By using this bot, you acknowledge that you are solely responsible for ensuring compliance with Instagram's terms of service and any applicable laws. We are not liable for any account bans, suspensions, or legal consequences resulting from its use. Use at your own risk.
