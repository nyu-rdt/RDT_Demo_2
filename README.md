# RDT_Demo
Demo website. Scrapping the old nyu.rdt.engineering.edu thing.

# Running Hugo
To run (assume you noobs run Window), install Chocolatey and then Hugo. On Powershell or Command Line, cd to the directory and run >> hugo server. Then use your favorite browser (not Chrome) and open localhost:1313

For mac, install homebrew. Then brew install hugo. Running hugo server in the hugo directory will start the server on the same 1313 port.

For linux, you should be able to install with a couple different ways (run with hugo server)
1. Snap compatible distributions - snap install hugo
2. Other debian distributions - sudo apt-get install hugo
3. Arch Linux and arch based distributions - sudo pacman -Syu hugo
4. Fedora - sudo dnf install hugo
5. OpenBSD - doas pkg_add hugo (I know not linux)

Also, you can always build from source.

# Customizing
config.toml in the root directory and homepage.yaml in the /data directory is where all the text and images are in. Change text around or put new image in. Hugo will automatically reload the page for you (although this is not always reliable).

## How to add a page
Add page in config.toml (in root directory). Then create a markdown (.md) file in the content directory. This will add a new page to the website and will show up in the directory.

## Changing css/js
themes/omega/assets contains the css and js for the website which can be called in the markdown files of the pages. You can also contain html snippets in the markdown files. You can also change some of the main css colors in /themes/omega/assets/scss/_variables.scss.

## Customizing data
The two places to customize data are the content folder and the data folder. The data folder has yaml files and the content folder has md files. If I wanted to customize the create page for example, I would customize the tile and description in the md file under content, and I would customize the rest in the yaml file under data.
