# Background

In the past, the llvm source code were split between separate repos. However, those repos are archived and no longer updated. The latest code now lives in a single repo called [`llvm-project`](https://github.com/llvm/llvm-project)

Because the llvm-project is a very large repo for people to clone as a submodule, the Darling team has decided that manually uploading the source code changes to our forked repos would be a better approach.

# Repos

If you plan on updating the llvm source code, it a good idea to make sure that all of the repo are updated to use the same release.

* [darling-compiler-rt](https://github.com/darlinghq/darling-compiler-rt)
* [darling-libcxx](https://github.com/darlinghq/darling-libcxx)
* [darling-libcxxabi](https://github.com/darlinghq/darling-libcxxabi)

# Copying Over Source From The llvm-project

After you clone the source code to your local drive, make sure that you checkout a tagged release (ex: `llvmorg-13.0.1`).

Unfortunately, there isn't an easy way to figure out which version is the right one to use. It requires a bit of trial and error to figure out.

Copy the contents from the folder into the repo that you are working on. For example, if you are working on libcxx, you copy the files inside the libcxx folder and paste them into the local copy of darling-libcxx.