
# **nlsrecon - Subdomain Discovery Tool**

```
 ███▄    █  ██▓      ██████     ██▀███  ▓█████  ▄████▄   ▒█████   ███▄    █
 ██ ▀█   █ ▓██▒    ▒██    ▒    ▓██ ▒ ██▒▓█   ▀ ▒██▀ ▀█  ▒██▒  ██▒ ██ ▀█   █
▓██  ▀█ ██▒▒██░    ░ ▓██▄      ▓██ ░▄█ ▒▒███   ▒▓█    ▄ ▒██░  ██▒▓██  ▀█ ██▒
▓██▒  ▐▌██▒▒██░      ▒   ██▒   ▒██▀▀█▄  ▒▓█  ▄ ▒▓▓▄ ▄██▒▒██   ██░▓██▒  ▐▌██▒
▒██░   ▓██░░██████▒▒██████▒▒   ░██▓ ▒██▒░▒████▒▒ ▓███▀ ░░ ████▓▒░▒██░   ▓██░
░ ▒░   ▒ ▒ ░ ▒░▓  ░▒ ▒▓▒ ▒ ░   ░ ▒▓ ░▒▓░░░ ▒░ ░░ ░▒ ▒  ░░ ▒░▒░▒░ ░ ▒░   ▒ ▒
░ ░░   ░ ▒░░ ░ ▒  ░░ ░▒  ░ ░     ░▒ ░ ▒░ ░ ░  ░  ░  ▒     ░ ▒ ▒░ ░ ░░   ░ ▒░
   ░   ░ ░   ░ ░   ░  ░  ░       ░░   ░    ░   ░        ░ ░ ░ ▒     ░   ░ ░
         ░     ░  ░      ░        ░        ░  ░░ ░          ░ ░           ░
                                      Made by @snillx <3
```

**nlsrecon** is a Bash-based subdomain discovery tool that integrates **Subfinder**, **Findomain**, and **Assetfinder**. Additionally, it uses **httpx-toolkit** to validate the discovered subdomains and expose their status, along with technologies detected on each.

## **Why nlsrecon?**

- **Fast and Efficient:** Runs all three subdomain enumeration tools in one simple script.
- **Comprehensive Results:** Leverages the power of Subfinder, Findomain, Assetfinder, and httpx-toolkit for thorough subdomain discovery and validation.
- **Technology Detection:** Shows the technologies found on each subdomain, such as CMS, web servers, and more.
- **Open-Source:** Free to use and modify.

## **Tools Integrated:**

 You will need to download these tools, in order to run **nlsrecon**.

- **[Subfinder](https://github.com/projectdiscovery/subfinder):** Fast and reliable passive subdomain discovery.
- **[Findomain](https://github.com/Findomain/Findomain):** High-speed subdomain enumeration written in Rust.
- **[Assetfinder](https://github.com/tomnomnom/assetfinder):** A simple tool for discovering subdomains from various public sources.
- **[httpx-toolkit](https://www.kali.org/tools/httpx-toolkit/):** Validates subdomains, checking if they are alive, and exposes useful information about the subdomains like response codes and technologies.

## **Installation Guide**

To install **nlsrecon**, run the following commands:

```bash
git clone https://github.com/Snillx/nlsrecon.git
cd nlsrecon
chmod +x nlsrecon
mv nlsrecon /usr/bin/
```

Now you can run **nlsrecon** from anywhere on your system.

## **Usage**

To discover subdomains, simply run:

```bash
nlsrecon -d <domain>
```

Where `<domain>` is the target domain you want to find subdomains for. The script will also validate the subdomains and provide information such as the HTTP response status and technologies used.

### **Example Result:**

```
https://example.com [200] [Cloudflare, WordPress, PHP]
https://subdomain.example.com [302] [Nginx]
https://other.example.com [403] [Cloudflare]
```

## **Help**

```
Usage: nlsrecon {options}

Options:
 -d, --domain                          Target domain. Ex: "site.com"
 -o, --output                          File name to save output. Ex: "site-subs.txt"
 -v, --verbose                         Show all running tasks. Ex: -d site.com -v
```

