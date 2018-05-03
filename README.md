# InternetDataAnaly

## 后端数据库设计

    +----------------------------------------------------------------+
    |                            user                                |
    +----------+-------------+------+-----+---------+----------------+
    | Field    | Type        | Null | Key | Default | Extra          |
    +----------+-------------+------+-----+---------+----------------+
    | uid      | int         | NO   | PRI |         | auto_increment |
    | sno      | varchar(20) | NO   | UNQ | NULL    |                |    
    | name     | varchar(50) | NO   |     | NULL    |                |
    | age      | varchar(5)  | NO   |     | NULL    |                |
    | grade    | varchar(5)  | No   |     | NULL    |                |
    |created_at| timestamp   | No   |     | NULL    |                |
    +----------+-------------+------+-----+---------+----------------+
    
    +----------------------------------------------------------------+
    |                        internetdata                            |
    +----------+-------------+------+-----+---------+----------------+
    | Field    | Type        | Null | Key | Default | Extra          |
    +----------+-------------+------+-----+---------+----------------+
    | id       |int          | NO   | PRI |         | auto_increment |
    | uid      |int          | NO   | UNQ |         |                |
    | url      |varchar(1000)| NO   |     | NULL    |                |    
    | date     |date         | NO   |     | NULL    |                | -- yyyy-mm-dd HH:mm:ss
    |created_at|timestamp    | No   |     | NULL    |                |
    +----------+-------------+------+-----+---------+----------------+
    

## 前端设计

1. 随机数据产生页面
    1. 随机数据产生配置文件
    2. 随机数据产生的结果（以配置文件的方式呈现）
2. 数据浏览页面
    1. 浏览产生的随机数据
    2. 根据用户自定义字段浏览
3. 计算结果并展示
    1. 数据汇总
    2. 根据用户要求进行计算
