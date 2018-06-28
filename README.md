#### 使用方法：  

1. 拉取代码：  
git clone https://github.com/lduhejian/docker-ecshop.git  
cd docker-ecshop  
mkdir web  
cd web  
2. 拉取 ecshop 代码：  
git clone repo:your-ecshop-code  
3. 配置 nginx:  
替换 default.conf 和 default.template.conf 第 11 行的 your_project_name 为你的项目名
4. 配置数据库：  
编辑 ecshop data/config.php 和 本项目的 .env 配置数据库信息  
编辑 config.php 中的 $db_host = "mysqldb"  
5. 导入数据库：  
sudo docker exec -i mysql mysql -uroot -p123456 dbname < 'xxxxxxxxxxxxxxx.sql'

更多信息参见：[docker-nginx-php-mysql](https://github.com/nanoninja/docker-nginx-php-mysql)
