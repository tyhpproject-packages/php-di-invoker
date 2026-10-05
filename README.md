<!-- tyhp-readme:start -->
# tyhpdef/php-di-invoker

Tyhp type definitions for `php-di/invoker` `2.3.7`.

```bash
composer require --dev tyhpdef/php-di-invoker:2.3.7
```

This is a metapackage. Composer also installs `tyhpdef/php-di-invoker-impl` (type files).
Require **this** name, not `tyhpdef/php-di-invoker-impl`.

See https://tyhplang.com.

## Maintain `php-di/invoker`? Ship the types yourself

If you are a Packagist maintainer of `php-di/invoker`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/php-di-invoker-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `php-di/invoker` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/php-di-invoker": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `php-di/invoker` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `php-di/invoker` with a real constraint,
   `"replace": { "tyhpdef/php-di-invoker": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `php-di/invoker` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/php-di-invoker` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
