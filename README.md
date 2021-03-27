# Sponsor Open Source Tooling

* Feel free to sponsor me for maintaining the tool: https://github.com/sponsors/vysecurity

# Disclaimer

* The project is to be used for educational and testing purposes only.

# Authors

* LinkedInt by Vincent Yiu (@vysecurity): https://www.vincentyiu.com | https://vysecurity.rocks
* Original Scraper by Danny Chrastil (@DisK0nn3cT): https://github.com/DisK0nn3cT/linkedin-gatherer

Contributors:

* Leesoh
* harshil-shah004

# Installation
```
pip install -r requirements.txt
```

# Change Log

**[v1.1 27-03-2021]**

Fixes:
* Fixed the authentication flow
* Fixed hunter API demo key - removed

Additions:
* Added better looking missing image value for the profiles with no photo.
* Embedded all images into the HTML file to allow for offline viewing.
* Added credits

**[v0.1 BETA 12-07-2017]**

Additions:
* UI Updates
* Constrain to company filters
* Addition of Hunter for e-mail prediction

# Usage

1. Put in LinkedIn credentials in LinkedInt.cfg
2. Put Hunter.io API key in LinkedInt.cfg
3. Run LinkedInt.py and follow instructions (example below).

# Example

Using General Motors as the target as they have a bug bounty program.

```
██╗     ██╗███╗   ██╗██╗  ██╗███████╗██████╗ ██╗███╗   ██╗████████╗
██║     ██║████╗  ██║██║ ██╔╝██╔════╝██╔══██╗██║████╗  ██║╚══██╔══╝
██║     ██║██╔██╗ ██║█████╔╝ █████╗  ██║  ██║██║██╔██╗ ██║   ██║
██║     ██║██║╚██╗██║██╔═██╗ ██╔══╝  ██║  ██║██║██║╚██╗██║   ██║
███████╗██║██║ ╚████║██║  ██╗███████╗██████╔╝██║██║ ╚████║   ██║
╚══════╝╚═╝╚═╝  ╚═══╝╚═╝  ╚═╝╚══════╝╚═════╝ ╚═╝╚═╝  ╚═══╝   ╚═╝

Providing you with Linkedin Intelligence
Author: Vincent Yiu (@vysec, @vysecurity)
Original version by @DisK0nn3cT
[*] Enter search Keywords (use quotes for more precise results)
"General Motors"

[*] Enter filename for output (exclude file extension)
generalmotors

[*] Filter by Company? (Y/N):
Y

[*] Specify a Company ID (Provide ID or leave blank to automate):


[*] Enter e-mail domain suffix (eg. contoso.com):
gm.com

[*] Select a prefix for e-mail generation (auto,full,firstlast,firstmlast,flast,first.last,fmlast):
auto

[*] Automatically using Hunter IO to determine best Prefix
[!] {first}.{last}
[+] Found first.last prefix
```

Output (HTML):

![Output HTML Report](asset/htmlreport.png)
