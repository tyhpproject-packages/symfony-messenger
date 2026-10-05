<!-- tyhp-readme:start -->
# tyhpdef/symfony-messenger

Tyhp type definitions for `symfony/messenger` `7.4.19`.

```bash
composer require --dev tyhpdef/symfony-messenger:7.4.19
```

This is a metapackage. Composer also installs `tyhpdef/symfony-messenger-impl` (type files).
Require **this** name, not `tyhpdef/symfony-messenger-impl`.

See https://tyhplang.com.

## Maintain `symfony/messenger`? Ship the types yourself

If you are a Packagist maintainer of `symfony/messenger`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-messenger-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/messenger` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-messenger": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/messenger` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/messenger` with a real constraint,
   `"replace": { "tyhpdef/symfony-messenger": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/messenger` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-messenger` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
