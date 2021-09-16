# anime-terminal

A cli to browse, watch and download anime.

Watch your favorite anime from linux terminal. You don't need a browser to watch anime now.

This tool scrapes the site [gogoanime](https://gogoanime.vc).

## Dependencies

* grep
* curl
* sed
* celluloid
* youtube-dl (not required to watch/only required if you need to download the anime)
  
## Optional Dependency
* git (to clone the script to your machine)

# Installation
### Install Dependencies

for arch based distros:

```
sudo pacman -Sy --needed curl grep sed celluloid
```

for debian based distros:

```
sudo apt-get install curl grep sed celluloid
```


### Install youtube-dl (only to download the anime)
for arch based distros:

```
sudo pacman -Sy --needed python python-pip && sudo pip install youtube-dl
```
  
for debian based distros:

```
sudo apt-get install python python-pip && sudo pip install youtube-dl
```

### install optional dependency to clone the script
for arch based distros:

```
sudo pacman -Sy --needed git
```
  
for debian based distros:

```
sudo apt-get install git
```

# Usage

get the script in your machine:

```
git clone https://github.com/YogeshLamichhane/anime-terminal/
```

change directory to the directory having anime script:

```
cd anime-terminal/
```

make the script executable:

```
chmod +x anime-terminal
```

watch anime:

```
./anime-terminal <your_query>
```

download anime: (anime will be downloaded in your current/active directory)

```
./anime-terminal -d <your_query>
```

resume watching anime:

```
./anime-terminal -H
```

### If you don't want to change directory and use ./ to execute the script every time, you can move the script to *bin* directory.
```
sudo mv anime-terminal /usr/local/bin/
```
and execute the script from anywhere in the terminal using command `anime-terminal`

### Example:
#### Lets take an example of anime called tokyo revengers.

To watch tokyo revengers: `./anime-terminal tokyo-revengers`

download anime: `./anime-terminal -d tokyo-revengers`

resume watching anime: `./anime-terminal -H tokyo-revengers`

### Multiple episodes can be viewed/downloaded by giving the episode range like:
Choose episode [1-13]: `1 6`

This would open/download episodes 1 2 3 4 5 6.
