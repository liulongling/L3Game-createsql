用于分库分表项目快速生成sql语句工具

# 配置数据库数据源
```
文件路径：D:\\liulongling\\work\\github\\L3Game-createsql\\config\\dbm\\prod.json

 prod.json配置文件示例：
 {
     "env": "prod",
     "dbName": "game_udb",
     "dbCount": 10, //数据库数量
     "port": 3306,
     "plat": "bilibili",
     "game": "SG",
     "remark": "示例",
     "username": "root",
     "password": "123456",
     "ips": ["127.0.0.1","192.0.0.1"]
 }
 
 
```
# 创建sql文件目录和存放文件
* * 存放文件夹层次：
* * 一层 项目 _ 版本_维护日期
* * 二层 平台
* * 三层 IP
* * 样例：
* * SG_1.8_20180731
* * ├── bili
* * │ ├── 192.168.0.2
* * │ │ ├── game_udb_10.sql
* * │ │ └── game_udb_20.sql
* * │ ├── 192.168.0.4
* * │ │ ├── game_udb_30.sql
* * │ │ └── game_udb_40.sql
* * ├── uo
* * │ ├── 192.168.1.2
* * │ │ ├── game_udb_10.sql
* * │ │ └── game_udb_20.sql
* * │ ├── 192.168.1.4
* * │ ├── game_udb_30.sql
* * │ └── game_udb_40.sql