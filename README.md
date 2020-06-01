# git-submodule-management

A fast git submodule management cli.

## Installation

```
npm install git-submodule-management -g
```

## Usage

### Init repository

Clone the repo and all submodules at one time.

```bash
gsm clone <repo>
```

### Add and commit changes the default tracked repo and submodules

```bash
gsm cm <message>
```

### Change branch of the default tracked repo and submodules

Switch the branches of the main repo and all submodules at the same time.

```bash
gsm checkout <localBranch>
```

### Add new branch to the default tracked repo and submodules

Synchronize the branches of the new main repo and all submodules. The default is to switch based on the branch name of the main repo. If the branch of the main repo and the submodules are inconsistent at this time, an error message will pop up. Please enter the submodules to maintain the branch name of the main repo and then execute this command.

```bash
gsm checkout -b <newBranch>
```

### Pull all updates from the default tracked repo and submodules

```bash
gsm pull
```

### Push all updates from the default tracked repo and submodules

```bash
gsm push
```
