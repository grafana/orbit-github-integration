# orbit-github-integration
Integration between Orbit and GitHub.

## Quickstart

Requirements:
- Python >= 3.8
- An Orbit account/workspace
- A GitHub account

To run **orbit-github** locally, you've to create a `.env` file like this one:

```sh
$ cat .env
# Required
ORBIT_WORKSPACE=your-orbit-workspace-id-goes-here
ORBIT_TOKEN=your-orbit-token-goes-here
GITHUB_TOKEN=your-github-token-goes-here
GITHUB_ORG_NAME=the-name-of-your-organization-goes-here
GITHUB_TOKEN=your-github-token-goes-here

# Optional
GITHUB_REPO_NAME_CONTAINS=string-to-match-repositories-with # Default: ""
ENLAPSED_TIME=10 # Default: 1 (hour)
```

Install the requirements with:
```sh
$ pip install -r requirements.txt
```

Run the script with:
```
$ python orbit-github.py
time=2021-11-22T13:43:55.060610 level=INFO location=orbit-github.py:221:<module> msg="Starting github_orbit" 
time=2021-11-22T13:43:56.278318 level=INFO location=orbit-github.py:233:<module> msg="Processing repo" repository="k6"
time=2021-11-22T13:43:56.774092 level=INFO location=orbit-github.py:114:parse_github_event msg="Parsing event" repository="k6" type="IssueCommentEvent" user="na--"
...
```
Profit!

