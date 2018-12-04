# Problem

```
C:\Users\vladi\Documents\src\test-bazel-43>bazel build ...
INFO: Invocation ID: 8e5f7b4d-5fab-4c32-87a6-11d9fd6d7f7c
ERROR: C:/users/vladi/documents/src/test-bazel-43/BUILD:1:1: no such package '@hi//': Traceback (most recent call last):
        File "C:/users/vladi/_bazel_vladi/3e23o57f/external/bazel_tools/tools/build_defs/repo/git.bzl", line 166
                _clone_or_update(ctx)
        File "C:/users/vladi/_bazel_vladi/3e23o57f/external/bazel_tools/tools/build_defs/repo/git.bzl", line 72, in _clone_or_update
                fail(("error cloning %s:\n%s" % (ctx....)))
error cloning hi:
+ cd C:/users/vladi/_bazel_vladi/3e23o57f/external
+ rm -rf C:/users/vladi/_bazel_vladi/3e23o57f/external/hi C:/users/vladi/_bazel_vladi/3e23o57f/external/hi
"C:/Users/vladi/scoop/apps/coreutils/current/bin/rm.exe": cannot remove directory `C:/users/vladi/_bazel_vladi/3e23o57f/external/hi': Permission denied
"C:/Users/vladi/scoop/apps/coreutils/current/bin/rm.exe": cannot remove directory `C:/users/vladi/_bazel_vladi/3e23o57f/external/hi': Permission denied
 and referenced by '//:test'
ERROR: Analysis of target '//:test' failed; build aborted: no such package '@hi//': Traceback (most recent call last):
        File "C:/users/vladi/_bazel_vladi/3e23o57f/external/bazel_tools/tools/build_defs/repo/git.bzl", line 166
                _clone_or_update(ctx)
        File "C:/users/vladi/_bazel_vladi/3e23o57f/external/bazel_tools/tools/build_defs/repo/git.bzl", line 72, in _clone_or_update
                fail(("error cloning %s:\n%s" % (ctx....)))
error cloning hi:
+ cd C:/users/vladi/_bazel_vladi/3e23o57f/external
+ rm -rf C:/users/vladi/_bazel_vladi/3e23o57f/external/hi C:/users/vladi/_bazel_vladi/3e23o57f/external/hi
"C:/Users/vladi/scoop/apps/coreutils/current/bin/rm.exe": cannot remove directory `C:/users/vladi/_bazel_vladi/3e23o57f/external/hi': Permission denied
"C:/Users/vladi/scoop/apps/coreutils/current/bin/rm.exe": cannot remove directory `C:/users/vladi/_bazel_vladi/3e23o57f/external/hi': Permission denied
INFO: Elapsed time: 5.491s
INFO: 0 processes.
FAILED: Build did NOT complete successfully (0 packages loaded, 0 targets configured)
    Fetching @hi; fetching
```
