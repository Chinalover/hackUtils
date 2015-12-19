# hackUtils
It is a hack tool kit for pentest and web security research, which is based on BeautifulSoup bs4 module http://www.crummy.com/software/BeautifulSoup/bs4/. 

Usage: 

    hackUtils.py [options]

Options:

    -h, --help                                  Show basic help message and exit
    -b keyword, --baidu=keyword                 Fetch URLs from Baidu based on specific keyword
    -g keyword, --google=keyword                Fetch URLs from Google based on specific keyword
    -w keyword, --wooyun=keyword                Fetch URLs from Wooyun Corps based on specific keyword
    -j url|file, --joomla=url|file              Exploit SQLi for Joomla 3.2 - 3.4
    -r url|file, --rce=url|file                 Exploit Remote Code Execution for Joomla 1.5 - 3.4.5
    -d site, --domain=site                      Scan subdomains based on specific site
    -e string, --encrypt=string                 Encrypt string based on specific encryption algorithms (e.g. base64, md5, sha1, sha256, etc.)


Examples:

    hackUtils.py -b inurl:www.example.com
    hackUtils.py -g inurl:www.example.com
    hackUtils.py -w .php?id=
    hackUtils.py -j http://www.joomla.com/
    hackUtils.py -j urls.txt
    hackUtils.py -r http://www.joomla.com/
    hackUtils.py -r urls.txt
    hackUtils.py -d example.com
    hackUtils.py -e text

Change Logs:

****2015.12.17****

1. Modify exploit payload for Joomla 1.5 - 3.4.5 - Object Injection Remote Code Execution

****2015.12.16****

1. Add exploit module for Joomla 1.5 - 3.4.5 - Object Injection Remote Code Execution

[!] legal disclaimer: Usage of hackUtils for attacking targets without prior mutual consent is illegal. It is the end user's responsibility to obey all applicable local, state and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program

声明：仅作学习使用，任何人不可用于非法目的，否则一切后果由其本人承担!
