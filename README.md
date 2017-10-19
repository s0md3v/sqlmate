# sqlmate
<img src='https://i.imgur.com/iXwyVul.png' />
A friend of SQLmap which will do what you always expected from SQLmap.

## What it does?
- Feed it a SQL injection dork via <b>--dork</b> option and it will find vulnerable sites for you. After that, it will try to find their admin panels and also try to bypass them with SQL queries.

- It can do very fast hashlookup for MD5, SHA1 and SHA2. You can supply a hash with <b>--hash</b> option.

- You can also supply it a txt file containing hashes to be cracked with <b>--list <path></b> option.
  
- The first mode just checks for 13 most common admin panel locations but if you feed a website through <b>--admin</b> option, you can do a full scan using 482 paths.

### Screenshots
<img src='https://i.imgur.com/ww2zupy.png' />
<img src='https://i.imgur.com/JUKq68V.png' />
<img src='https://i.imgur.com/itjrbrH.png' />
<img src='https://i.imgur.com/IxFbg8G.png' />

#### Requirements
  - Mechanize
  - BeautifulSoup
  - requests

#### Want to contribute?
Alright jump in! Help me add these features:
- [ ] Avoiding duplicates in dork scan results
- [ ] Feature to dump latest dorks
- [ ] A list of examples of sqlmap commands demonstrating some useful and less known sqlmap options
- [ ] Whatever you like

Thats all for now
