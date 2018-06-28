cd /web
拉去代码：
git clone repo:your-ecshop-code
配置 nginx:
替换 default.conf 和 default.template.conf 第 11 行的 your_project_name 为你的项目名
配置数据库：
编辑 ecshop config.php 和 本项目的 .env 配置数据库信息
注意 config.php 中的 $db_host = "mysqldb"
导入数据库：
sudo docker exec -i mysql mysql -uroot -p123456 dbname < 'xxxxxxxxxxxxxxx.sql'
启动环境：
sudo docker-compose up
