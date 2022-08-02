# dokku-traefik

**traefik load balancer for dokku**

## Installation

Install the plugin:

```bash
dokku plugin:install https://github.com/maayanlab/dokku-traefik.git
```

### Installation Notes

This plugin is currently quite opinionated, requiring letsencrypt and using tlsChallenge.

## Usage

The plugin offers the following commands via the dokku tool:

```
traefik:enable  <app> <port> Expose a port
traefik:disable <app>        Clear configured ports
traefik:list                 Show all configured apps
traefik:start                Start traefik
traefik:restart              Restart traefik
traefik:stop                 Stop traefik
```

To add a port configuration, run the following example command:

```bash
dokku traefik:enable my-app 8080
```

To remove that configuration later, run the following example command:

```bash
dokku traefik:disable my-app
```
