# B'ad Samurai URL, Domain, & File Extension Lists

Various lists for threat hunting, enforcing warnings, blocks or research.

Lists are in standard domain formats, but sometimes PAN or Zscaler format to make it clear if it's an inclusive subdomain block.

|  File  |  Usage | Description  |  Tags  |
|--------|------------------|---------------|--------| 
| [alt-browsers.txt](./alt-browsers.txt) | Block | URL list to alternate browsers including S3s, repos and download locations | browser proxy vpn tor |
| [chat-hooks.txt](./chat-hooks.txt) | Block | Chat platform hook and API URLs | C2 exfil |
| [cloud-ide.txt](./cloud-ide.txt) | Block, Warning | URL list of cloud-based or browser-based IDEs | C2 IDE DLP |
| [email-file-extensions.txt](./email-file-extensions.txt) | Block | File extension list most orgs likely do not want in their SEG | file extension email gateway |
| [file-mirrors.txt](./file-mirrors.txt) | Block | URL list of higher risk 3rd party file mirrors | file filez mirror spyware |
| [geoshitties.txt](./geoshitties.txt) | Block, Warning | URL list of free domain-less web hosting commonly used for phishing and credential harvesting | geocities free hosting phishing credential harvesting |
| [json-storage.txt](./json-storage.txt) | Block, Warning | URL list of free/low-cost JSON storage aaS - basically JSON pastebins | json free hosting exfil c2 pastebin |
| [living-off-trusted-tunnels.txt](./living-off-trusted-tunnels.txt) | Block | URL list of services often abused | tunnel LOTT LOTS | 
| [login-cloud-service-providers.txt](./login-cloud-service-providers.txt) | Block, Warning | URL of logins to common Cloud Service Providers that may not be authorized in your organization | CSP login CASB DLP | 
| [login-registrar.txt](./login-registrar.txt) | Block | URL list of mostly North American ICANN accredited registrar logins that may not be authorized in your organization | domain ICANN login registrar |
| [online-pdf-editors.txt](./online-pdf-editors.txt) | Block, Warning | URL list of common web-based PDF editors and converters | PDF DLP converter editor |
| [open-redirect.txt](./open-redirect.txt) | Warning | URL list of open redirects commonly abused on legitimate platforms | LOTS redirect URL |
| [pastebins-code.txt](./pastebins-code.txt) | Block | URL list of pastebins aimed at sharing code | pastebin c2 threat malware exposure coding |
| [pastebins.txt](./pastebins.txt) | Block | URL list of pastebin clones | pastebin c2 threat malware exposure |
| [risky-devtools.txt](./risky-devtools.txt) | Block / Warning | URL list of developer tools posing secret exposure and shadow dev risks | coding developer exposure |
| [sensitive-file-extensions.txt](./sensitive-file-extensions.txt) | Block, Strip | File extension list of common IAC, DevOps and admin where credentials, keys and token may exist | DLP email gateway credential exfil |
| [webhooks.txt](./webhooks.txt) | Block | Webhook testing and relay SaaS | exfil webhook |

## Purpose

These lists exist because despite the critical nature of enforcing policy across these objects, vendor-provided categories are too broad or uncategorized. Many small organizations and MSPs do not have the skill, tools, or subscriptions to manage lists themselves, resulting in a widening [Cyber Poverty Line](https://www.cyberpovertyline.org/). The lists are provided as-is open source intelligence (OSINT).  

## Usage

Most of the lists are intended for control policies within an organization or enterprise. These are not intended as pass-through detections in a SIEM, but do work well in a risk-based alerting (RBA) model utilizing scoring on multiple hits in a short period. Because no list is perfect, it's a helpful canary to escalate risky browsing behavior such as a user hunting for an unblocked pastebin, domain registrar or online PDF editor. Unlike indicators of compromise and the pytramid of pain, these are not *threat lists*; most of them are legitimate platforms, SaaS, and tools that are abused. You'll want to check if these lists contain any providers your organization has approved and depends on before implementation.

## Contribution

I haven't made an official doc yet, but it's the usual jam.

## License

Currently MIT. There is no limit to user, practitioner, and vendor for individual or commercial purposes. These lists are only suggestions to mitigate potential risks in an organization. It is not an industry standard or best practice--but a __default deny__ is.
