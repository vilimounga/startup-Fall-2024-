## GitHub Assignment
- I learned the steps of using git to push and pull code on my local and remote repo.
Here is a simple list of the steps of using Git.
1. git add [filename]
2. git commit -m "what you did"
3. git push
- For getting changes from your remote repo:
1. git fetch
2. git status
3. git pull
- Link to my README.md: https://github.com/vilimounga/startup/blob/main/README.md
## Simon HTML
- HTML is the backbone structure of my web application.
- HTML sets up the structure for the browser so that it can know how to display the text.
- The deploy file is complicated but it pretty much serves my files up to my server.
## Amazon Web Services - Route 53
- Route 53 is the AWS service that handles DNS-related tasks.
- These DNS-related tasks are buying domain names, hosting my domain on AMS DNS servers, and creating DNS records.
- Steps to getting a domain:
1. Go to Route 53
2. Go to Domains > Registered Domains > Register Domain
3. Choose your domain name 
4. Fill out contract information > Complete Order > Check "Hosted Zones"
- Steps to Creating/Managing my DNS records:
1. Go to Route 53 > Hosted Zones on the left menu
2. Create your root domain DNS record > Create record
3. Input public IP address of server > Create records
4. Create DNS record for any subdomain of my root domain > Create record
5. Input public IP address of server
6. Input "*" for any wildcard for any subdomain in the "Record name" box
7. Press Create records
## Caddy
- Caddy is a web service that listens for HTTP requests.
- It serves requested static files or routes request to another web service.
- This is called, "Gateway". It allows me to expose multiple web services through one external web service (Caddy).
- Caddy handles creation and rotation of web certificates. Supports HTTPS
- It serves HTML,CSS, and Javascript filess.
- Caddy also is a gateway for Subdomain requests. (ex.simon.tracktribe.click)
### Configuration file:
- There are 2 links in the Ubuntu user home directory pointing to Caddy files.
- "~/Caddyfile"
- It contains definitions for routing HTTP requests that Caddy receives.
- It determines the location where HTML static files are loaded from.
- It also proxy requests into the 3rd party services used.
### HTML Files:
- "~/public_html"
- This is the directory of files that Caddy serves per requests made to the root of my web server.
## HTTPS, TLS, and web certificates
- HTTPS is a secure connection so that no data is stolen when requests are given or received.
- Transport Layer Security (TLS) is a security protocol that protects data and communication over the internet. It's used to encrypt data between web applications and servers, such as when a web browser loads a website.
- A web certificate, also known as an SSL or TLS certificate, is a digital object that verifies the identity of a website and encrypts data sent between a browser and a server.
## Simon HTML & Deploying Files
- Make sure you have a deployFiles.sh to deploy your files to your server
- The script does three things. Deletes any previous deployment for simon, copies up all of the files found in the project directory, and makes sure Caddy is hosting the files under the simon subdomain of your domain (e.g. simon.yourdomain.click).
- "./deployFiles.sh -k ~/keys/production.pem -h yourdomain.click -s simon" (example of a command prompt for deploying)