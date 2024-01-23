# How to quickly set up things for a new gig

## Python or/and Conda

[get Python]( https://www.python.org/downloads/windows/) or Mamba from [conda-forge](https://github.com/conda-forge/miniforge)

## VSCode

[code.visualstudio](https://code.visualstudio.com/)

## Addins & profile

cf vscode_profile.code-profile

## Git

[Download and install](https://git-scm.com/downloads) and then import config and aliases from `.gitconfig`

## If non root - troubles begin

### conda activate

One may need to duplicate `profile.ps1` to activate conda env.

### proxy

```ps1
conda config --show
# proxy_servers:
#  http: http://user:pw@server:port
#  https: http://user:pw@server:port

pip config list
# global.proxy='http://user:pw@server:port'

git config --global http.proxy http://user:pw@server:port
git config --global https.proxy http://user:pw@server:port
```
