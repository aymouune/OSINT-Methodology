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
    
    [Reddit](https://www.reddit.com/domain/your_domain/)
    
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

7. **Potentially malicious similar domains:** Use `Red Flags` tool to confirm any potentially malicious similar domains, manually confirm them, and use `Virustotal` and `Wayback Machine` to gather more information.

8. **Gathering employees information:** Use `linkedin2username`, `LinkedInt`, `CrossLinked`, `Uhoh365`, and `Apollo tool` to gather employees' names, positions, profile pictures, emails, etc.
    
    [Hunter](https://hunter.io/)
    
    [Phonebook](https://phonebook.cz/)
    
    [Voilanorbert](https://www.voilanorbert.com/)
    
    [Emailhippo](https://tools.emailhippo.com/)
    
    [Email-checker](https://email-checker.net/)
    
    **PowerShell library AADInternals:** `Invoke-AADIntUserEnumerationAsOutsider -UserName "user@company.com"` and `Get-Content .\users.txt | Invoke-AADIntUserEnumerationAsOutsider -Method Normal`


10. **Shodan and Censys results:** Use `metabigor` to gather results from `Shodan` and `Censys API (Python)`.
11. **Extracting dark web information:** Use `digital shadows`, `Flare`, `Dehashed`, and `Crackstation` to extract dark web information.
12. **Extracting malicious reports:** Use `VirusTotal` and `Zone-h` to extract malicious reports.
13. **Google Dorks, GitHub, PasteBin, Wayback machine:** Use these sources to find leaked files.
14. **Extracting Microsoft Azure Information:** Use `AADInternals`, `MXTOOLBOX`, and `Invoke-AADIntReconAsOutsider -DomainName example.com | Format-Table` to extract Microsoft Azure information.
