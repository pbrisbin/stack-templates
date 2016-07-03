# Stack Templates

My personal stack templates, so far just one.

## yesod-docker

This template creates a yesod project with my own preferences and a bunch of
machinery to develop and deploy via Docker.

```
stack new --resolver lts-6.5 --omit-packages \
  myproject https://raw.githubusercontent.com/pbrisbin/stack-templates/master/yesod-docker.hsfiles

make setup

bin/stack test
bin/stack exec yesod devel

make production
docker tag you/myproject registry/myproject
docker push registry/myproject
```
