# minimal-node-10-build-env

> Containerized Minimal express Web Server using Alpine-based Node build environment.

> Based on `node:10.14.1-alpine`

## Use

https://docs.docker.com/develop/develop-images/multistage-build/

```
FROM minimal-node-10-build-env
...
```

> Hint: Use `npm ci` to install npm packages to speed up your installs.

## How to Build, Run and Publish
There are three scripts in `package.json`
- `npm run docker:build` will rebuild the Docker image with any changes
- `npm run docker:run` will run the Docker image locally without having to publish it first
- `npm run docker:publish` will publish the image to http://hub.docker.com

## Resources
  > The environment is configured following best practices from [NodeSource](https://nodesource.com/blog/8-protips-to-start-killing-it-when-dockerizing-node-js/).

## Credits
* [Doguhan Uluca](https://github.com/duluca/minimal-node-web-server.git)