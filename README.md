AWS cli in minimal footprint
============================

Automatic built minimal docker image for AWS cli based on Alpine Linux for ppc64le architecture (`library/alpine:latest`), around 77MB.

Forked from: https://github.com/anigeo/docker-awscli

## Usage
```
docker run --rm -v <config_path>:/root/.aws:ro -v <option_yml>:/aws:ro seemethere/awscli-ppc64le <argument>
```

Or

```
docker run --rm -e AWS_ACCESS_KEY_ID=<key> -e AWS_SECRET_ACCESS_KEY=<secret> -e AWS_DEFAULT_REGION=<region> -v <option_yml>:/aws:ro seemethere/awscli-ppc64le <argument>
```

Refer to <http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html> for detail.

## More information
Alpine Linux for ppc64le: <https://registry.hub.docker.com/_/ppc64le/alpine/>

AWS cli: <https://aws.amazon.com/cli/>
