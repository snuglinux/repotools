Scripts for working with the repository

Description of the configuration file of the repository:

In the program configuration file "repotools.conf", you can specify in the parameter "REPOCONF" arbitrary configuration file of the repository.

REPOCONF=repo.conf

In the file "repo.conf" the parameter "NOT_HANDLE" lists the packages that are ignored.

Example:
NOT_HANDLE="smail repotools"

Option ONLY_WARN checks updates and alerts about this email.

Example:
ONLY_WARN="catalyst-utils"

Auto start on schedule: systemctl enable repo-upd.timer

To run manually: systemctl start repo-upd