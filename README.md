libcue fork used by [pylibcue](https://github.com/Cycloctane/pylibcue).

Based on libcue v2.3.0. Added custom bugfixes and enhancements to make it more usable.

Applied changes:

`v2.3.0.dev0`: sync master/HEAD of upstream

`v2.3.0.dev1`:

- Fix compatibility issue of `CUE_EXPORT` when using msvc compiler.
- Add `never-interactive` option in flex.
- Add a macro to disable syntax warning output in stderr. (cc -DLIBCUE_QUIET_MODE)

`v2.3.0.dev2`:
- Fix yylineno int overflow (Merge https://github.com/lipnitsk/libcue/pull/49)
- Add missing `cd_get_catalog` API (Merge https://github.com/lipnitsk/libcue/pull/56)
- Fix NULL pointer check in `cd_get_track` (Merge https://github.com/lipnitsk/libcue/pull/60)

`v2.3.0.dev3`:

- Parse `REM COMMENT` lines.
- Parse `REM DISCID` and `REM COMPOSER` lines (stored in cdtext as "DISC_ID" and "COMPOSER").
