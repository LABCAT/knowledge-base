# Setting Up a Remote Database to Optimize WordPress Performance with MySQL

1. Set up two VPS instances.

2. Set up your application server

3. Set up your MySQL server.

4. Complete the <a rel="noreferrer noopener" aria-label="instructions (opens in a new tab)" href="https://www.digitalocean.com/community/tutorials/how-to-set-up-a-remote-database-to-optimize-site-performance-with-mysql-on-ubuntu-18-04" target="_blank">instructions</a> here to allow the web server to connect to the database server.

5. Create a mysql user who can connect to the database from the web server:

```
CREATE USER 'myuser'@'localhost' IDENTIFIED BY 'mypass';
CREATE USER 'myuser'@'IP.ADD.RE.SS' IDENTIFIED BY 'mypass';
GRANT ALL PRIVILEGES ON database.* TO 'myuser'@'localhost';
GRANT ALL PRIVILEGES ON databa
```
