# Triton-Tinder-Bot

A Tinder bot to Swipe Right for Cardi B.

## Getting Started

The bot can be used in three easy steps:

1. Create a new real/fake ID on Tinder using **Facebook**, or use a pre-existing ID. (Do not forget to add UC San Diego as the current school on the profile)

2. Get the **Facebook ID** for the Facebook account linked with the Tinder account that you plan on using with the bot. (Refer to 'Prerequisites' to see how to get this)

3. Import the script ```tinder-bot.py``` and pass **facebook_id, email and password** to the function swipe() and run your Python script. (Preferably, try to run multiple Python scripts simultaneously with different Tinder accounts to maximize the odds for UCSD to win).


### Prerequisites

* This package requires a Python 3.6+ installation on your computer. All the required packages for this script are installed by running the following command on your Terminal:

  ```
  pip install numpy robobrowser
  ```
  ```
  pip install git+https://github.com/charliewolf/pynder
  ```

* You will need to create a real/fake Tinder account with a Facebook **email address** and **password**. 
Here's a website that provides temporary:
  [Guerrila Mail](https://www.guerrillamail.com/) - Temporary Email Address Generator
  
  #### Note:
    Tinder is known to block new accounts from exotic email addresses like those issued by the above service. If you experience a **Request Error 403**, try using a **Gmail email address** to create your account. 

* You will also need to find the Facebook ID for your account. 
This is a very easy and can be done by copy-pasting your profile URL at the following link:
  [Find my FB ID](https://findmyfbid.com/) - Facebook ID Finder


### Security Note

This is a rather simple script and there is no way for your email address or password to be accessed by anyone except you. That said, it is justified to be paranoid and hence, I suggest using a throwaway email address and password through a temporary email service provider.

### Installing

This script is not available as a library yet which means that you will have to clone the repository in the same directory as your Python script.

```
git clone https://github.com/devanshuDesai/Triton-Tinder-Bot
```

### Usage

Once you have completed the above steps, the Python script is fairly easy to write. In fact, you can literally copy-paste the code below and save it with a name of your choice. For the purpose of this "tutorial", I will save my script as ```my_bot_1.py```.

Copy-paste the following code into ```my_bot_1.py``` and replace ```facebook_id```, ```email``` and ```password``` with the values you created/found in the previous steps.

```
from tinder_bot import *
swipe(facebook_id, email, password)
```
That is it! Trust me.

Now, save ```my_bot_1.py``` in the same directory as ```tinder_bot.py```.

Open terminal and navigate to the directory where both ```tinder_bot.py``` and ```my_bot_1.py``` are saved and run the bot by typing the following command into Terminal:

```
python my_bot_1.py
````


There's no limit on the number of scripts that you can create as long as you can create enough Tinder/Facebook accounts. Bonus points if you have Tinder+ or Tinder Gold as your bot can keep swiping till the end of time.

## Built With

* [Pynder](https://github.com/charliewolf/pynder) - Python Client for Tinder API


## Authors

* **Devanshu Desai** - *Initial work* - [Devanshu Desai](https://github.com/devanshuDesai)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Note

Please report any bugs/fixes/improvements that you find. I am listening and eager to make this library as functional and easy-to-use as possible.

This bot is not affiliated or endorsed by The Reagents of University of California in any way.
