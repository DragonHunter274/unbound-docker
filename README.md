<p align="center">
    <img src="https://repository-images.githubusercontent.com/440215882/b79c7ae3-c3d4-4a6a-a1d7-d27fa626754b" alt="Logo">
</p>

# Alpine Linux Based DNSSEC Validating Recursive Unbound DNS Resolver Docker Image

[![Build Multiarch Unbound Docker Image](https://img.shields.io/github/actions/workflow/status/madnuttah/unbound-docker/build-unbound.yaml?branch=main&label=madnuttah/unbound%20build%20status&style=flat-square)](https://github.com/madnuttah/unbound-docker/actions/workflows/build-unbound.yaml)
[![GitHub version](https://img.shields.io/github/v/release/madnuttah/unbound-docker?include_prereleases&style=flat-square)](https://github.com/madnuttah/unbound-docker/releases)

This is an actively maintained and trustworthy, lightweight Alpine Linux based Docker image that runs [Unbound](https://unbound.net), an open source high-performance DNS resolver brought to you by the nice people [@NLnetLabs](https://github.com/NLnetLabs) running as **your own** recursive DNS server in a "distroless" scratch image.

<details> 
    
  <summary>Features</summary><br>
    
| Feature                                  | Supported          |
| ---------------------------------------- | ------------------ |
| Minimalist distroless scratch image      | :white_check_mark: |
| Unprivileged user                        | :white_check_mark: |
| Libevent                                 | :white_check_mark: |
| DNSSEC                                   | :white_check_mark: |
| DNSCrypt                                 | :white_check_mark: |
| DNSTap                                   | :white_check_mark: |
| DNS64                                    | :white_check_mark: |
| Draft-0x20 (caps-for-id: yes)            | :white_check_mark: |    
| DNS over HTTPS                           | :white_check_mark: |
| DNS over TLS                             | :white_check_mark: |
| QName Minimization                       | :white_check_mark: |
| Auth. zones with local copy of root zone | :white_check_mark: |
| Aggressive use of DNSSEC-Validated Cache | :white_check_mark: |
| Response Policy Zones                    | :white_check_mark: |
| Redis                                    | :white_check_mark: |
| Python                                   | :x:                |
| EDNS Client Subnet                       | :x:                |
    
</details>

**If you would like to have Unbound statistics, take a look [`here`](https://github.com/madnuttah/unbound-docker-stats)**

## Getting started

Docker containers are most easily used with docker compose.

 - Some [`installation intructions and details`](https://github.com/madnuttah/unbound-docker/blob/main/doc/DETAILS.md)
 - You find example docker-compose files [`here`](https://github.com/madnuttah/unbound-docker/tree/main/doc/examples)
 - There are some scripts in the directory [`scripts`](https://github.com/madnuttah/unbound-docker/tree/main/scripts)
    - `self-build-docker-images.sh` when you want or need to build the docker images yourself

## Available Docker Tags

<details> 
    
  <summary>Tags</summary><br>  
  
   - [1.19.1-2 (latest)](https://hub.docker.com/r/madnuttah/unbound/tags)   
   - [1.19.1-1](https://hub.docker.com/r/madnuttah/unbound/tags)   
   - [1.19.1-0](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.19.0-5](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.19.0-4](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.19.0-3](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.19.0-2](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.19.0-1](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.19.0](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.19.0rc1 (Pre-release)](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.18.0-3](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.18.0-2](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.18.0-1](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.18.0](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.18.0rc1 (Pre-release)](https://hub.docker.com/r/madnuttah/unbound/tags)  
   - [1.17.1-7](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.17.1-6](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.17.1-5](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.17.1-4](https://hub.docker.com/r/madnuttah/unbound/tags)  
   - [1.17.1-3](https://hub.docker.com/r/madnuttah/unbound/tags)  
   - [1.17.1-2](https://hub.docker.com/r/madnuttah/unbound/tags)  
   - [1.17.1-1](https://hub.docker.com/r/madnuttah/unbound/tags)  
   - [1.17.1](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.17.1rc2 (Pre-release)](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.17.1rc1 (Pre-release)](https://hub.docker.com/r/madnuttah/unbound/tags) 
   - [1.17.0-5](https://hub.docker.com/r/madnuttah/unbound/tags) 
   - [1.17.0-4](https://hub.docker.com/r/madnuttah/unbound/tags) 
   - [1.17.0-3](https://hub.docker.com/r/madnuttah/unbound/tags) 
   - [1.17.0-2](https://hub.docker.com/r/madnuttah/unbound/tags) 
   - [1.17.0-1](https://hub.docker.com/r/madnuttah/unbound/tags) 
   - [1.17.0](https://hub.docker.com/r/madnuttah/unbound/tags) 
   - [1.16.3-1](https://hub.docker.com/r/madnuttah/unbound/tags) 
   - [1.17.0rc1 (Pre-release)](https://hub.docker.com/r/madnuttah/unbound/tags)  
   - [1.16.3](https://hub.docker.com/r/madnuttah/unbound/tags)  
   - [1.16.2-1](https://hub.docker.com/r/madnuttah/unbound/tags)  
   - [1.16.2](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.16.1-1](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.16.1](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.16.1rc1-1 (Pre-release)](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.16.1rc1 (Pre-release)](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.16.0-2](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.16.0-1](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.16.0](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.16.0rc1 (Pre-release)](https://hub.docker.com/r/madnuttah/unbound/tags)    
   - [1.15.0-7](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.15.0-6](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.15.0-5](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.15.0-4](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.15.0-3](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.15.0-2](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.15.0-1](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.15.0](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.15.0rc1 (Pre-release)](https://hub.docker.com/r/madnuttah/unbound/tags)
   - [1.14.0](https://hub.docker.com/r/madnuttah/unbound/tags)
    
</details>
    
## Changes
    
You can view the changelogs in the [`Releases`](https://github.com/madnuttah/unbound-docker/releases) section.

## Feedback

I am here to help! Don't hesitate to contact me through a [`GitHub Issue`](https://github.com/madnuttah/unbound-docker/issues) if you have any questions, requests or problems with the image. 

You can also reach me on Fosstodon: 

[![Follow me on Mastodon](https://img.shields.io/mastodon/follow/107779375129112763?domain=https%3A%2F%2Ffosstodon.org%2F&style=social)](https://fosstodon.org/@madnuttah)

## Acknowledgements

- [Alpine Linux](https://www.alpinelinux.org/)
- [Docker](https://www.docker.com/)
- [Unbound](https://unbound.net/)
- [OpenSSL](https://www.openssl.org/)
- [Libevent](https://libevent.org/)
- [Redis](https://redis.io/)
- [Pi-hole](https://pi-hole.net/)
- [StepSecurity](https://www.stepsecurity.io/)
- The many Docker Images which got me inspired
- **Thank you for using my image** ❤️

## Licenses

### License

Unless otherwise specified, all code is released under the MIT license.
See the [`LICENSE`](https://github.com/madnuttah/unbound-docker/blob/main/LICENSE) for details.

### Licenses for other components

- Docker: [Apache 2.0](https://github.com/docker/docker/blob/master/LICENSE)
- Unbound: [BSD License](https://unbound.nlnetlabs.nl/svn/trunk/LICENSE)
- OpenSSL: [Apache-style license](https://www.openssl.org/source/license.html)

## Legal

Please note that this is a work of a private contributor and I'm neither affiliated with NLnet Labs or Pi-hole nor is NLnet Labs or Pi-hole involved in the development of the image. The marks and properties 'Unbound' and 'Pi-hole' are properties of NLnet Labs and Pi-hole respectively. All rights in the source codes, including logos relating to said marks and properties belong to their respective owners.
