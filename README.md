# Project 5: Two Websites on One EC2

## What I did
Hosted two different websites on the same EC2 server using different ports.

## URLs
- Site 1 (Blue): `http://<ip>/` (port 80)
- Site 2 (Red): `http://<ip>:81/` (port 81)

## Config location
`/etc/nginx/sites-available/default`

## Key learning
- One server can host multiple sites
- Different ports = different entrances
- nginx directs traffic based on port

# Added location blocks in nginx config for / and /site2/
sudo nginx -t
sudo systemctl reload nginx
