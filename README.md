# NGINX Reverse Proxy Using Docker Compose Example
How it works: Each service has its own docker-compose. All services will join the same docker network for nginx reverse proxy to be able to proxy incoming requests. 

## Adding New Service 
- Service must have docker-compose.yaml 
- Service must join the same network. In this example, the network is `reverse_proxy_default`
- Update nginx.conf in reverse_proxy directory to add the proxy