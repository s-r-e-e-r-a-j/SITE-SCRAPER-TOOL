SiteScraper

The Site Scraper Tool is an ethical hacking program developed in Python that enables users to clone websites for educational purposes by copying HTML, CSS, JavaScript, and PHP. **Note:** Use this tool responsibly and only on sites where you have explicit permission, as unauthorized scraping can lead to legal issues.

Use Responsibly


Warning: Use SiteScraper only on websites you own or have explicit permission to test and analyze. Unauthorized use of this tool on external sites without permission may violate laws and terms of service.


Installation

Clone the repository:

```git clone https://github.com/s-r-e-e-r-a-j/SITE-SCRAPER-TOOL.git```



```cd SITE-SCRAPER-TOOL```

``` cd 'Site Scraper' ```

Requirements:

```requests```


```beautifulsoup4```


```argparse```

```os```

Install It By Executing:

```pip3 install requests```

```pip3 install beautifulsoup4```

```pip3 install argparse```

```pip3 install os```

If You Run This Tool any module is missing execute this command on terminal

```pip3 install missingmodulename```

Usage


Run SiteScraper from the command line with the following options:

```python3 sitescraper.py <URL> [options]```


Command-Line Options

Option	Description


```<URL>	The URL of the website to clone```


```-d, --depth (Optional) Set the maximum crawl depth (default: 3)```


```-o, --output	(Optional) Set the output directory (default: website_clone)     you can also specify path to save    example -o /home/kali/Desktop/result    ```



Example

To clone a website up to a depth of 2 and save it in a directory named my_clone:


```python3 sitescraper.py https://example.com -d 2 -o /home/kali/Desktop/my_clone```

Then a directory is inside the my_clone directory the directory name is you provided url

then open the inside directory 

there is a index.html file in it

open it by executing 

```firefox index.html```

then you can see the cloned website

How It Works
SiteScraper follows these steps:

1. Initial Crawl: Downloads the main page of the target site.

 
2.  Recursive Crawling: Finds all internal links, then recursively crawls and saves them.

  
3. Asset Handling: Downloads and saves linked assets (CSS, JS, images).


4. File Structure Preservation: Saves files with the same structure as the original website, maintaining directories and paths.


License


This project is licensed under the MIT License.



