pr2patch - create a patch file from a github pr

If your project is forked and the original project has not stylefile or uses a different style you can reformat all pull request to simplify the merge process into you code.

# usage:

```
# goto your cloned git remosetory
# pr2patch pullrequest_id <patchfile>
./pr2patch 42 ../pr42.patch
# goto your repo where you like to apply the patch
patch -p0 < ../pr42.patch.patch
```

Note: it is not allowed to place the patchfile into the git reposetory.
