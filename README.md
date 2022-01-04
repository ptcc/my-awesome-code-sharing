# my-awesome-code-sharing
collection of links, resources and ideas on code sharing for typescript/javascript projects

## Table of contents
 - [Developer eXperience](#Developer)
 - [Multiple repositories](#Multiple)
 - [Monorepo](#Monorepo)
 - [React Native](#React)

Developer eXperience
====================
 - [npm-local-development](https://www.npmjs.com/package/npm-local-development)
 - Symlinking
 - lerna
 - yarn workspaces
 - meta

Multiple repositories
=====================
 - Meta
    - [Library](https://github.com/mateodelnorte/meta)
    - [npm plugin](https://github.com/mateodelnorte/meta-npm)
    - [bump plugin](https://github.com/patrykzurawik/meta-bump)
    - [github plugin](https://github.com/mateodelnorte/meta-gh)
 - private npm packages 
    - hosted npm registry
    - [npm private](https://docs.npmjs.com/about-private-packages)(paid) 
    - [github packages](https://levelup.gitconnected.com/private-npm-packages-in-github-package-registry-fbfda43acab3)
    - use git urls
    

### Library creation
 - [tsdx.io](https://tsdx.io/)

Monorepo
========

- [mobile+web React monorepo example](https://github.com/jlcastillo/rn-react-mobile-web-monorepo)

React Native
============
Since React Native metro packager does not follow symlinks some extra workaround setup needs to be done.

A good solution is watching and copying files

```bash
onchange 'mylib/dist/*.js' -- cp ./mylib/dist/* ./myapp/node_modules/mylib
```

