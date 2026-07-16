pnpm, in a single file
========
[pnpm] in a single file, powered by [AppImage].

```console
$ ./pnpm --help
Usage: pnpm [command] [flags]
       pnpm [ -h | --help | -v | --version ]
...
```

NOTE: This is not an official pnpm application.

Installation
--------
```bash
curl -L https://github.com/simnalamburt/pnpm.appimage/releases/latest/download/pnpm-x86_64.AppImage -o pnpm
chmod +x pnpm
```

Maintaining releases
--------
The release workflow can rebuild a specific pnpm version from the GitHub
Actions UI. To find releases that are missing either architecture and queue
all of them after the workflow change is on the default branch:

```bash
./backfill       # list missing assets without changing anything
./backfill --run # queue one workflow run per missing release
```

&nbsp;

--------
*pnpm* is primarily distributed under the terms of both the [Apache License
(Version 2.0)] and the [MIT license]. See [COPYRIGHT] for details.

[pnpm]: https://pnpm.io/
[AppImage]: https://appimage.org/
[aws/aws-cli#4947]: https://github.com/aws/aws-cli/issues/4947

[Apache License (Version 2.0)]: LICENSE-APACHE
[MIT license]: LICENSE-MIT
[COPYRIGHT]: COPYRIGHT
