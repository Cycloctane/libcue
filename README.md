libcue fork used by [pylibcue](https://github.com/Cycloctane/pylibcue).

Based on libcue v2.4.4. Added custom bugfixes and enhancements to make it more usable. Some of the patches are accepted by upstream.

Applied changes (since upstream v2.4.4):

- Remove unused `DiscMode` and `TrackSubMode`, as they are only used by toc files in legacy cuetools codes and do not exist in CUE.
- Add a macro to disable syntax warning output in stderr. (cc -DLIBCUE_QUIET_MODE)
