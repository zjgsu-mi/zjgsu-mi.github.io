---
author: 韩建伟
title:  数据库应用
date:   2021-09-14
---

# [ER模型][er]

实体关系模型，是数据库系统设计的常用工具。

- [Visio][]
- [Dia][]

![er_fig][]

# 数据库连接

- 应用程序通过数据库驱动与数据库连接
- [Python][python_driver]、 [Node.js][node.js_driver]、 [Ruby][ruby_driver]、 [PHP][php_driver]、 [Java][java_driver]等都有相应的数据库驱动

# [数据库迁移][db_migration]

- 对关系数据库增量、可逆变化的管理
- 用编程的方式维护数据库的变化
- 在不同版本的数据库之间进行转换
- Ruby on Rails: Active Record
- Python: [alembic][]
- Node.js: [knex][]、[Sequelize][]

# [ORM][]

对象关系映射，把关系数据库和面向对象技术中对象关联起来

![orm_image][]

# 常用ORM

- 文档数据库(MongoDB等): [ODM][]
- Ruby on Rails: [Active Record][]
- Python: [SQLAlchemy][]
- Java: [Hibernate][]
- Node.js: [Sequelize][]等。


# 数据库缓存

- 提高数据的访问速度
- 读数据时，先从内存缓存中读取，如果缓存中没有再读取数据库，并把数据库中读取的数据保存到缓存中
- 通常采用[Redis][]、[Memcached][]等

# NoSQL

- KV型的数据，可采用Redis
- 对象型的，可以采用MongoDB之类的文档数据库

# MongoDB示例

~~~ javascript
// MongoDB
db.users.insert( {
    user_id: "abc123",
    age: 55,
    status: "A"
 } )

db.users.ensureIndex( { user_id: 1, age: -1 } )

db.users.find(
    { status: "A" },
    { user_id: 1, status: 1, _id: 0 }
)

db.users.update(
   { age: { $gt: 25 } },
   { $set: { status: "C" } },
   { multi: true }
)

db.users.remove( { status: "D" } )

db.users.drop()
~~~

[active record]: https://ruby-china.github.io/rails-guides/active_record_basics.html
[alembic]: https://pypi.org/project/alembic/
[db_migration]: https://en.wikipedia.org/wiki/Schema_migration
[dia]: http://dia-installer.de/
[er]: https://zh.wikipedia.org/wiki/ER%E6%A8%A1%E5%9E%8B
[er_fig]: ./er.png "ER图"
[hibernate]: http://hibernate.org/
[java_driver]: http://www.oracle.com/technetwork/java/javase/jdbc/index.html
[knex]: https://knexjs.org/
[memcached]: https://memcached.org/
[node.js_driver]: https://github.com/sindresorhus/awesome-nodejs#database
[odm]: https://docs.mongodb.com/ecosystem/drivers/#mongodb-odm-object-document-mapper
[orm]: https://zh.wikipedia.org/wiki/%E5%AF%B9%E8%B1%A1%E5%85%B3%E7%B3%BB%E6%98%A0%E5%B0%84
[orm_image]: ./orm.png "ORM"
[php_driver]: https://github.com/ziadoz/awesome-php#database
[python_driver]: https://github.com/vinta/awesome-python#database-drivers
[redis]: https://redis.io/
[ruby_driver]: https://github.com/markets/awesome-ruby#database-drivers
[sequelize]: http://docs.sequelizejs.com/
[sqlalchemy]: https://www.sqlalchemy.org/
[visio]: https://products.office.com/zh-cn/visio/flowchart-software
