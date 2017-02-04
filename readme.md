# Autoindex customization for Apache HTTP server
This package configures your Apache HTTP server to use custom directory index pages instead of the default ones.

## Dependencies
This customization requires that your Apache HTTP server is equal to or greater than **2.4** in the version. In addition, the following modules needs to be enabled:

* `mod_alias`: <https://httpd.apache.org/docs/2.4/mod/mod_alias.html>
* `mod_include`: <https://httpd.apache.org/docs/2.4/mod/mod_include.html>
* `mod_authz_core`: <https://httpd.apache.org/docs/2.4/mod/mod_authz_core.html>

## Installation
All files and directories provided in this package are relative to the `/etc/apache2/` (depends on the system you use) directory. To activate the configuration, just execute `a2enconf autoindex` and reload the configuration with `systemctl reload apache2`.