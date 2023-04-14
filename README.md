# OSINT Methodology

This repository contains an OSINT methodology for conducting investigations on a company. The following steps can be used to gather information about a company:

1. **General Information:** Search for any information related to the target company.

    a. Search Engine Operators:
      [Google](https://www.google.com)
      [Duckduckgo](http://duckduckgo.com/)
      [Bing](http://bing.com/)
      [Yandex](http://yandex.com/)
      [Baidu](http://baidu.com/)
    
    b. Advanced Search with Google:
      [Google](https://www.google.com/advanced_search)
      
    c. Search for acquisitions and mergers in articles and news using `dnb Business Directory`:
    
    [D&B](https://www.dnb.com/)

    [Backlinkwatch](https://www.backlinkwatch.com/index.php)

    [Wayback Machine](https://web.archive.org/)

    [AI-HIT](https://www.aihitdata.com/)

    [Open-Corporates](https://opencorporates.com/)

2. **Company's domains:** To find the company's domains, use `SEO Domain Finder` and `Reverse IP Lookup`:

    [Mxtoolbox](https://mxtoolbox.com/)

    [Centralops](https://centralops.net/co/)

    site:company.com -www
    
3. **Company's subdomains:** Use `Sublist3r`, `Amass`, `Security Trails`, `PureDNS`, `Wayback Machine`, and `Certificate-based Censys search` to find the company's subdomains:

    [Securitytrails](https://securitytrails.com/)

    [Wayback Machine](http://web.archive.org/)

    [Censys](https://search.censys.io/) Search using both `Hosts` and `Certificate`.

    [Builtwith](https://builtwith.com/)

    [crt.sh](https://crt.sh/)

    [pentest-tools](https://pentest-tools.com/)

    [phonebook](https://phonebook.cz/)

    [Reddit](https://www.reddit.com/domain/) `https://www.reddit.com/domain/your_domain/` : replace `your_domain` with your domain

    [Namech_k](https://namechk.com/)

    **Subdomain's check:** Visit the subdomains to gather more information.

4. **Retrieving IPs:** Use `nslookup` command on the domains and subdomains as well as some sites like :

    [Centralops](https://centralops.net/co/) Domain --> DNS records

    [Dnslytics](https://dnslytics.com/reverse-ip)

    [Spyonweb](https://spyonweb.com/) IP address --> Domain name

    [Viewdns](https://viewdns.info/)

5. **Retrieving ASN:** You can get the `ASN` number using this tool:

    [ASN Lookup](https://hackertarget.com/as-ip-lookup/)

6. **Retrieving Technologies:** Use online tools to retrieve technologies such as CMS.

    [Whatcms](https://whatcms.org/)
    
    [virustotal](https://www.virustotal.com/gui/home/upload)

7. **Potentially malicious similar domains:** Use `Red Flags` tool to confirm any potentially malicious similar domains, manually confirm them, and use `Virustotal` and `Wayback Machine` to gather more information.

8. **Gathering employees information:** Use `linkedin2username`, `LinkedInt`, `CrossLinked`, `Uhoh365`, and `Apollo tool` to gather employees' names, positions, profile pictures, emails, etc.

    A. Gathering employees linkedin accounts :
    
    [linkedin2username](https://github.com/initstring/linkedin2username) : `python3 linkedin2username.py -u "your_email@gmail.com" -c "company_identifier"` where the company_identifier is the path to the company's Linkedin account `https://www.linkedin.com/company/company_identifier/`

    [LinkedInt](https://github.com/vysecurity/LinkedInt) : gather linkedin's users infos such as pictures, emails, jobs, locations 

    [CrossLinked](https://github.com/m8sec/CrossLinked) : CrossLinked is a LinkedIn enumeration tool that uses search engine scraping to collect valid employee names from an organization. This technique provides accurate results without the use of API keys, credentials, or accessing LinkedIn directly!

    B. Gathering emails :
    
    [Hunter](https://hunter.io/)

    [Phonebook](https://phonebook.cz/)

    [Voilanorbert](https://www.voilanorbert.com/)

    [Clearbit Connect](chrome.google.com/webstore/detail/clearbit-connect-free-ver/pmnhcgfcafcnkbengdcanjablaabjplo) 
    
    C. Verifing emails :
    
    [Emailhippo](https://tools.emailhippo.com/)

    [Email-checker](https://email-checker.net/)

    [Uhoh365](https://github.com/Raikia/UhOh365) : A script that can see if an email address is valid in Office365. This does not perform any login attempts, is unthrottled, and is incredibly useful for social engineering assessments to find which emails exist and which don't.

    **PowerShell library AADInternals:**
    
    **For one user :** `Invoke-AADIntUserEnumerationAsOutsider -UserName "user@company.com"`

    **For list of users :** `Get-Content .\users.txt | Invoke-AADIntUserEnumerationAsOutsider -Method Normal` 

      
    D. Gathering employees' Accounts :
    
    [Namech_k](https://namechk.com/)

    [whatsmyname](https://whatsmyname.app/)

    [Reddit](https://www.reddit.com/user/) `reddit.com/user/username/` : replace the `username` with your username
    
    E. Gathering  employees' inforamtions : 
    
    Only people living in USA :

    [whitepages](https://www.whitepages.com/) 

    [peekyou](https://www.peekyou.com/) 

    [411](https://www.411.com/)

    [spokeo](https://www.spokeo.com/)

    [thatsthem](https://thatsthem.com/)

    [voterrecords](https://voterrecords.com/) 

    All people :

    [webmii](https://webmii.com/)
    
    F. Gathering Phone numbers :
    
    [truecaller](https://www.truecaller.com/)

    [calleridtest](https://calleridtest.com/)

    [infobel](https://www.infobel.com/fr/world)
    
    
10. **Shodan and Censys results:** Use `metabigor` to gather results from `Shodan` and `Censys API (Python)`.
11. **Extracting dark web information:** Use `digital shadows`, `Flare`, `Dehashed`, and `Crackstation` to extract dark web information.
12. **Extracting malicious reports:** Use `VirusTotal` and `Zone-h` to extract malicious reports.
13. **Google Dorks, GitHub, PasteBin, Wayback machine:** Use these sources to find leaked files.
14. **Extracting Microsoft Azure Information:** Use `AADInternals`, `MXTOOLBOX`, and `Invoke-AADIntReconAsOutsider -DomainName example.com | Format-Table` to extract Microsoft Azure information.
