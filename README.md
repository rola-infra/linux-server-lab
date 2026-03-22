Linux Server Lab

Hands-on Linux server setup and debugging on a live VPS (Ubuntu).

What I did

- Set up Nginx with SSL, caching and basic security
- Deployed WordPress manually (no cPanel)
- Configured PHP-FPM and MySQL
- Applied basic server hardening (SSH, UFW, Fail2Ban)

Issues I faced and fixed

- 502 Bad Gateway
  → PHP-FPM was not running / wrong socket
  → Fixed by restarting service and correcting config

- 504 Gateway Timeout
  → PHP response was too slow
  → Adjusted timeout settings

- 403 Forbidden
  → Happened due to missing index file and permission issues
  → Fixed by correcting file and permissions

Stack

Ubuntu, Nginx, PHP 8.3 FPM, MySQL, Let's Encrypt (Certbot)

Notes

This is my practice project where I tested real server issues on a VPS and fixed them.
