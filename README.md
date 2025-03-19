# cowquote
Using the wonderful cowsay to give you a quote every time you open a terminal window. 

## Installation

If you are using linux, or another unix-like system, follow the instructions below to install and setup. If you are not using linux or another unix-like system, first change operating systems to something more reasonable, then come back to this guide.

### Prerequisites

Cowquote requires the ubiquitous "cowsay" to work. If you are on Ubuntu, use the following command to install. If not, use whichever installation method works on your distro to install cowsay.

```
sudo apt install cowsay
```

Git is optional, but makes the installation slightly faster. Also, git is wonderful, so maybe install it anyways.

```
sudo apt install git
```

### Downloading cowquote

If, as recommended, you installed git, use the following command to install cowsay. I have it in my home directory (`cd` to get there), but I know everyone organizes their directories a little differently, so wherever you please. 

```
git clone https://github.com/DaeganBrown/cowquote.git
```

If you did not install git, and being quite disagreeable, refuse to, then simply download the .zip file from [this](https://github.com/DaeganBrown/cowquote) link, that is, the website you are currently reading this README on, unless you've already downloaded it. Why are you reading this otherwise? Odd choice. 

Then simply unzip that file in your home directory. 

### Setting up your system

The following lines need to be put in your .bashrc file, or equivalent, if you are not using bash. Note that the file path needs to match where you downloaded cowquote, these are simply the commands if you used the home directory. These commands add lines to the bottom of your .bashrc, but anywhere in the .bashrc should work. 

```
echo '# Setup cowquote:' >> .bashrc
echo 'export PATH="$HOME/cowquote:$PATH"' >> .bashrc
echo 'cowquote' >> .bashrc
```

## Usage

Now, every time you open or resource a terminal, it will give you a random quote in the cowsay format! To call another quote, either re-source bash, or use the command `cowquote`. If you have any permissions denied errors, change the permissions. If you don't know what that means, run the command `sudo chmod +e cowquote/cowquote`. If you trust me, that is. 

### Adding more quotes

As of writing this, there are 56 quotes. I have some empty space there, as well as a default case, for any who wish to add their own quotes. I will also be periodically adding more quotes as they are given to me or as I find them, so be sure to check up on the repo every now and then. 

### Suggesting more quotes, or other changes

If you have a quote you would like to see added to the repo for everyone, raise an issue on this repo with your recommendation. If I like it, I will add it. 

If you have other issues, please feel free to let me know! I appreciate any and all feedback, and might even take feedback into consideration. 

## Current Things being worked on

- [x] Licensing
- [x] Fixing string formatting to prevent irregular display
- [ ] More quotes, always
- [ ] Potential config to change cow into other avatars

## License

This is intended as an open source project. It has the MIT license, so you can use it as you want, with attribution.