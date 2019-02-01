# devbox

This is a setup for remote developing.
Don't work with t2.micro (low free mem) but with aws t3.small works fine.

I use this first to learn with the strapi nuxt tutorial.
The next step is to make my website with strapi and nuxt.
Target:
* Store and manage data of the website in Strapi
* Export the data from Strapi to Nuxt to make a static fast website.  

```
git clone https://github.com/gstrainovic/devbox.git
docker-compose up -d
```

| Docker        | Subdomain       | Details        |
| ------------- |:--------------  | -------------- |
| Strapi        | strapi.gost.pw  | A headless cms |
| Nuxt          | nuxt.gost.pw    | Static Vue with hot reloading and static website export|
| Theia         | theia.gost.pw   | A IDE like VSCODE. Secured with password with help of traefik. |
| Traefik       | traefik.gost.pw | Connect Docker with different subdomains on port 80 instead of different ports, ideal behind a firewall. The dashboard is also password protected.


