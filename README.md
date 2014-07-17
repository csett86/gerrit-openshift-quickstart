Running Gerrit on OpenShift
---------------------------

Create an account at https://www.openshift.com

Create a DIY 0.1 application + a MySQL 5.5 cartridge to the app, and import the quickstart code:

    rhc app create <app name> diy mysql-5.5 --from-code=https://github.com/csett86/gerrit-openshift-quickstart.git

You can now checkout Gerrit application at:

    http://<app name>-<your namespace>.rhcloud.com

Login is configured to be OpenID. The first registered user will be in the Administrators group.
