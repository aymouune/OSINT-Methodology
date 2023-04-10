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

2. **Company's domains:** To find the company's domains, use `SEO Domain Finder` and `Reverse IP Lookup`:

    [Mxtoolbox](https://mxtoolbox.com/)

    [Centralops](https://centralops.net/co/)
    
    site:company.com -www
    
3. **Company's subdomains:** Use `Sublist3r`, `Amass`, `Security Trails`, `PureDNS`, `Wayback Machine`, and `Certificate-based Censys search` to find the company's subdomains.
5. **Potentially malicious similar domains:** Use `Red Flags Github` to confirm any potentially malicious similar domains, manually confirm them, and use `Virustotal` and `Wayback Machine` to gather more information.
6. **Retrieving IPs:** Use `nslookup/dig` on the subdomains (domains and subdomains) + ASN -> IP addresses to retrieve IPs. Note that they do not 100% belong to the company and may need further confirmation.
7. **Retrieving technologies:** Use `webtech` to retrieve technologies such as CMS.
8. **Manually check the subdomains:** Visit the subdomains manually to gather more information.
9. **Gathering employees information:** Use `linkedin2username`, `LinkedInt`, `CrossLinked`, `Uhoh365`, and `Apollo tool` to gather employees' names, positions, profile pictures, emails, etc.
10. **Shodan and Censys results:** Use `metabigor` to gather results from `Shodan` and `Censys API (Python)`.
11. **Extracting dark web information:** Use `digital shadows`, `Flare`, `Dehashed`, and `Crackstation` to extract dark web information.
12. **Extracting malicious reports:** Use `VirusTotal` and `Zone-h` to extract malicious reports.
13. **Google Dorks, GitHub, PasteBin, Wayback machine:** Use these sources to find leaked files.
14. **Extracting Microsoft Azure Information:** Use `AADInternals`, `MXTOOLBOX`, and `Invoke-AADIntReconAsOutsider -DomainName example.com | Format-Table` to extract Microsoft Azure information.
