# minimal-node-10-build-env

> Alpine-based Node build environment with npm, bash and git

> Based on `node:10.14.1-alpine`

## Use

https://docs.docker.com/develop/develop-images/multistage-build/

```
FROM minimal-node-10-build-env
...
```

> Hint: Use `npm ci` to install npm packages to speed up your installs.

## To build

```
npm run build
```

or


```
docker image build .
```

## To update git tag

Any time there's a new version execute `npm run push-tag`


> Only use when updating Alpine contents, but specific version of the base package remains the same

```
git push origin :refs/tags/<tagname>
git tag -fa <tagname>
git push origin master --tags
```
# minimal-node-10-build-env
