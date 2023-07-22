# ZMK Firmware: Personal fork

This repo is a [jyojoh](https://github.com/jyojoh/zmk)'s fork combined with [urob](https://github.com/urob/zmk)'s fork in order to get the reatures form both repos.

In order to use this branch with Github Actions, replace the contents of `west.yml` in
your `zmk-config/config` directory with the following contents:

```
manifest:
  remotes:
    - name: raydevs
      url-base: https://github.com/raydevs
  projects:
    - name: zmk
      remote: raydevs
      revision: main
      import: app/west.yml
  self:
    path: config
```


