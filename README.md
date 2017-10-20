# sqlmate
<img src='https://i.imgur.com/iXwyVul.png' />
There are some features that we think SQLMap should have. Like finding admin panel of the target, better hash cracking etc. If you think the same, SQLMate is for you.

## What it does?
- Feed it a SQL injection dork via <b>--dork</b> option and it will find vulnerable sites for you. After that, it will try to find their admin panels and also try to bypass them with SQL queries.

- It can do very fast hash lookups for MD5, SHA1 and SHA2. You can supply a hash with <b>--hash</b> option. Average lookup takes less than 2 seconds.

- You can also supply it a txt file containing hashes to be cracked with <b>--list <path></b> option.
  
- The first mode just checks for 13 most common admin panel locations but if you feed a website through <b>--admin</b> option, you can do a full scan using 482 paths.

- SQLMate has ability to scrap dorks as well. Specify dumping level via <b>--dump</b> option. Using <b>--dump 1</b> will dump nearly 20 dorks so set the level anywhere between 1-184 as per your needs. SQLMate automatically saves the dorks into a txt file so you can use them later.

Scroll down for more.

### Screenshots
<img src='https://i.imgur.com/8JDL1xt.png' />
<img src='https://i.imgur.com/ww2zupy.png' />
<img src='https://i.imgur.com/itjrbrH.png' />
<img src='https://i.imgur.com/IxFbg8G.png' />

#### Running SQLMate
Enter the following command in terminal to download SQLMate
```
git clone https://github.com/UltimateHackers/sqlmate
```
Then navigate to the sqlmate directory by entering this command
```
cd sqlmate
```
Now install the required modules
```
pip install -r requirements.txt
```
Now run sqlmate
```
python sqlmate
```

##### Available command line options
```
usage: sqlmate [-h] [--dork DORK] [--hash HASH] [--list <path>]
 [--dump 1-184] [--admin URL] [--type PHP,ASP,HTML]

optional arguments:
  -h, --help            show this help message and exit
  --dork DORK           Supply a dork and let SQLMate do its thing
  --hash HASH           'Crack' a hash in 5 secs
  --list <path>         Import and crack hashes from a txt file
  --dump 1-184          Get dorks. Specify dumping level. Level 1 = 20 dorks
  --admin URL           Find admin panel of website
  --type PHP,ASP,HTML   Choose extension to scan (Use with --admin option,
          		Default is all)
```
#### Want to contribute?
Alright jump in! Find bugs or help me add these features:
- [ ] Avoiding duplicates in dork scan results
- [ ] A list of examples of sqlmap commands demonstrating some useful and less known sqlmap options
- [ ] Whatever you like

Thanks for using SQLMate.
