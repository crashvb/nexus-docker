# nexus-docker

## Overview

This docker image contains [Nexus](https://www.sonatype.com/nexus-repository-oss).

## Entrypoint Scripts

### nexus

The embedded entrypoint script is located at `/etc/entrypoint.d/10nexus` and performs the following actions:

1. A new nexus configuration is generated.

## Standard Configuration

### Container Layout

```
/
├─ etc/
│  └─ entrypoint.d/
│     └─ 10nexus
├─ usr/
│  └─ share/
│     └─ nexus/
└─ var/
   └─ lib/
      └─ nexus/
```

### Exposed Ports

* `5000/tcp` - docker registry port.
* `8081/tcp` - nexus listening port.

### Volumes

* `/var/lib/nexus` - The nexus data location.

## Development

[Source Control](https://github.com/crashvb/nexus-docker)

