# deploy-certbot

Generate certificates for a domain using certbot/cloudflare-dns.

## Usage

Setup an .env file

```env
CLOUDFLARE_API_TOKEN=
CERTBOT_EMAIL=
CERTBOT_DOMAINS=example1.com,a.example.com
```

1. Provision

```sh
docker compose run --rm certbot-init
```

2. Setup renewal
```sh
docker compose up -d certbot
```