# Southwest Airlines Check in Bot
## Introduction:
If you're reading this, you and I both know Southwest has a horrible check in process. If you want any hope of getting a decent seat, so help you God, you'd better hit that button exactly at the 24h mark. Natrually, the only solution is to embrace our robot overlords and their ever-superior clicking abilities.
    
## The Boring Stuff:
There's an easy way or a hard way to do this. I'd recommend the easy way. Included with this repository is a script to do all the dirty work for you. To use it, run:
```bash
curl -s https://raw.githubusercontent.com/kclejeune/SouthwestBot/master/setup.sh | sh
```
The setup script will install everything you need and then clean up. If you use it, you can skip to The Fun Stuff.
## Manual Install (the REALLY boring stuff):
First, clone the repository.  
```bash
git clone https://github.com/kclejeune/SouthwestBot.git
```
This script requires python 3 and chromedriver. For linux, look at the dependencies; you can figure out the rest with your own package manager of preference. For mac, use homebrew to install these. If you're on a mac and you don't have homebrew, get it:
```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
We'll install chromedriver, python3, and some additional requirements using this:
```bash
brew cask install chromedriver
brew install python
cd ~/SouthwestBot/
pip3 install -r requirements.txt
```
That's it! Now, check out the fun stuff.
## The Fun Stuff:
Now we have everything necessary for this to work. Nice.
To run:
```bash
python3 ~/SouthwestBot/southwest_bot.py
```
Follow the instructions in the script, don't shut down your computer, and you'll be looking at a seat somewhere hopefully other than the very back of your next southwest flight.
