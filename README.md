#### 使用方法：  

1. 拉取代码:  
git clone https://github.com/lduhejian/docker-ecshop.git  
cd docker-ecshop/web  
2. 拉取 ecshop 代码：  
git clone repo:your-ecshop-code  
3. 配置 nginx:  
cp .env.example .env  
编辑 .env, 设置 PROJECT_NAME 为你的 ecshop 项目名
4. 配置数据库:  
编辑 ecshop data/config.php 和 本项目的 .env 配置数据库信息  
编辑 config.php 中的 $db_host = "mysqldb"  
5. 运行 container:  
sudo docker-compose up
6. 导入数据库:  
sudo docker exec -i mysql mysql -uroot -p123456 dbname < 'xxxxxxxxxxxxxxx.sql'
7. 访问商城:  
localhost:10001

更多信息参见：[docker-nginx-php-mysql](https://github.com/nanoninja/docker-nginx-php-mysql)
