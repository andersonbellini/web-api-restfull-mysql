# web-api-restfull-mysql
Api restfull with express and connection with mysql using sequelize.

Database need to br created:<br />
CREATE DATABASE "DabaBaseName"

Error:<br />
Unhandled rejection SequelizeConnectionError: Client does not support authentication protocol requested by server; consider upgrading MySQL client

Correction:<br />
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'youpassword'

Endpoints:<br />
http://localhost:3000/api/task  (get and post)<br />
http://localhost:3000/api/task/1 (getById, delete e put)<br />
http://localhost:3000/api/task/?limit=10&page=1 (find paginated and records of limits)

[Created by Anderson V. Bellini](https://linkedin.com/in/abellini/)