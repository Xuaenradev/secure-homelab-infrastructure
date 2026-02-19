# Nginx Proxy Manager Setup Notes

## Purpose

Nginx Proxy Manager centralizes incoming traffic and routes requests to internal Docker services.

## Configuration Approach

- Only ports 80 and 443 exposed externally
- Each service assigned internal Docker network IP
- SSL certificates managed through NPM interface
- Admin interface restricted

## Benefits

- Reduces exposed services
- Enables SSL management
- Simplifies routing
- Improves infrastructure organization

## Security Practices

- No direct exposure of container ports
- Strong admin credentials
- Internal services bound to Docker network
