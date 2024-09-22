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