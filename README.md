# certbot-systemd
systemd service for automatic letsencrypt renewals

The timer unit should be enabled.
certbot-users should be copied or created in /etc/ and should list systemd units for anything that uses certbot certificates. Whenever the certificates are renewed, each unit listed will be reloaded or restarted if it is running.
