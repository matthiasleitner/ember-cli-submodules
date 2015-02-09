# Description

Util for managing multiple ember-cli projects using git submodules.

# Install

Install ember-cli-submodules

  `sudo npm install -g ember-cli-submodules`

This installs the ember-sub util which provides the following tasks:

# Usage

- Initialize and update submodules
  **Run this after you first checkout the umbrella projects including the git submodules**

```
    ember-sub init
```

- Install dependencies in all projects

```
    ember-sub install
```

- Execute ember-cli commands in all repos

```
    ember-sub ember <<ember-cli command>> (e.g. install:bower)
```

- Link or unlink one of the ember-cli-projects to all others

```
    ember-sub link|unlink <<project-name>> (e.g. ember-cli-runtastic-commons)
```

- Update one of the submodule to a new version and reference it in all others if needed.
  Supply the `--upgrade` option in order to perform the update in all repos referencing it

```
    ember-sub version <<project-name>> 0.0.10
```

- Bump the version of a given dependency in all submodules if it exists

```
    ember-sub upgrade <<project-name>> 0.0.10
```
