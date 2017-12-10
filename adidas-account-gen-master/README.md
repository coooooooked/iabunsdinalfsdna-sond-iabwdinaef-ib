# Adidas Account Generator

## Description
A tool coded in Python that allows the user to generate accounts for Adidas US or Adidas UK using a catch-all domain (support for gmail tricks coming soon!). The tool supports the recent captcha requirement change by Adidas.  Accounts are created in the format `PREFIX-RANDOMNUMBER@DOMAIN` with a random password. The prefix and domain can be edited in `config.json`.

## Requirements
- Python 3+
- `requests`
- `bs4`
- `flask`
- `colorama`
- `termcolor`

## Installation and Usage
- You need to add the below line to your hosts file (google how to do this if you do not know)
- `127.0.0.1 fuckrsvpkingz.adidas.co.uk`
- Make sure you have installed all of the modules listed above, using `pip install` (or `pip3 install` if you have python2 too) to do so
- Edit `config.json` with a suitable editor e.g. sublime or atom (NOT NOTEPAD)
- `cd` into the directory location
- `python main.py` or `python3 main.py` if you also have python2 installed and added to path
- You must SOLVE CAPTCHAS MANUALLY (one per account you want to create)

## To-Do List
- [X] Add captcha support
- [X] Catch-all domain support
- [X] Random password generation
- [ ] 2captcha support
- [ ] Gmail tricks support
- [ ] Multi-threading
- [ ] Custom password usage

## Notes
- I will push the full version in the next few days, the current version contains some of the code for 2captcha but does not function as it should (some accounts don't actually create) so edit the code at your own risk.
- Try check your email inbox for adidas account creation emails to make sure the accounts are actually being created
- If you choose 100 accounts, be prepared to solve 100 captchas. If you exit the script before all accounts have been created they will NOT be saved
