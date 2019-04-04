townhall -- the Stakeholder Democracy
===========================

**ESE Senior Design Team 17**

=== Quickstart ===

townhall is compatible with nearly all GNU/Linux servers with Apache, MySQL, and PHP. Simply clone the repository (with `git clone https://github.com/stakeholderdemocracy/townhall`) in your Apache public HTML directory and then navigate to `/index.php` to auto-configure. 

If extra permissions are needed to create MySQL tables, log in to your SQL console and create them with these commands, changing `<PASSWORD>` to your database password:

```
CREATE DATABASE `townhall`;
GRANT ALL ON `townhall`.* TO `townhall_dbuser`@localhost IDENTIFIED BY '<PASSWORD>';
FLUSH PRIVILEGES;
```

=== License ===

To be as free and transparent as possible for all local governments, the townhall platform is licensed under the GNU General Public License, version 3 only.
