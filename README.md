# askpass

> Safe Password Entry for R, Git, and SSH

[![Build Status](https://travis-ci.org/jeroen/askpass.svg?branch=master)](https://travis-ci.org/jeroen/askpass)
[![AppVeyor Build Status](https://ci.appveyor.com/api/projects/status/github/jeroen/askpass?branch=master&svg=true)](https://ci.appveyor.com/project/jeroen/askpass)
[![CRAN_Status_Badge](http://www.r-pkg.org/badges/version/askpass)](https://cran.r-project.org/package=askpass)
[![CRAN RStudio mirror downloads](http://cranlogs.r-pkg.org/badges/askpass)](https://cran.r-project.org/package=askpass)

Cross-platform utilities for prompting the user for credentials or a 
passphrase, for example to authenticate with a server or read a protected key.
Includes native programs for MacOS and Windows, hence no 'tcltk' is required. 
Password entry can be invoked in two different ways: directly from R via the 
askpass() function, or indirectly as password-entry back-end for 'ssh-agent' 
or 'git-credential' via the SSH_ASKPASS and GIT_ASKPASS environment variables.
Thereby the user can be prompted for credentials or a passphrase if needed 
when R calls out to git or ssh.

## Example

To invoke the password prompt manually use:

```r
askpass::askpass()
```

### R for MacOS 

![askpass-mac](img/askpass-mac.png)


### RStudio (server, desktop)


![askpass-rs](img/askpass-rs.png)


### RGUI / Windows

![askpass-rs](img/askpass-win.png)


### Terminals

![askpass-rs](img/askpass-term.png)



