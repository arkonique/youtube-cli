# youtube-cli

## Dependencies

Requires pip, selenium for python, pyvirtualdisplay,python 2.7, youtube-dl, vlc

All of the abovecan be installed by the following commands:

```bash
sudo apt install youtube-dl
sudo apt-install vlc
sudo apt install python-pip
pip install selenium
pip install pyvirtualdisplay
```

## Setup

Clone this repository: 

```bash
git clone https://github.com/arkonique/youtube-cli
```

Change the permissions for youtube-cli:

```bash
chmod 755 youtube-cli
```

Add chromedriver to the system path:

```bash
sudo cp chromedriver /usr/local/bin
```

That should set up the project

you can optionally add youtube-cli to the system path as well:

```bash
sudo cp youtube-cli /usr/local/bin
```

## Usage

Run youtube-cli along with the  search term:

```bash
./youtube-cli "hello world"
```

If you have added youtube-cli to the system path, you can use:

```bash
youtube-cli "hello world"
```

After displaying the results, you will get a console.

- Press v followed by `:` and a number from the displayed list to view the video in vlc
	eg: 

	```bash
	> v:5
	```

- Press d followed by `:` and a range (beginning-end) or a single number from the displayed list to download the videos using youtube-dl
	eg:

	```bash
	> d:3-5
	> d:4
	```

- Press q to quit

## Todo

- [ ] Add `n` feature to the console to view the next set of results