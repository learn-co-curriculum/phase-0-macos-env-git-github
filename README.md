# Mac Git And Github Configuration

## Install `git`

[Git][git] generally comes pre-installed with most operating systems, but you
can check by running `git version` in the terminal. If this gives you an error
or does not come back with a version number, you'll need to install Git. You can
install it using Homebrew.

[git]: https://git-scm.com/

### Action Item

1. Open the "Terminal" application using "Spotlight Search"
2. Type `brew install git` and press `<Enter>`
3. Close and reopen the "Terminal" application
4. Type `git version` and press `<Enter>`

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/D9Eudqng2sU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you see a message starting with "git version...", continue below.

## Create a GitHub Account

To work on and get credit for the labs and lessons that you work on during the
program, you will need to sign up for a GitHub account _if you don’t already
have one_.

### Action Item

1. Open the [GitHub signup webpage][] (https://github.com/join)
2. Fill out the form and create your account
3. Verify the email address connected to your GitHub account

[github signup webpage]: https://github.com/join

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/cVNLBQssm8g" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you were able to verify your email address, continue below.

## Configure Git and GitHub

Git is the tool that we’ll use to download and upload the work that we do in
labs and lessons. To use Git without signing in every time, you can create a
Secure Shell (SSH) key and associate that to your GitHub account. Lastly, you
will want to run a few commands to make sure that when you use Git, you get the
proper credit for your work. This step will ask you to do work both in your
browser and your terminal.

### Action Item

1. Open the "Terminal" application using "Spotlight Search"
2. Type `git config --global color.ui true` and press `<Enter>`
3. Type `git config --global user.name` + `<Space>` + your name and press
   `<Enter>` _(Note: this should be your full name, not your GitHub username, in
   quotes.)_
4. Type `git config --global user.email` + `<Space>` + the email address you
   used to sign up to GitHub and press `<Enter>`
5. Type `git config --global init.defaultBranch main` to
   [update the default branch name][] to `main`
6. Type `ssh-keygen` and press `<Enter>`
7. For each prompt **do not type anything**, just continue to press `<Enter>`.
   It's particularly important that you **do not enter a passphase** and leave
   the passphrase empty when prompted; otherwise, you'll have to enter that
   passphrase any time you interact with GitHub (which will happen a lot during
   the program); and you may run into issues submitting assignments later.
8. Type `cat ~/.ssh/id_rsa.pub | pbcopy` and press `<Enter>`. This will copy
   your SSH key to your clipboard
9. Open the [GitHub New SSH key form][] (https://github.com/settings/ssh/new)
   _(Note: you need to be logged in to GitHub to access that link.)_
10. Type "My personal Mac" in the "Title" input field
11. Paste what’s on your clipboard from step 8 in the "Key" input field
12. Click "Add SSH Key"

[github new ssh key form]: https://github.com/settings/ssh/new
[update the default branch name]: https://github.com/github/renaming

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/2YF15UlenxM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you see your new SSH key beneath the "SSH keys" heading, continue to the next
lesson, **Configuring the Flatiron Student Portal**.
