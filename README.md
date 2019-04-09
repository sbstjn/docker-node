# sbstjn/node [![Docker Stars](https://img.shields.io/docker/stars/sbstjn/node.svg?maxAge=600)](https://hub.docker.com/r/sbstjn/node/) [![Docker Pulls](https://img.shields.io/docker/pulls/sbstjn/node.svg?maxAge=600)](https://hub.docker.com/r/sbstjn/node/)

> Docker image with useful tools for `node` projects. Works fine in CircleCI and GitLab CI.

## Components

- `aws-cli/1.16.70 Python/2.7.15 Linux/4.9.125-linuxkit botocore/1.12.60`
- `Docker version 18.06.1-ce, build e68fc7a`

### Packages

- `swagger-combine`

## Usage

### General

```Dockerfile
# Dockerfile

FROM sbstjn/node
```

### CircleCI

```yaml
jobs:
  checkout:
    working_directory: ~/repo
    docker:
      - image: sbstjn/node
```

## Development

```bash
# Clone repository

$ > git clone git@github.com:sbstjn/docker-node.git
$ > cd docker-node

# Build container

$ > docker build .

# Start bash and test your environment

$ > docker run -it --entrypoint /bin/bash <container-id>
```

## License

Feel free to use the code, it's released using the [MIT license](LICENSE.md).

## Contribution

You are welcome to contribute to this project! 😘

To make sure you have a pleasant experience, please read the [code of conduct](CODE_OF_CONDUCT.md). It outlines core values and beliefs and will make working together a happier experience.
