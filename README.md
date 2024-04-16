# Wheels for OpenCV

Generate Python *manylinux* wheels for OpenCV with some customizations through GitHub actions.

The builds mostly correspond to the official headless variant, but with further modules disabled
which I do not need for server-based deployments and which omits possibly problematic third-party
dependencies like FFmpeg while https://github.com/opencv/opencv-python/issues/353 is unsolved.

## License

This repository is subject to the MIT license, as far as the workflow file sections can
actually be considered copyrightable anyway.

For the generated wheels, see the upstream license file at https://github.com/opencv/opencv-python/blob/4.x/LICENSE-3RD-PARTY.txt
Please note that some dependencies are omitted in builds from this repository, while I do not
give any guarantees that this list is complete and/or this repository does not introduce further
undeclared dependencies. Please review the source files and the build process/logs to avoid doubts.
