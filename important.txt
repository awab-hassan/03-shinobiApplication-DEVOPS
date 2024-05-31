Installing the database for MariaDB/MySQL
0. Kubectl exec -it SHINOBI_POD_NAME -- /bin/bash

1. Navigate to your Shinobi directory

CMD: cd /home/Shinobi

2. Open the MariaDB/MySQL Terminal client.

CMD: sudo mysql

3. Load the SQL files. user.sql are the credentials for Shinobi to connect to the database.

CMD: source sql/user.sql;

4. Exit the SQL client

CMD: exit;

4. If you need to enable the mysql database type you can run the following.

CMD: node tools/modifyConfiguration.js databaseType=mysql

5. Restart Shinobi. You should see a fresh log stream displaying Table creation notices.

CMD: pm2 flush && pm2 restart all 

6. If you want to see logs in container

CMD: pm2 flush && pm2 restart all && pm2 logs

7. Add your account in shinobi

browser: http[://]SHINOBI_IP/super > Accounts

8. Login with new account. 

browser: http[://]SHINOBI_IP:30754/ > LOGIN

