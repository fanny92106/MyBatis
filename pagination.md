# MyBatis - page helper interceptor (插件)


1. add jars

        - pagehelper-5.0.0.jar
        - jsqlparser-0.9.5.jar


2. config pagination plugin in myBatis-config.xml file
![paginationPluginConfig](imagePool/paginationPluginConfig.png)


3. concat page string in pageUtil.java
![paginationUtil_0](imagePool/paginationUtil_0.png)
![paginationUtil_1](imagePool/paginationUtil_1.png)


4. test pagination
![paginationTest](imagePool/paginationTest.png)
![paginationResult](imagePool/paginationResult.png)
