# DNSCrypt Server

This app runs a DNSCrypt server using the official `jedisct1/dnscrypt-server` Docker image.

- **Ports:** 443 TCP and UDP
- **Purpose:** Provides encrypted DNS resolution using DNSCrypt protocol.
- **Configuration:** Keys are persisted in `${APP_DATA_DIR}/dnscrypt-server/keys` on the host.
- **Usage:** Enter your server's public IP address or hostname and domain name during setup.

**Note:** Ensure your firewall allows UDP and TCP traffic on port 443.
