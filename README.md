# Awesome Domain Intelligence [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, APIs, datasets and resources for **domain intelligence**: DNS, WHOIS and RDAP, SSL/TLS and certificate transparency, subdomain discovery, domain availability and valuation, email security, typosquatting and brand protection.

Domain intelligence is the practice of turning a domain name into actionable data: who owns it, where it resolves, how it is secured, what else the owner runs, what it is worth, and whether it is being abused. It powers security research, OSINT, due diligence, brand protection and the domain-investing market. This list collects the best tools, APIs, datasets and references in one place.

Contributions are very welcome. Read the [contribution guidelines](CONTRIBUTING.md) first, then open a pull request.

> Maintained by the team behind [DomScan](https://domscan.net). We keep this list neutral and useful; other tools are listed alongside our own on purpose.

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

Platforms that combine several of the categories below behind a single API or dashboard.

- [DomScan](https://domscan.net) - Domain intelligence for developers and AI agents: one API, an MCP server and free tools for domain availability, DNS, WHOIS/RDAP, SSL, valuation, typosquatting and brand protection.
- [SecurityTrails](https://securitytrails.com/) - Current and historical DNS, WHOIS, subdomains and IP data with an API.
- [WhoisXML API](https://www.whoisxmlapi.com/) - WHOIS, DNS, subdomains, IP geolocation and threat-intel APIs and downloadable databases.
- [IPinfo](https://ipinfo.io/) - IP and ASN data with domain and hosting context.
- [Host.io](https://host.io/) - Domains data API: backlinks, redirects, related domains and DNS.
- [Spyse / Criminal IP](https://www.criminalip.io/) - Attack-surface search across hosts, domains, certificates and ports.

## DNS Tools and Lookups

- [DomScan DNS Lookup](https://domscan.net/tools/dns) - Free DNS record lookup; also available as the [DNS Lookup API](https://domscan.net/dns-lookup-api).
- [DomScan DNS Propagation](https://domscan.net/dns-propagation) - Check DNS propagation across global resolvers.
- [DomScan DNS Security](https://domscan.net/dns-security) - Check DNS and email security posture.
- [DNSViz](https://dnsviz.net/) - Visual analysis of DNS and DNSSEC configuration.
- [Dig Web Interface](https://www.digwebinterface.com/) - Online `dig` across multiple resolvers and record types.
- [DNSDumpster](https://dnsdumpster.com/) - Online DNS recon and host discovery.
- [intoDNS](https://intodns.com/) - DNS and mail server health report.
- [MXToolbox](https://mxtoolbox.com/) - DNS, MX, blacklist and email diagnostics.

## WHOIS and RDAP

- [DomScan WHOIS](https://domscan.net/tools/whois) - Free WHOIS lookup; also available as the [WHOIS API](https://domscan.net/whois-api).
- [ICANN Lookup](https://lookup.icann.org/) - Official registration data lookup.
- [RDAP.org](https://about.rdap.org/) - Entry point and bootstrap for the Registration Data Access Protocol.
- [who.is](https://who.is/) - Web WHOIS and domain history.
- [Whoisology](https://whoisology.com/) - Historical WHOIS and reverse WHOIS.

## SSL/TLS and Certificate Transparency

- [DomScan SSL Tools](https://domscan.net/tools/ssl) - Free SSL checks; APIs for [audit](https://domscan.net/ssl-audit-api), [chain](https://domscan.net/ssl-chain-api), [grade](https://domscan.net/ssl-grade-api), [expiry](https://domscan.net/ssl-expiry-check-api) and [deep scan](https://domscan.net/ssl-deep-scan-api).
- [SSL Labs](https://www.ssllabs.com/ssltest/) - Deep TLS configuration analysis and grading.
- [crt.sh](https://crt.sh/) - Search certificate transparency logs.
- [Censys Search](https://search.censys.io/) - Internet-wide host and certificate search.
- [CertStream](https://certstream.calidog.io/) - Real-time certificate transparency log stream.

## Subdomain Enumeration

- [DomScan Subdomains](https://domscan.net/tools/dns) - Subdomain discovery as part of domain recon.
- [Subfinder](https://github.com/projectdiscovery/subfinder) - Fast passive subdomain enumeration.
- [Amass](https://github.com/owasp-amass/amass) - In-depth attack-surface mapping and asset discovery.
- [assetfinder](https://github.com/tomnomnom/assetfinder) - Find domains and subdomains related to a target.
- [crt.sh subdomain search](https://crt.sh/) - Discover subdomains via certificate transparency.

## Domain Availability, Valuation and Domaining

- [DomScan Domain Checker](https://domscan.net/tools/domain-checker) - Free availability checks via [check-domain-availability](https://domscan.net/check-domain-availability).
- [DomScan Valuation](https://domscan.net/tools/valuation) - Domain appraisal, also at [domain-valuation](https://domscan.net/domain-valuation).
- [DomScan Suggestions](https://domscan.net/tools/suggestions) - Domain name ideas and suggestions.
- [Instant Domain Search](https://instantdomainsearch.com/) - Fast availability search.
- [Estibot](https://www.estibot.com/) - Domain appraisal and research for investors.
- [Namebio](https://namebio.com/) - Historical domain sales data.
- [Expired Domains](https://www.expireddomains.net/) - Search expiring and deleted domains.

## Email Security

- [DomScan DNS Security](https://domscan.net/dns-security) - SPF, DKIM, DMARC and DNSSEC checks.
- [MXToolbox SuperTool](https://mxtoolbox.com/SuperTool.aspx) - SPF, DKIM, DMARC and blacklist checks.
- [DMARC Analyzer / dmarcian](https://dmarcian.com/) - DMARC inspection and reporting.
- [Hardenize](https://www.hardenize.com/) - Email and web security posture report.

## Typosquatting and Brand Protection

- [DomScan Typosquatting](https://domscan.net/tools/typosquatting) - Generate and check look-alike domains.
- [dnstwist](https://github.com/elceef/dnstwist) - Detect typosquatting, phishing and brand-impersonation domains.
- [URLCrazy](https://github.com/urbanadventurer/urlcrazy) - Generate and test domain typo variations.

## Reputation, Blocklists and Threat Intel

- [DomScan Security Tools](https://domscan.net/tools/security) - Domain reputation and security checks.
- [VirusTotal](https://www.virustotal.com/) - Analyze domains, URLs, IPs and files across many engines.
- [URLhaus](https://urlhaus.abuse.ch/) - Database of malicious URLs and domains.
- [PhishTank](https://www.phishtank.com/) - Community phishing URL database.
- [Spamhaus](https://www.spamhaus.org/) - Domain and IP blocklists.

## Hosting, IP and ASN

- [DomScan IP Lookup](https://domscan.net/ip-lookup-api) - IP intelligence and hosting detection.
- [DomScan MAC Lookup](https://domscan.net/mac-address-lookup-api) - MAC address vendor lookup.
- [BGP.he.net](https://bgp.he.net/) - ASN, prefix and peering data from Hurricane Electric.
- [bgpview.io](https://bgpview.io/) - ASN, IP and BGP route lookups.
- [Shodan](https://www.shodan.io/) - Search engine for internet-connected hosts and services.

## Technology Detection

- [DomScan Company Lookup](https://domscan.net/company-lookup-api) - Company and organization data behind a domain.
- [Wappalyzer](https://www.wappalyzer.com/) - Identify technologies used by a website.
- [BuiltWith](https://builtwith.com/) - Web technology profiler and lead data.

## MCP Servers

Model Context Protocol servers that expose domain intelligence to AI assistants.

- [DomScan MCP](https://domscan.net) - MCP server for DNS, WHOIS/RDAP, SSL, subdomains, valuation, availability and brand protection.
- [Model Context Protocol](https://modelcontextprotocol.io/) - The open standard for connecting AI assistants to tools and data.

## Libraries

- [dnspython](https://github.com/rthalley/dnspython) - DNS toolkit for Python.
- [miekg/dns](https://github.com/miekg/dns) - DNS library for Go.
- [whois (Python)](https://github.com/DannyCork/python-whois) - WHOIS lookups and parsing in Python.
- [whois-parser (Go)](https://github.com/likexian/whois-parser) - WHOIS parser for Go.
- [whoiser (Node.js)](https://github.com/LayeredStudio/whoiser) - Modern WHOIS and RDAP client for Node.js.

## Datasets

- [DomScan Datasets](https://domscan.net/tools) - Downloadable [WHOIS](https://domscan.net/datasets/whois-database), [WHOIS history](https://domscan.net/datasets/whois-history-database), [reverse WHOIS](https://domscan.net/datasets/reverse-whois-database), [DNS](https://domscan.net/datasets/dns-database), [SSL certificates](https://domscan.net/datasets/ssl-certificates-database), [IP WHOIS](https://domscan.net/datasets/ip-whois-database), [ASN WHOIS](https://domscan.net/datasets/asn-whois-database) and [free email domains](https://domscan.net/datasets/free-email-domains-database) databases.
- [Tranco List](https://tranco-list.eu/) - Research-grade ranking of the most popular domains.
- [Common Crawl](https://commoncrawl.org/) - Open web crawl corpus useful for domain and link analysis.
- [OpenINTEL](https://www.openintel.nl/) - Long-running active DNS measurement dataset.

## Standards and RFCs

- [RFC 1034 / 1035](https://www.rfc-editor.org/rfc/rfc1035) - Domain names: concepts, facilities and implementation.
- [RFC 9083](https://www.rfc-editor.org/rfc/rfc9083) - JSON responses for RDAP.
- [RFC 7489](https://www.rfc-editor.org/rfc/rfc7489) - DMARC.
- [RFC 6797](https://www.rfc-editor.org/rfc/rfc6797) - HTTP Strict Transport Security (HSTS).
- [RFC 6962](https://www.rfc-editor.org/rfc/rfc6962) - Certificate Transparency.

## Learning Resources

- [DomScan Blog](https://domscan.net/blog) - Guides on DNS, WHOIS, SSL and domain intelligence.
- [DNS for Rocket Scientists](https://www.zytrax.com/books/dns/) - Free, in-depth DNS reference.
- [Cloudflare Learning: What is DNS?](https://www.cloudflare.com/learning/dns/what-is-dns/) - Approachable DNS primer.

## Related Awesome Lists

- [awesome-dns](https://github.com/SoylentBob/awesome-dns)
- [awesome-osint](https://github.com/jivoi/awesome-osint)
- [awesome-ai-search](https://github.com/estevecastells/awesome-ai-search)

## Contributing

Found something missing or out of date? Contributions are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) and open a pull request with a public URL and a short, neutral description.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work. See [LICENSE](LICENSE).
