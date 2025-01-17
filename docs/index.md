---
title: Ruby Lando Plugin
description: Add a highly configurable ruby service to Lando for local development with all the power of Docker and Docker Compose.
next: ./config.html
---

# Ruby

[Ruby](https://www.ruby-lang.org/en/) A dynamic, open source programming language with a focus on simplicity and productivity. It has an elegant syntax that is natural to read and easy to write.

You can easily add it to your Lando app by adding an entry to the [services](https://docs.lando.dev/core/v3/services/lando.html) top-level config in your [Landofile](https://docs.lando.dev/core/v3).

## Supported versions

*   [3.4](https://hub.docker.com/_/ruby)
*   [3.3](https://hub.docker.com/_/ruby)
*   [3.2](https://hub.docker.com/_/ruby)
*   [3.1](https://hub.docker.com/_/ruby)
*   **[2.7](https://hub.docker.com/_/ruby)** **(default)**
*   [custom](https://docs.lando.dev/core/v3/services/lando.html#overrides)

## Legacy versions

You can still run these versions with Lando but for all intents and purposes they should be considered deprecated (e.g. YMMV and do not expect a ton of support if you have an issue).

*   [3.0](https://hub.docker.com/_/ruby)
*   [2.6](https://hub.docker.com/_/ruby)
*   [2.5](https://hub.docker.com/_/ruby)
*   [2.4](https://hub.docker.com/_/ruby)
*   [2.3](https://hub.docker.com/_/ruby)
*   [1.9](https://hub.docker.com/_/ruby)

Version 2.7 should be considered legacy, but as it has been the default version, we are maintaining support to not break installs where the version is not specified. We recommend specifying a more recent version.

## Patch versions

::: warning Not officially supported!
While we allow users to specify patch versions for this service, they are not *officially* supported, so if you use one, YMMV.
:::

To use a patch version, you can do something as shown below:

```yaml
services:
  myservice:
    type: ruby:3.4.1
```

But make sure you use one of the available [patch tags](https://hub.docker.com/_/ruby/tags) for the underlying image we are using.

