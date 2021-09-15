# anime-terminal

A cli to browse, watch and download anime.

This tool scrapes the site [gogoanime](https://gogoanime.vc).

<h2 color=green>⚠️ Update: the error has been fixed and the script is working fine again. </h2>

## Dependencies

* grep
* curl
* sed
* celluloid
* youtube-dl (not required to watch/only required if you need to download the anime)
  
## Optional Dependency
* git (to clone the script to your machine)

# Installation
<h4 color=red>install dependencies</h4>
for arch based distros:

```
sudo pacman -Sy --needed curl grep sed celluloid
```

for debian based distros:

```
sudo apt-get install curl grep sed celluloid
```

<h4 color=red>install youtube-dl (to download the anime)</h4>
for arch based distros:

```
sudo pacman -Sy --needed python python-pip && sudo pip install youtube-dl
```
  
for debian based distros:

```
sudo apt-get install python python-pip && sudo pip install youtube-dl
```

<h4 color=red>install optional dependency to clone the script</h4>
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

download anime:

```
./anime-terminal -d <your_query>
```

resume watching anime:

```
./anime-terminal -H
```

<h3 color=green>Example: </h3>
<h4 color=purple>Lets take an example of anime called tokyo revengers.</h4>

watch anime: <code color=cyan>./anime-terminal tokyo-revengers</code>

download anime: <code color=cyan>./anime-terminal -d tokyo-revengers</code>

resume watching anime: <code color=cyan>./anime-terminal -H tokyo-revengers</code>

<h3 color=green>Multiple episodes can be viewed/downloaded by giving the episode range like:</h3>

Choose episode [1-13]: <code color=cyan>1 6</code>

This would open/download episodes 1 2 3 4 5 6
