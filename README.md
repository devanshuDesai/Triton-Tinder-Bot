# Triton-Tinder-Bot

A Tinder bot to Swipe Right for Cardi B.

## FAQ

### Q. But.. But... This bot is going to get us disqualified!?
A. This bot extensively uses randomization wherever possible. Specifically, there are are three areas where decisions are made randomly:

* **Choosing your GPS co-ordinates :** The guidelines require the user to swipe on campus. Thus, the bot **randomly** chooses a pair of latitude and longitude to spoof your location from a possible combination of **100 million possible co-ordinates on campus**.

* **Choosing when to swipe right :** The bot uses a weighted probablity distribution model to "know" when to swipe right. As a result, the bot **randomly swipes right on 9/10 users** while swiping left on others.

* **Choosing the time between swipes :** After randomly swiping left/right on a user, the bot **randomly waits between 5-15 seconds** before moving to the next user. This gives it a very human feel.

Admittedly no system can be perfect, but this bot has a reasonable number of safeguards against bot detection systems deployed by Tinder. Besides if you have any suggestions on how to make the bot more human-like, I am listening.


## Getting Started

The bot can be used in three easy steps:

1. Create a new real/fake ID on Tinder using **Facebook**, or use a pre-existing ID. (Do not forget to add UC San Diego as the current school on the profile)

2. Get the **Facebook ID** for the Facebook account linked with the Tinder account that you plan on using with the bot. (Refer to 'Prerequisites' to see how to get this)

3. Clone the script onto your computer, modify the credentials in the script with your credentials and run the script.


### Prerequisites

* This package requires a **Python 3.6+** installation on your computer. All the required packages for this script are installed by running the following command on your Terminal:

  ```
  pip install numpy robobrowser
  ```
  ```
  pip install git+https://github.com/charliewolf/pynder
  ```

* **[OPTIONAL]** You will need to create a real/fake Tinder account with a Facebook **email address** and **password** if you do not have a Tinder already, or want to run multiple bots running simultaneously. 
Here's a website that provides temporary email addresses:
  [Guerrila Mail](https://www.guerrillamail.com/) - Temporary Email Address Generator
  
  **Note:** Tinder is known to block new accounts from exotic email addresses like those issued by the above service. If you experience a **Request Error 403**, try using a **Gmail email address** to create your account. 


* You will also need to find the Facebook ID for your account. 
This is a very easy and can be done by copy-pasting your profile URL at the following link:
  [Find my FB ID](https://findmyfbid.com/) - Facebook ID Finder


### Security Note

This is a rather simple script and there is no way for your email address or password to be accessed by anyone except you. That said, it is justified to be paranoid and hence, I suggest using a secondary email address and password for this script.

### Installing

This script is not available as a library yet which means that you will have to clone the repository in the same directory as your Python script.

```
git clone https://github.com/devanshuDesai/Triton-Tinder-Bot
```

### Usage

Open **Terminal** and navigate to the directory where ```Triton-Tinder-Bot``` is saved:

```
cd Triton-Tinder-Bot
```

Open the script with the following command: 

```
open tinder_bot.py
```

Modify ```fb_id```, ```email``` and ```password``` variables with respective values for your Tinder account and **save** it. 

Now, run the script using the following command:

```
python tinder_bot.py
````
**Voila!** Your bot should be up and running.

There's no limit on the number of scripts that you can create as long as you can create enough Tinder/Facebook accounts. Bonus points if you have Tinder+ or Tinder Gold as your bot can keep swiping till the end of time.

## Built With

* [Pynder](https://github.com/charliewolf/pynder) - Python Client for Tinder API


## Authors

* **Devanshu Desai** - *Initial work* - [Devanshu Desai](https://github.com/devanshuDesai)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Known Issues

**This script is known to throw a 403 Error when you use a throwaway email address like: anbds3@xyz.com.**

This occurs because Tinder has built-in security measures to protect it against bots using temporary email addresses like the one I listed above. I am unable to come up with a workaround for this problem in such a short time, which means that you will have to use a large service like Gmail for your account. I am actively looking to resolve this problem, and if you have a solution to this, I'd be glad to merge your solution.

## Note

* Please report any bugs/fixes/improvements that you find. I am listening and eager to make this library as functional and easy-to-use as possible.

* I am actively looking to make this script accessible to all. If you can help me set up a simple website where users can enter their email address and password and the bot does the rest, please hit me up.

* This bot is not affiliated or endorsed by The Reagents of University of California in any way.
