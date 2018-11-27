##采集管理后台

### 部署文档
```text
git clone -b master https://github.com/Uwingame/spider-admin.git
 
chmod -R 777 storage
 
chmod -R 777 bootstrap
 
cp .env.example  .env
    
#修改.env数据库配置文件
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=project_spider_admin
DB_USERNAME=root
DB_PASSWORD=root
    
#接口服务器host地址


```
### 安装第三方控件
```text
composer install

```

### 单独安装日志系统
```text
php artisan log-viewer:publish
 
php artisan log-viewer:publish --force
 
php artisan log-viewer:publish --tag=config
 
php artisan log-viewer:publish --tag=lang
 
php artisan log-viewer:check

```

### 表迁移
```text
php artisan migrate

php artisan db:seed --class=UserTableSeeder

```
###(完毕)
