libcue fork used by [pylibcue](https://github.com/Cycloctane/pylibcue).

Based on libcue v2.3.0. Added custom bugfixes and enhancements to make it more usable.

Applied changes:

`v2.3.0.dev0`: sync master/HEAD of upstream

`v2.3.0.dev1`:

- Fix compatibility issue of `CUE_EXPORT` when using msvc compiler.
- Add `never-interactive` option in flex.
- Add a macro to disable syntax warning output in stderr. (cc -DLIBCUE_QUIET_MODE)
