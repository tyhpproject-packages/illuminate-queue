<!-- tyhp-readme:start -->
# tyhpdef/illuminate-queue

Tyhp type definitions for `illuminate/queue` `13.32.0`.

```bash
composer require --dev tyhpdef/illuminate-queue:13.32.0
```

This is a metapackage. Composer also installs `tyhpdef/illuminate-queue-impl` (type files).
Require **this** name, not `tyhpdef/illuminate-queue-impl`.

See https://tyhplang.com.

## Maintain `illuminate/queue`? Ship the types yourself

If you are a Packagist maintainer of `illuminate/queue`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/illuminate-queue-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `illuminate/queue` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/illuminate-queue": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `illuminate/queue` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `illuminate/queue` with a real constraint,
   `"replace": { "tyhpdef/illuminate-queue": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `illuminate/queue` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/illuminate-queue` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
