# gitbucket-community.herokuapp.com

This project stores the definition of the community demo version of gitbucket available at : http://gitbucket-community.herokuapp.com/

## How to deploy

The herokuapp update itself using the content of the github project.
Thus on push, it will autiomatically redeploy with the new content.

## Update to a new version of gitbucket

- change in `update.sh` the version of gitbucket (use the tag value)
  for example from `GITBUCKET_VERSION=4.4` to `GITBUCKET_VERSION=4.5`
- run `./update.sh`
- commit & push the changes

## Update a plugin version

- change in `update.sh` the version of the plugin
  for example from `GITBUCKET_ANNOUNCE_PLUGIN_VERSION=1.4.0` to `GITBUCKET_ANNOUNCE_PLUGIN_VERSION=1.5.0`
- run `./update.sh`
- commit & push the changes

## Add a plugin

- add a variable storing the plugin version
- duplicate & adapt from another plugin the check and download part
- run `./update.sh`
- commit & push the changes
