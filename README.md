Phabricator SSO
===============

This patch enables Single Sign-On (SSO) for <a href="http://phabricator.org/">Phabricator</a>.
This is set up to use <a href="http://github.com/exflickr/GodAuth">GodAuth</a> but can be easily be modified for any SSO system.


Installation
------------

Copy the provided files on top of the following paths in your Phabricator install:

 * `phabricator/src/applications/auth/controller/PhabricatorLoginController.php`
 * `phabricator/src/applications/auth/application/PhabricatorApplicationAuth.php`

As-is, this patch requires an administrator-level user with the name 'admin' to be present.
If you have a differently-named admin account already configured, edit `PhabricatorLoginController.php`.
