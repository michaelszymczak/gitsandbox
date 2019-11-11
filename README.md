# gitsandbox
Git sandbox

To export only subdirectory changes to another repository (works on new and existing local repo)

```bash

git clone git@github.com:michaelszymczak/gitsandbox.git fresh_main_repo || true
cd fresh_main_repo
git pull -r
git subtree split --prefix=subdir -b library
git push git@github.com:michaelszymczak/gitsandboxsubtree.git library:master
cd ..

```

Edited on Github
