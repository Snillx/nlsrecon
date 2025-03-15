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

**nlsrecon** is a Bash-based subdomain discovery tool that integrates **Subfinder**, **Findomain**, and **Assetfinder**. With **nlsrecon**, you can easily discover subdomains for any domain using these powerful tools.

## **Why nlsrecon?**

- **Fast and Efficient:** Runs all three subdomain enumeration tools in one simple script.
- **Comprehensive Results:** Leverages the power of Subfinder, Findomain, and Assetfinder for thorough subdomain discovery.
- **Open-Source:** Free to use and modify.

## **Tools Integrated:**

- **[Subfinder](https://github.com/projectdiscovery/subfinder):** Fast and reliable passive subdomain discovery.
- **[Findomain](https://github.com/Findomain/Findomain):** High-speed subdomain enumeration written in Rust.
- **[Assetfinder](https://github.com/tomnomnom/assetfinder):** A simple tool for discovering subdomains from various public sources.

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

Where `<domain>` is the target domain you want to find subdomains for.

## **Help**

```
Usage: nlsrecon {options}

Options:
 -d, --domain                          Target domain. Ex: "site.com"
 -o, --output                          File name to save output. Ex: "site-subs.txt"
 -v, --verbose                         Show all running tasks. Ex: -d site.com -v
```


