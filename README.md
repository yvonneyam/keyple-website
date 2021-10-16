# Eclipse Keyple website  

Repository to the www.keyple.org website of the 'Eclipse Keyple' project.

The Eclipse Keyple website is generated with Hugo.

## Getting started

### Local installation
Install [hugo extended](https://gohugo.io/getting-started/installing/) on your machine.
Install dependencies, build assets and start a webserver:
```bash
hugo server
```

Checkout http://localhost:1313/

### Using docker 

You can use the image "ext-alpine" from the project : https://github.com/klakegg/docker-hugo. An "ext" is needed image because it includes golang.


Launch a shell into hugo container from the root directory of this project
```bash
docker run --rm -it \
  -v $(pwd):/src \
    -p 1313:1313 \
  klakegg/hugo:ext-alpine \
  shell
```

Then run
```bash
hugo server --environment development
```

If you want to avoid downloading modules at each run, install them locally by running
```bash
hugo mod vendor
```


## Contributing

1. [Fork](https://help.github.com/articles/fork-a-repo/) the [eclipse/keyple-website](https://github.com/eclipse/keyple-website) repository
2. Clone repository: `git clone https://github.com/[your_github_username]/keyple-website.git`
3. Create your feature branch: `git checkout -b my-new-feature`
4. Make your changes
5. Commit your changes: `git commit -m "Add some feature" -s`
6. Push feature branch: `git push origin my-new-feature`
7. Submit a pull request


### Declared Project Licenses

This program and the accompanying materials are made available under the terms
of the Eclipse Public License v. 2.0 which is available at
http://www.eclipse.org/legal/epl-2.0.

SPDX-License-Identifier: EPL-2.0

## Related projects

### [Wowchemy](https://github.com/wowchemy/wowchemy-hugo-modules)

[Wowchemy theme](https://wowchemy.com/) for [Hugo](https://gohugo.io/). 

## Bugs and feature requests

Have a bug or a feature request? Please search for existing and closed issues. If your problem or idea is not addressed yet, [please open a new issue](https://github.com/eclipse/keyple-website/issues/new).

## Trademarks

* Eclipse Keyple and the Eclipse Keyple project are Trademarks of the Eclipse Foundation, Inc.
* Eclipse® is a Trademark of the Eclipse Foundation, Inc.
* Eclipse Foundation is a Trademark of the Eclipse Foundation, Inc.

## Copyright and license

Copyright 2020 the [Eclipse Foundation, Inc.](https://www.eclipse.org) and the [keyple-website authors](https://github.com/eclipse/keyple-website/graphs/contributors). Code released under the [Eclipse Public License Version 2.0 (EPL-2.0)](https://github.com/eclipse/keyple-website/blob/src/LICENSE).
