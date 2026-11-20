[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]

<!-- PROJECT HEADER -->
<br />
<p align="center">
  <!-- https://github.com/stefanjudis/github-light-dark-image-example -->
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.github.com/Good-Games-Munich/assets/main/logos/GGM_logo_white.png">
    <img alt="Logo" src="https://raw.github.com/Good-Games-Munich/assets/main/logos/GGM_logo_black.png" height="150">
  </picture>

  <h3 align="center">📙 Paperless-ngx</h3>

  <p align="center">
    ·
    <a href="https://github.com/Good-Games-Munich/paperless-ngx/issues">Report Bug</a>
    ·
    <a href="https://github.com/Good-Games-Munich/paperless-ngx/issues">Request Feature</a>
    ·
  </p>
</p>

<!-- ABOUT THE PROJECT -->

## About The Project

Setup for paperless-ngx as document index/archive.

## Setup

### Production

Follow [Creating a release](https://github.com/Good-Games-Munich/.github/wiki/workflows#creating-a-release).

### Development

1. Follow [local setup](https://github.com/Good-Games-Munich/.github/wiki/workflows#local-setup).
2. Follow the [Customization](#customization) section and set all variables with `Required in dev` `true`.
3. Navigate to `http://localhost:3500`

### Customization

Create a environment file `touch .env`. Override variables in the `{variable name}={variable value}` format. All required variables need to be overridden for the respected environment.

| Variable            | Description                                                      | Required in dev | Required in prod | Default value |
| ------------------- | ---------------------------------------------------------------- | --------------- | ---------------- | ------------- |
| `POSTGRES_PASSWORD` | Postgres password. Choose a secure one.                          | `true`          | `true`           | none          |
| `PAPERLESS_HOST`    | URL to be used by the reverse proxy. E.g. `paperless.domain.de`. | `false`         | `true`           | none          |
| `PAPERLESS_SECRET_KEY` | Secret used for cryptographic signing (required since v3). Generate one with `python3 -c "import secrets; print(secrets.token_urlsafe(64))"`. | `true`          | `true`           | none          |

<!-- CONTRIBUTING -->

## Contributing

Follow [contributing](https://github.com/Good-Games-Munich/.github/wiki/workflows#contributing).

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[contributors-shield]: https://img.shields.io/github/contributors/Good-Games-Munich/paperless-ngx.svg?style=flat-square
[contributors-url]: https://github.com/Good-Games-Munich/paperless-ngx/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Good-Games-Munich/paperless-ngx.svg?style=flat-square
[forks-url]: https://github.com/Good-Games-Munich/paperless-ngx/network/members
[stars-shield]: https://img.shields.io/github/stars/Good-Games-Munich/paperless-ngx.svg?style=flat-square
[stars-url]: https://github.com/Good-Games-Munich/paperless-ngx/stargazers
[issues-shield]: https://img.shields.io/github/issues/Good-Games-Munich/paperless-ngx.svg?style=flat-square
[issues-url]: https://github.com/Good-Games-Munich/paperless-ngx/issues
