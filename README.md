CPCBOT0
CPCBOT0 is a Python script that reads a JSON file named CPCCOMMS.json and extracts messages that match a specific format. It saves the extracted messages to a new JSON file named PENDING.json, which can be used by another script to create user account tables and CPC unverified tables.

Prerequisites
Before running CPCBOT0, you'll need to have Python installed on your computer. You can download the latest version of Python from the official Python website: https://www.python.org/downloads/

Installation
To use CPCBOT0, simply download the main.py file from this repository and place it in a folder on your computer.

Usage
Place the CPCCOMMS.json file in the same folder as main.py.
Run the main.py script by opening a terminal or command prompt and navigating to the folder where main.py is located. Then, run the following command:
css
Copy code
python main.py
If the script runs successfully, it will output a message indicating that the PENDING.json file has been saved to the directory C:\Users\Eric\PycharmProjects\CPCTABLEBOT.
Message Format
CPCBOT0 expects messages in the following format:

css
Copy code
{
  "time": "2023-04-05 01:21:49",
  "message": "%message%format%",
  "response": "Message received: %message%format%"
}
The script will extract the message and format fields from messages that contain the placeholders %message% and %format%.
