# anime-terminal
<h3 color=green> ani-cli.sh</h3>

This is an original project of pystardust's [ani-cli](https://github.com/pystardust/ani-cli) followed by me ([YogeshLamichhane](https://www.github.com/YogeshLamichhane/))

A cli to browse, watch and download anime.

This tool scrapes the site [gogoanime](https://gogoanime.vc).

## Dependencies

* grep
* curl
* sed
* celluloid
* youtube-dl (not required to watch/only required if you need to download the anime)
  
## Optional Dependency
* git (to clone the script to your machine)

<h4 color=red>install dependencies</h4>
for arch based distros:<code color=yellow>sudo pacman -Sy --needed curl grep sed celluloid</code>
  
for debian based distros: <code color=yellow>sudo apt-get install curl grep sed celluloid</code>

<h4 color=red>install youtube-dl (to download the anime)</h4>
for arch based distros:<code color=yellow>sudo pacman -Sy --needed python python-pip && sudo pip install youtube-dl</code>
  
for debian based distros: <code color=yellow>sudo apt-get install python python-pip && sudo pip install youtube-dl</code>

<h4 color=red>install optional dependency to clone the script</h4>
for arch based distros:<code color=yellow>sudo pacman -Sy --needed git</code>
  
for debian based distros: <code color=yellow>sudo apt-get install git</code>
<h3 color=green>Usage</h3>
get the script in your machine: <code color=yellow>git clone https://github.com/YogeshLamichhane/anime-terminal/</code>

change directory to the directory having anime script:<code color=yellow>cd anime-terminal/</code>

make the script executable: <code color=yellow>chmod +x ani-cli.sh</code>

watch anime:<code color=yellow>./ani-cli.sh <i>"your_query"</i></code>

download anime:<code color=yellow>./ani-cli.sh -d <i>"your_query"</i></code>

resume watching anime:<code color=yellow>./ani-cli.sh -H <i>"your_query"</i></code>

<h3 color=green>Multiple episodes can be viewed/downloaded by giving the episode range like:</h3>

Choose episode [1-13]: 1 6

This would open/download episodes 1 2 3 4 5 6
