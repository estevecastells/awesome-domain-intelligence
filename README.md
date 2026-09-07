# Awesome Domain Intelligence [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, APIs, datasets and resources for **domain intelligence**: DNS, WHOIS and RDAP, SSL/TLS and certificate transparency, subdomain discovery, domain availability and valuation, email security, typosquatting and brand protection.

Domain intelligence is the practice of turning a domain name into actionable data: who owns it, where it resolves, how it is secured, what else the owner runs, what it is worth, and whether it is being abused. It powers security research, OSINT, due diligence, brand protection and the domain-investing market. This list collects the best tools, APIs, datasets and references in one place.

Contributions are very welcome. Read the [contribution guidelines](CONTRIBUTING.md) first, then open a pull request.

## Contents

- [What Is Domain Intelligence?](#what-is-domain-intelligence)
- [All-in-One Platforms and APIs](#all-in-one-platforms-and-apis)
- [DNS Tools and Lookups](#dns-tools-and-lookups)
- [WHOIS and RDAP](#whois-and-rdap)
- [SSL/TLS and Certificate Transparency](#ssltls-and-certificate-transparency)
- [Subdomain Enumeration](#subdomain-enumeration)
- [Domain Availability, Valuation and Domaining](#domain-availability-valuation-and-domaining)
- [Email Security](#email-security)
- [Typosquatting and Brand Protection](#typosquatting-and-brand-protection)
- [Reputation, Blocklists and Threat Intel](#reputation-blocklists-and-threat-intel)
- [Hosting, IP and ASN](#hosting-ip-and-asn)
- [Technology Detection](#technology-detection)
- [MCP Servers](#mcp-servers)
- [Libraries](#libraries)
- [Datasets](#datasets)
- [Standards and RFCs](#standards-and-rfcs)
- [Learning Resources](#learning-resources)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)
- [License](#license)

## What Is Domain Intelligence?

A domain name is a starting point for a surprising amount of data:

- **DNS**: the records (A, AAAA, MX, TXT, NS, CNAME, CAA) that say where a domain points and how it sends mail.
- **WHOIS / RDAP**: registration data such as registrar, creation and expiry dates and name servers.
- **SSL/TLS**: the certificates a domain serves, their chains, grades and expiry, plus certificate transparency logs.
- **Subdomains**: the wider attack surface and infrastructure behind a single apex domain.
- **Availability and valuation**: whether a name can be registered and what it is worth.
- **Email security**: SPF, DKIM, DMARC and DNSSEC posture.
- **Reputation**: whether a domain is associated with phishing, malware or abuse.

## All-in-One Platforms and APIs

Platforms that combine several of the categories below behind a single API or dashboard. Listed alphabetically.

- [Criminal IP](https://www.criminalip.io/) - Attack-surface search across hosts, domains, certificates and ports.
- [DNSlytics](https://dnslytics.com/) - Domain, IP and provider intelligence with reverse lookups.
- [DomainTools](https://www.domaintools.com/) - WHOIS history, reverse WHOIS, DNS and risk scoring.
- [DomScan](https://domscan.net) - Domain intelligence for developers and AI agents: one API, an MCP server and free tools for availability, DNS, WHOIS/RDAP, SSL, valuation, typosquatting and brand protection.
- [FullHunt](https://fullhunt.io/) - Attack-surface management and discovery.
- [Host.io](https://host.io/) - Domains data API: backlinks, redirects, related domains and DNS.
- [IPinfo](https://ipinfo.io/) - IP and ASN data with domain and hosting context.
- [Netlas](https://netlas.io/) - Internet-wide search across hosts, domains, certificates and WHOIS.
- [SecurityTrails](https://securitytrails.com/) - Current and historical DNS, WHOIS, subdomains and IP data with an API.
- [WhoisXML API](https://www.whoisxmlapi.com/) - WHOIS, DNS, subdomains, IP geolocation and threat-intel APIs and databases.

## DNS Tools and Lookups

Listed alphabetically.

- [Dig Web Interface](https://www.digwebinterface.com/) - Online `dig` across multiple resolvers and record types.
- [DNSChecker](https://dnschecker.org/) - DNS propagation checks across global locations.
- [DNSDumpster](https://dnsdumpster.com/) - Online DNS recon and host discovery.
- [DNSViz](https://dnsviz.net/) - Visual analysis of DNS and DNSSEC configuration.
- [DomScan DNS Lookup](https://domscan.net/tools/dns) - Free DNS record lookup, also available as a [DNS Lookup API](https://domscan.net/dns-lookup-api) and a [propagation checker](https://domscan.net/dns-propagation).
- [Google Public DNS](https://dns.google/) - Web interface for DNS-over-HTTPS lookups.
- [intoDNS](https://intodns.com/) - DNS and mail server health report.
- [MXToolbox](https://mxtoolbox.com/) - DNS, MX, blacklist and email diagnostics.
- [NSLookup.io](https://www.nslookup.io/) - Friendly web DNS lookup.
- [Robtex](https://www.robtex.com/) - DNS, IP and routing research.
- [ViewDNS.info](https://viewdns.info/) - Bundle of DNS, WHOIS and IP tools.

## WHOIS and RDAP

Listed alphabetically.

- [DomScan WHOIS](https://domscan.net/tools/whois) - Free WHOIS lookup, also available as a [WHOIS API](https://domscan.net/whois-api).
- [ICANN Lookup](https://lookup.icann.org/) - Official registration data lookup.
- [RDAP.org](https://about.rdap.org/) - Entry point and bootstrap for the Registration Data Access Protocol.
- [who.is](https://who.is/) - Web WHOIS and domain history.
- [WhoisFreaks](https://whoisfreaks.com/) - WHOIS, reverse WHOIS and DNS APIs and datasets.
- [Whoisology](https://whoisology.com/) - Historical WHOIS and reverse WHOIS.

## SSL/TLS and Certificate Transparency

Listed alphabetically.

- [Censys Search](https://search.censys.io/) - Internet-wide host and certificate search.
- [Cert Spotter](https://sslmate.com/certspotter/) - Certificate transparency monitoring by SSLMate.
- [CertStream](https://certstream.calidog.io/) - Real-time certificate transparency log stream.
- [crt.sh](https://crt.sh/) - Search certificate transparency logs.
- [DomScan SSL Tools](https://domscan.net/tools/ssl) - Free SSL checks with APIs for [audit](https://domscan.net/ssl-audit-api), [chain](https://domscan.net/ssl-chain-api), [grade](https://domscan.net/ssl-grade-api), [expiry](https://domscan.net/ssl-expiry-check-api) and [deep scan](https://domscan.net/ssl-deep-scan-api).
- [Hardenize](https://www.hardenize.com/) - Web and email security posture report.
- [SSL Labs](https://www.ssllabs.com/ssltest/) - Deep TLS configuration analysis and grading.
- [testssl.sh](https://testssl.sh/) - Command-line tool to test TLS/SSL on any port.

## Subdomain Enumeration

Listed alphabetically.

- [Amass](https://github.com/owasp-amass/amass) - In-depth attack-surface mapping and asset discovery.
- [assetfinder](https://github.com/tomnomnom/assetfinder) - Find domains and subdomains related to a target.
- [Chaos](https://chaos.projectdiscovery.io/) - Public dataset of subdomains for bug-bounty programs.
- [DomScan Subdomains](https://domscan.net/tools/dns) - Subdomain discovery as part of domain recon.
- [Findomain](https://github.com/Findomain/Findomain) - Fast cross-platform subdomain enumerator.
- [Subfinder](https://github.com/projectdiscovery/subfinder) - Fast passive subdomain enumeration.
- [Sublist3r](https://github.com/aboul3la/Sublist3r) - Subdomain enumeration using search engines and sources.

## Domain Availability, Valuation and Domaining

Listed alphabetically.

- [Domainr](https://domainr.com/) - Fast domain availability and discovery by API or web.
- [DomScan Domain Checker](https://domscan.net/tools/domain-checker) - Free availability checks, [valuation](https://domscan.net/domain-valuation) and [name suggestions](https://domscan.net/tools/suggestions).
- [DropCatch](https://www.dropcatch.com/) - Expired domain backordering and auctions.
- [Estibot](https://www.estibot.com/) - Domain appraisal and research for investors.
- [Expired Domains](https://www.expireddomains.net/) - Search expiring and deleted domains.
- [Instant Domain Search](https://instantdomainsearch.com/) - Fast availability search.
- [NameBio](https://namebio.com/) - Historical domain sales data.
- [Vacato](https://vacato.io) - RDAP domain availability watchlist with Telegram/email/Slack alerts when a name looks available; free 10 domains (not a drop-catcher).

## Email Security

Listed alphabetically.

- [DMARCLY](https://dmarcly.com/tools) - Free SPF, DKIM and DMARC checkers.
- [dmarcian](https://dmarcian.com/) - DMARC inspection, deployment and reporting.
- [DomScan DNS Security](https://domscan.net/dns-security) - SPF, DKIM, DMARC and DNSSEC checks.
- [EasyDMARC](https://easydmarc.com/tools) - Free email-security analyzers.
- [Google Admin Toolbox](https://toolbox.googleapps.com/apps/checkmx/) - Check MX and mail configuration.
- [Hardenize](https://www.hardenize.com/) - Combined web and email security posture report.
- [MXToolbox SuperTool](https://mxtoolbox.com/SuperTool.aspx) - SPF, DKIM, DMARC and blacklist checks.

## Typosquatting and Brand Protection

Listed alphabetically.

- [dnstwist](https://github.com/elceef/dnstwist) - Detect typosquatting, phishing and brand-impersonation domains.
- [DomScan Typosquatting](https://domscan.net/tools/typosquatting) - Generate and check look-alike domains.
- [DNSTwister](https://dnstwister.report/) - Web service to monitor typo variants of a domain.
- [URLCrazy](https://github.com/urbanadventurer/urlcrazy) - Generate and test domain typo variations.

## Reputation, Blocklists and Threat Intel

Listed alphabetically.

- [AbuseIPDB](https://www.abuseipdb.com/) - Community database of abusive IPs and domains.
- [DomScan Security Tools](https://domscan.net/tools/security) - Domain reputation and security checks.
- [Google Safe Browsing](https://transparencyreport.google.com/safe-browsing/search) - Check whether a site is flagged as unsafe.
- [PhishTank](https://www.phishtank.com/) - Community phishing URL database.
- [Spamhaus](https://www.spamhaus.org/) - Domain and IP blocklists.
- [Talos Intelligence](https://talosintelligence.com/) - Cisco reputation lookup for domains and IPs.
- [URLhaus](https://urlhaus.abuse.ch/) - Database of malicious URLs and domains.
- [urlscan.io](https://urlscan.io/) - Scan and analyze websites and the resources they load.
- [VirusTotal](https://www.virustotal.com/) - Analyze domains, URLs, IPs and files across many engines.

## Hosting, IP and ASN

Listed alphabetically.

- [BGP.he.net](https://bgp.he.net/) - ASN, prefix and peering data from Hurricane Electric.
- [bgpview.io](https://bgpview.io/) - ASN, IP and BGP route lookups.
- [DomScan IP Lookup](https://domscan.net/ip-lookup-api) - IP intelligence and hosting detection, plus a [MAC lookup](https://domscan.net/mac-address-lookup-api).
- [ipdata](https://ipdata.co/) - IP geolocation and threat data API.
- [Shodan](https://www.shodan.io/) - Search engine for internet-connected hosts and services.

## Technology Detection

Listed alphabetically.

- [BuiltWith](https://builtwith.com/) - Web technology profiler and lead data.
- [DomScan Company Lookup](https://domscan.net/company-lookup-api) - Company and organization data behind a domain.
- [Wappalyzer](https://www.wappalyzer.com/) - Identify technologies used by a website.
- [WhatRuns](https://www.whatruns.com/) - Browser extension that detects website technologies.

## MCP Servers

Model Context Protocol servers that expose domain intelligence to AI assistants. Listed alphabetically.

- [DomScan MCP](https://domscan.net) - MCP server for DNS, WHOIS/RDAP, SSL, subdomains, valuation, availability and brand protection.
- [mcp-dnstwist](https://github.com/BurtTheCoder/mcp-dnstwist) - MCP server wrapping dnstwist for typosquatting detection.
- [Model Context Protocol](https://modelcontextprotocol.io/) - The open standard for connecting AI assistants to tools and data.

## Libraries

Listed alphabetically.

- [c-ares](https://github.com/c-ares/c-ares) - Asynchronous DNS resolver library in C.
- [dnspython](https://github.com/rthalley/dnspython) - DNS toolkit for Python.
- [hickory-dns](https://github.com/hickory-dns/hickory-dns) - DNS client, resolver and server in Rust (formerly trust-dns).
- [ldns](https://www.nlnetlabs.nl/projects/ldns/about/) - DNS library in C from NLnet Labs.
- [miekg/dns](https://github.com/miekg/dns) - DNS library for Go.
- [python-whois](https://github.com/DannyCork/python-whois) - WHOIS lookups and parsing in Python.
- [whois-parser](https://github.com/likexian/whois-parser) - WHOIS parser for Go.
- [whoiser](https://github.com/LayeredStudio/whoiser) - Modern WHOIS and RDAP client for Node.js.

## Datasets

Listed alphabetically.

- [Common Crawl](https://commoncrawl.org/) - Open web crawl corpus useful for domain and link analysis.
- [CZDS](https://czds.icann.org/) - ICANN Centralized Zone Data Service for gTLD zone files.
- [DomScan Datasets](https://domscan.net/tools) - Downloadable [WHOIS](https://domscan.net/datasets/whois-database), [WHOIS history](https://domscan.net/datasets/whois-history-database), [reverse WHOIS](https://domscan.net/datasets/reverse-whois-database), [DNS](https://domscan.net/datasets/dns-database), [SSL](https://domscan.net/datasets/ssl-certificates-database), [IP WHOIS](https://domscan.net/datasets/ip-whois-database), [ASN WHOIS](https://domscan.net/datasets/asn-whois-database) and [free email domains](https://domscan.net/datasets/free-email-domains-database) databases.
- [OpenINTEL](https://www.openintel.nl/) - Long-running active DNS measurement dataset.
- [Rapid7 Open Data](https://opendata.rapid7.com/) - Internet-wide scan datasets including DNS and certificates.
- [Tranco List](https://tranco-list.eu/) - Research-grade ranking of the most popular domains.

## Standards and RFCs

Listed by number.

- [RFC 1034 / 1035](https://www.rfc-editor.org/rfc/rfc1035) - Domain names: concepts, facilities and implementation.
- [RFC 4033-4035](https://www.rfc-editor.org/rfc/rfc4033) - DNS Security Extensions (DNSSEC).
- [RFC 6376](https://www.rfc-editor.org/rfc/rfc6376) - DomainKeys Identified Mail (DKIM).
- [RFC 6962](https://www.rfc-editor.org/rfc/rfc6962) - Certificate Transparency.
- [RFC 7208](https://www.rfc-editor.org/rfc/rfc7208) - Sender Policy Framework (SPF).
- [RFC 7489](https://www.rfc-editor.org/rfc/rfc7489) - DMARC.
- [RFC 9083](https://www.rfc-editor.org/rfc/rfc9083) - JSON responses for RDAP.

## Learning Resources

Listed alphabetically.

- [Cloudflare Learning: What is DNS?](https://www.cloudflare.com/learning/dns/what-is-dns/) - Approachable DNS primer.
- [DNS for Rocket Scientists](https://www.zytrax.com/books/dns/) - Free, in-depth DNS reference.
- [DomScan Blog](https://domscan.net/blog) - Guides on DNS, WHOIS, SSL and domain intelligence.
- [How DNS Works (comic)](https://howdns.works/) - Friendly illustrated DNS explainer.
- [RIPE NCC Academy](https://academy.ripe.net/) - Free courses on DNS, routing and internet infrastructure.

## Related Awesome Lists

- [awesome-ai-search](https://github.com/estevecastells/awesome-ai-search)
- [awesome-dns](https://github.com/SoylentBob/awesome-dns)
- [awesome-osint](https://github.com/jivoi/awesome-osint)

## Contributing

Found something missing or out of date? Contributions are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) and open a pull request with a public URL and a short, neutral description.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work. See [LICENSE](LICENSE).
