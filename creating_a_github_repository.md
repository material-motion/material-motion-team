# Creating a GitHub repository

GitHub repository creation rights for the `material-motion` org is restricted to a small set of Googlers.

## Convention

This is the naming convention we follow:

    github.com/material-motion/material-motion-<feature>-<platform/language>

## Step 1: Branches

Run the following to configure your initial branches:

    git init
    git checkout -b develop
    git push origin develop

## Step 2: Default branch

Update the default branch for your repository by visiting your repository's branches settings page.

> Example: https://github.com/material-motion/material-motion-team/settings/branches

## Step 3: Delete master

You can now delete the `master` branch.

    git push origin :master

## Step 4: Set up gh (one time global setup)

Set up the `gh` command line tool:

    git clone git@github.com:material-motion/gh.git
    cd gh
    sudo npm link

## Step 5: Configure the labels

Set up your repository's labels by running the following from a local copy of the material-motion-team repo:

    gh label templatize --template labels.json -u material-motion -r material-motion-repo-name