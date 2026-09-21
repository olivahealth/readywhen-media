# readywhen-media

Finished readywhen social creative that has already been published. Buffer pulls the images from here by URL.

## Rules

- **Published work only.** This repo is public and its history is permanent: anything committed here can still be retrieved from forks and caches after it is deleted. Never commit a draft, an unreleased campaign, or anything you would not post publicly today.
- **Our own assets only.** Do not commit licensed stock or third-party creative whose terms do not allow public redistribution.
- **No secrets.** Nothing here runs. Actions and Pages are off by design.

## Getting an image URL for Buffer

Commit the file, then use its raw URL:

```
https://raw.githubusercontent.com/olivahealth/readywhen-media/main/<path/to/file>
```

The GitHub web UI gives you the same link under the file's **Raw** button.

### How files normally get here

`_tooling/li-media/publish.py` in the private readywhen-marketing-assets repo. It only accepts finished
images from the folders where creative is built, so a brief or a photo cannot be published by a
mistyped path, and it checks the address loads as an image before handing it back.

- **Published at approval, not at render.** Creative is published when a post is approved to go out,
  never while it is being worked on. That is how the first rule above holds in practice.
- **Names are made from the file's content** (`anniversary-1585b12813.gif`), so a file is never
  overwritten under the same address. GitHub caches for five minutes, and an overwritten file could
  let Buffer post the old version.
- **Do not edit or delete files by hand.** A post in Buffer may still point at one.

## Copyright

Copyright readywhen. All rights reserved. Public visibility exists so the files can be fetched by URL; it does not grant a licence to reuse them.
