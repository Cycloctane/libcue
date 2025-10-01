libcue fork used by [pylibcue](https://github.com/Cycloctane/pylibcue).

Based on libcue v2.3.0. Added custom bugfixes, security patches, enhancements and win32 (msvc) compatibility to make it more usable. Some of the patches are accepted by upstream.

Applied changes (Changelog since v2.3.0):

`v2.3.0.dev4`:

- **Remove** unused `DiscMode` and `TrackSubMode`, as they are only used by toc files in legacy cuetools codes and do not exist in CUE.
- Parse `REM DISCNUMBER` and `REM TOTALDISCS` lines. (Backported to upstream in https://github.com/lipnitsk/libcue/pull/69 )
- Fix buffer overflow in `time_frame_to_mmssff`. (Backported to upstream in https://github.com/lipnitsk/libcue/pull/67 )
- Fix sign-compare warning in `cdtext.c`.
- Correct typo in rem.c and rem.h (Merge https://github.com/lipnitsk/libcue/pull/63)

`v2.3.0.dev3`:

- Parse `REM COMMENT` lines. (Backported to upstream in https://github.com/lipnitsk/libcue/pull/66 )
- Parse `REM DISCID` and `REM COMPOSER` lines (stored in cdtext as "DISC_ID" and "COMPOSER").

`v2.3.0.dev2`:

- Fix yylineno int overflow. (Merge https://github.com/lipnitsk/libcue/pull/49)
- Add missing `cd_get_catalog` API. (Merge https://github.com/lipnitsk/libcue/pull/56)
- Fix NULL pointer check in `cd_get_track`. (Merge https://github.com/lipnitsk/libcue/pull/60)

`v2.3.0.dev1`:

- Fix compatibility issue of `CUE_EXPORT` when using msvc compiler. Avoid the use of `unistd.h` to improve windows compatibility. (Backported to upstream in https://github.com/lipnitsk/libcue/pull/65 )
- Add a macro to disable syntax warning output in stderr. (cc -DLIBCUE_QUIET_MODE)

`v2.3.0.dev0`: sync upstream master/HEAD.
