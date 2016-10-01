# github-keygen
SSH configuration for Github / SPCM

=head2 github-keygen - GitHub SSH Configuration Bootstrap

=head3 SYNOPSIS

Unix/Linux/MacOS X:

    git clone https://github.com/cdsalmons/github-keygen.git
    cd github-keygen
    ./github-keygen <my-github-username>
    cd ..
    rm -Rf github-keygen

=head3 EXAMPLE

    git clone https://github.com/cdsalmons/github-keygen.git
    cd github-keygen
    ./github-keygen cdsalmons
    cd ..
    rm -Rf github-keygen
    
=item *

It creates unique host aliases for github.com/gist.github.com that you'll be
able to use in Git URLs (C<git remote>) to connect to a particular account.
This gives the flexibility to use B<multiple GitHub accounts> (and therefore a
different SSH key for each).

    <account>.github.com:<repo-owner>/<repo>.git  (for each account)
    github.com:<repo-owner>/<repo>.git            (for the default account)

in addition to:

    git@github.com:<repo-owner>/<repo>.git
    
=head3 UPGRADE

To upgrade your config to the latest one, update C<github-keygen> and relaunch
it. It will update your F<~/.ssh/config> and show you the diff of what it
changed:

    cd github-keygen
    git rebase
    ./github-keygen
    
=head3 MORE INFO
 github-keygen-README.md


