# Nginx Proxy Manager

## Overview
Nginx Proxy Manager is a powerful, user-friendly tool for managing reverse proxies and SSL certificates. It provides an intuitive web interface to configure proxy hosts, SSL certificates with Let’s Encrypt, access controls, and more, making it ideal for home servers or small-scale deployments. With this app, you can securely expose your services to the internet without manually editing Nginx configuration files.

## Features
- **Web-Based Management**: Easily configure proxy hosts, redirections, and SSL certificates through a clean dashboard.
- **Automatic SSL**: Generate and renew free SSL certificates via Let’s Encrypt for secure HTTPS connections.
- **Reverse Proxy**: Forward HTTP/HTTPS traffic to other services or containers with minimal setup.
- **Access Controls**: Set up access lists, HTTP/2, HSTS, and user permissions for enhanced security.
- **Database Flexibility**: Uses SQLite by default, with optional support for MySQL, MariaDB, or PostgreSQL.
- **Multi-Platform Support**: Compatible with various architectures (note: some ARM devices may require alternative database images).

## Requirements
- **Docker**: Configured via Docker Compose, included in Runtipi’s deployment.
- **Ports**: Exposes ports 80 (HTTP), 443 (HTTPS), and 81 (admin interface). Ensure these do not conflict with other services (e.g., Runtipi’s Traefik).
- **Storage**: Persistent storage for configuration (`./data`), SSL certificates (`./letsencrypt`), and optional database (`./mysql` for MySQL/MariaDB).
- **Optional Database**: For MySQL/MariaDB setups, use `jc21/mariadb-aria:latest` or `yobasystems/alpine-mariadb` (recommended for ARM devices).

## Installation
1. Deploy the app via your Runtipi app store.
2. Access the admin interface at `http://<your-server-ip>:81`.
3. Log in with default credentials:
   - **Email**: `admin@example.com`
   - **Password**: `changeme`
4. Update the default credentials upon first login.
5. Configure proxy hosts and SSL certificates through the web interface.

## Configuration
- **Docker Compose**: The app uses `jc21/nginx-proxy-manager:latest` with optional database support. Check the `docker-compose.yml` for volume mappings and environment variables.
- **Traefik Integration**: Runtipi uses Traefik as the default reverse proxy. To avoid conflicts, consider remapping Nginx Proxy Manager’s ports (80, 443) or disabling Traefik for specific services.
- **SSL Setup**: Enable Let’s Encrypt for automatic SSL certificate management during proxy host configuration.
- **Database**: SQLite is enabled by default. For MySQL/MariaDB, configure environment variables (e.g., `DB_MYSQL_HOST`, `DB_MYSQL_USER`) in the `docker-compose.yml`.

## Usage
- **Add Proxy Hosts**: Create proxy hosts to forward traffic to other services (e.g., a web server on another container).
- **Secure Services**: Use access lists and SSL settings to restrict access and enhance security.
- **Monitor Traffic**: Optionally integrate with tools like GoAccess for log analysis.

## Notes
- **ARM Compatibility**: If running on ARM devices, use `yobasystems/alpine-mariadb` for MariaDB to avoid issues with `jc21/mariadb-aria`.
- **Port Conflicts**: Ensure ports 80, 443, and 81 are free or remapped to avoid conflicts with other Runtipi apps.
- **Updates**: Regularly check for updates to `jc21/nginx-proxy-manager:latest` to maintain security and performance.

## Resources
- [Official Website](https://nginxproxymanager.com)
- [GitHub Repository](https://github.com/NginxProxyManager/nginx-proxy-manager)
- [Runtipi Documentation](https://runtipi.io)

---

**Version**: Latest (`jc21/nginx-proxy-manager:latest`)  
**Category**: Networking, Proxy  
**License**: MIT  
**Maintained by**: jc21 and the Nginx Proxy Manager community