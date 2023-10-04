# gomods

An index of Go modules referenced on [my domain](https://go.nc0.fr).
The index is a set of static HTML documents generated using the
[SVGU](https://svgu.nc0.fr) tool which is then hosted on a Web server.

## Usage

Note: Apart from modifying the configuration, this project is not
meant to be used manually. Instead, everything is automated within
CI/CD.

The configuration for the index is done within the
[`svgu.sky`](svgu.sky) file, which is a
[Starlark](https://starlark.net) document. Everything it written
based upon the [SVGU API](https://svgu.nc0.fr/references).

To build the index, you need to install SVGU,
[Node.js](https://nodejs.org) and [NPM](https://npmjs.com).
Then, it is a matter of running the command:

```bash
 $ npm run build
```

A static set of HTML documents will be available inside a `dist`
directory.

## License

Copyright 2023 Nicolas Paul. All rights reserved.

The content of this repository is governed by a BSD-style license that
can be found in the [LICENSE](LICENSE) file.

The following header should be placed at the top of every file possible:

```text
Copyright 2023 Nicolas Paul. All rights reserved.
Use of this source code is governed by a BSD-style
license that can be found in the LICENSE file.
```
