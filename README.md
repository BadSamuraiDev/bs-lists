# B'ad Samurai URL, Domain, & File Extension Lists

Various lists for threat hunting, enforcing warnings, blocks or research.

Lists are in Zscaler format to make it clear if it's a subdomain block (leading period) and wildcard after the domain (the /)

|  File  |  Usage | Description  |  Tags  |
|--------|------------------|---------------|--------| 
| [alt-browsers.txt](./alt-browsers.txt) | Block | URL list to alternate browsers including S3s, repos and download locations | browser proxy vpn tor |
| [cloud-ide.txt](./cloud-ide.txt) | Block, Warning | URL list of cloud-based or browser-based IDEs | C2 IDE DLP |
| [email-file-extensions.txt](./email-file-extensions.txt) | Block | File extension list most orgs likely do not want in their SEG | file extension email gateway |
| [file-mirrors.txt](./file-mirrors.txt) | Block | URL list of higher risk 3rd party file mirrors | file filez mirror spyware |
| [living-off-trusted-tunnels.txt](./living-off-trusted-tunnels.txt) | Block | URL list of services often abused | tunnel LOTT LOTS | 
| [login-cloud-service-providers.txt](./login-cloud-service-providers.txt) | Block, Warning | URL of logins to common Cloud Service Providers that may not be authorized in your organization | CSP login CASB DLP | 
| [login-registrar.txt](./login-registrar.txt) | Block | URL list of mostly North American ICANN accredited registrar logins that may not be authorized in your organization | domain ICANN login registrar |
| [geoshitties.txt](./geoshitties.txt) | Block, Warning | URL list of free domain-less web hosting commonly used for phishing and credential harvesting | geocities free hosting phishing credential harvesting |
| [open-redirect.txt](.open-redirect.txt) | Warning | URL list of open redirects commonly abused on legitimate platforms | LOTS redirect URL |
| [pasties.txt](./pasties.txt) | Block | URL list of pastebin clones | pastebin c2 c3 threat malware |
| [sensitive-file-extensions.txt](./sensitive-file-extensions.txt) | Block, Strip | File extension list of common IAC, DevOps and admin where credentials, keys and token may exist | DLP email gateway credential exfil |
