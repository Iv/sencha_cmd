# Sencha Cmd docker image for building ExtJS projects

Based on [hub.docker.com/r/rockmagicnet/sencha-cmd](https://hub.docker.com/r/rockmagicnet/sencha-cmd). Modified to be able to build a legacy extjs 4.2.1 project.

## Using image for automated builds

To build app in working directory use the following command:

```
docker run --rm -v `pwd`:/app -w /app \
  rockmagicnet/sencha-cmd:latest \
  app build
```

Note that the absolute path is provided with `pwd` command.

For Sencha Cmd instructions please refer the official documentation at https://docs.sencha.com/cmd/
