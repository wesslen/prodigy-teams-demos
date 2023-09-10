# Prodigy Teams Demos

## Setup

Setup the venv:

```
~/.pyenv/versions/3.9.9/bin/python3.9 -m venv venv-pt
source venv-pt/bin/activate
```

Install libraries with either `make install` or

```
pip install --upgrade pip
pip install prodigy-teams
pip install dev/*.whl
pip install prodigy-teams-recipes-sdk
pip install prodigy-teams-recipes
```

Then setup PAM and Cluster:

```
export PRODIGY_TEAMS_PAM_HOST="https://app.prodigy.ai/"
export PRODIGY_TEAMS_CLUSTER_HOST="https://[name of cluster].prodigy.ai"
ptc config set-pam-host $PRODIGY_TEAMS_PAM_HOST
ptc config set-cluster-host $PRODIGY_TEAMS_CLUSTER_HOST
```

Then login:
```
ptc login
```