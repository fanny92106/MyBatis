# MyBatis



0. 持久层框架对比: Hibernate 和 MyBatis
![HibernateVSMyBatis](imagePool/HibernateVSMyBatis.png)



1. 核心开发步骤

    - 导入jar 包
    
            - mybatis
            - mysql-connector
            
    - 核心配置文件 MyBatis.xml
    
            作用:
                - 配置数据源信息
                - 配置transactionManager信息
                - MyBatis其他相关配置信息
                - 注册映射配置文件
                - 用于创建sessionFactory
            
    - 映射配置文件
    
            作用:
                - 与interface进行映射, 用于MyBatis创建实现类对象
                    - namespacee: interface名
                    - id: method名
                    - resultType: method返回类型
                - 创建SQL语句, 与Java(业务逻辑)代码解耦分离
    
    - 开发
    
            根据核心配置文件得到SqlSessionFactory
            使用SqlSessionFactory工厂获取sqlSession对象来执行增删改查,
            一个sqlSession就代表和数据库的一次对话, 非线程安全的, 用完关闭
![MyBatisMappterInterfaceAndMapperConfigFile](imagePool/MyBatisMappterInterfaceAndMapperConfigFile.png)
                
