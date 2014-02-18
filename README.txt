Code Login module for Drupal 7.x

Author: Massimo Simonini


SUMMARY
===============
Code Login is a simple Drupal module that allow users to login using its own Italian Codice Fiscale instead of username.

It implements hook-form_alter() to override Username's "title" and "description" fields and Password's "description" field on:
- user_profile form
- user register form
- user_login e user_pass pages
- user login block

In the module is also included a "code_login_validate()" function to check Codice Fiscale validation.
By default, validation check is performed only on user-register, allowing super-user to login with it's own username. To extend validation to user-login (and force super-user to login the same way) follow the instructions in code_login.module file


REQUIREMENTS
===============
The Code Login module works for Drupal version 7 only.


INSTALLATION
===============
1 - Install as usual, see http://drupal.org/node/895232 for further information.
2 - Enable the module in admin/modules
3 - That's all!
    Now you have the "Codice Fiscale" field instead of Username field in all user pages/blocks


TROUBLESHOOTING
===============
If you encounter an issue while using this module, please post it as a bug or feature request on Github issues: https://github.com/massiws
Suggestions are also appreciated!
