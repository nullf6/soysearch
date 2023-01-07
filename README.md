# soysearch
A script that displays gems from booru.soy onto sxiv to select and copy.

## Dependencies:
1. python3
2. BeautifulSoup (bs4)
3. sxiv

## How to use:
1. Add the directories `soysearch/.temp` to your home folder with ```mkdir -p ~/soysearch/.temp```
2. Add script to your path
3. Make the file executable
4. Syntax: `soysearch {page number} {tag1} {tag2} ..... `

## How to copy image from sxiv
1. Open `.config/sxiv/exec/key-handler` and add the following line to your config:
   ```
   "Y")
		xclip -selection clipboard -t image/png -i "$file" ;;
   ```
