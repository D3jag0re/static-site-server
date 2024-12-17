# static-site-server

# simple-monitoring

This is based off the DevOps Roadmap Project [Statis Site Server](https://roadmap.sh/projects/static-site-server)

Setup a basic linux server and configure it to serve a static site. 

This is number 6 of [21 DevOps Projects](https://roadmap.sh/devops/projects) as per roadmap.sh

## Description From Site 

The goal of this project is to help you understand the basics of setting up a web server using a basic static site served using Nginx. You will also learn how to use rsync to deploy your changes to the server.

## Requirements

Here are the requirements for this project:

- [X] Register and setup a remote linux server on any provider e.g. a simple droplet on DigitalOcean which gives you $200 in free credits with the link. Alternatively, use AWS or any other provider.
- [ ] Make sure that you can connect to your server using SSH.
- [ ] Install and configure nginx to serve a static site.
- [ ] Create a simple webpage with basic HTML, CSS and image files.
- [ ] Use rsync to update a remote server with a local static site.
- [ ] If you have a domain name, point it to your server and serve your static site from there. Alternatively, set up your nginx server to serve the static site from the server’s IP address.

You can write a script deploy.sh which when you run will use rsync to sync your static site to the server.

Once you have completed the project, you should have a basic understanding of how to setup a web server using a basic static site served using Nginx. You should also have a basic understanding of how to use rsync to deploy your changes to the server.
## To Run 

- Setup the following repository secrets:
    - DO_TOKEN : Digital Ocean access token
    - DO_SPACES_SECRET_KEY : Digital Ocean spaces secret key (for Terraform state file)
    - DO_SPACES_ACCESS_KEY : Digital Ocean spaces access key (for Terraform state file)
    - DO_SSH_PUBLIC_KEY : Keypair to be used for VM 
    - DO_SSH_PRIVATE_KEY : Keypair to be used for VM

- Run workflow: This will build and install everything, as well as run 1 cpu stress test 


## Notes 

- Going to use terraform to build droplet 
- Going to use GitHub Actions to do all the initial setup

## Lessons Learned

- LL 1