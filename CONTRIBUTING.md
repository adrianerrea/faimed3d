# How to contribute

## How to get started


This repository was initialized from a `nbdev` template. To make simple fixes to the code (e.g., typos) and push working notebooks to Github, which pass all tests, you need at least a basic anaconda environment with `nbdev`, which can be created with `conda create --name <env> -c fastai nbdev`. 
To participate in development you need to run `conda create --name <env> -c fastai -c PyTorch -c simpleitk -c conda-forge fastai simpleitk av nbdev scikit-image`, to create an environment with working fastai, SimpleITK and PyTorch modules.  
Before starting to change code in the notebooks, please install the git hooks that run automatic scripts during each commit and merge to strip the notebooks of superfluous metadata (and avoid merge conflicts). After cloning the repository, run the following command inside it:

```
nbdev_install_git_hooks
```
You also need to create a symlink between the libs and nbs by executing `!ln -s ../faimed3d nbs/faimed3d` from within one notebook or the terminal.

## Did you find a bug?

* Ensure the bug was not already reported by searching on GitHub under Issues.
* If you're unable to find an open issue addressing the problem, open a new one. Be sure to include a title and clear description, as much relevant information as possible, and a code sample or an executable test case demonstrating the expected behavior that is not occurring.
* Be sure to add the complete error messages.

#### Did you write a patch that fixes a bug?

* Open a new GitHub pull request with the patch.
* Ensure that your PR includes a test that fails without your patch, and pass with it.
* Ensure the PR description clearly describes the problem and solution. Include the relevant issue number if applicable.

## PR submission guidelines

* Keep each PR focused. While it's more convenient, do not combine several unrelated fixes together. Create as many branches as needing to keep each PR focused.
* Do not mix style changes/fixes with "functional" changes. It's very difficult to review such PRs and it most likely get rejected.
* Do not add/remove vertical whitespace. Preserve the original style of the file you edit as much as you can.
* Do not turn an already submitted PR into your development playground. If after you submitted PR, you discovered that more work is needed - close the PR, do the required work and then submit a new PR. Otherwise each of your commits requires attention from maintainers of the project.
* If, however, you submitted a PR and received a request for changes, you should proceed with commits inside that PR, so that the maintainer can see the incremental fixes and won't need to review the whole PR again. In the exception case where you realize it'll take many many commits to complete the requests, then it's probably best to close the PR, do the work and then submit it again. Use common sense where you'd choose one way over another.

## Do you want to contribute to the documentation?

* Docs are automatically created from the notebooks in the nbs folder.

