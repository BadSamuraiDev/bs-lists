# B'ad Samurai URL & Domain Lists

Various lists for threat hunting, enforcing warnings, blocks or research.

Lists are in Zscaler format to make it clear if it's a subdomain block (leading period) and wildcard after the domain (the /)

|  File  |  Usage | Description  |  Tags  |
|--------|------------------|---------------|--------| 
| [alt-browsers.txt](./alt-browsers.txt) | Block | URL list to alternate browsers including S3s, repos and download locations | browser proxy vpn tor |
| [file-mirrors.txt](./file-mirrors.txt) | Block | URL list of higher risk 3rd party file mirrors | file filez mirror spyware |
| [living-off-trusted-tunnels.txt](./living-off-trusted-tunnels.txt) | Block | URL list of services often abused | tunnel LOTT LOTS | 
| [login-cloud-service-providers.txt](./login-cloud-service-providers.txt) | Block, Warning | URL of logins to common Cloud Service Providers that may not be authorized in your organization | CSP login CASB DLP | 
| [login-registrar.txt](./login-registrar.txt) | Block | URL list of mostly North American ICANN accredited registrar logins that may not be authorized in your organization | domain ICANN login registrar |
| [geoshitties.txt](./geoshitties.txt) | Block, Warning | URL list of free domain-less web hosting commonly used for phishing and credential harvesting | geocities free hosting phishing credential harvesting |
| [open-redirect.txt](.open-redirect.txt) | Warning | URL list of open redirects commonly abused on legitimate platforms | LOTS redirect URL |
| [pasties.txt](./pasties.txt) | Block | URL list of pastebin clones | pastebin c2 c3 threat malware |
