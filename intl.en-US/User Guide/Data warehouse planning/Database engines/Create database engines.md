# Create database engines {#concept_hfz_cjt_2hb .concept}

Data sources are classified into database engines and computing engines. A database engine is an external data source used as the storage medium for your source business system or the business system to be served after data construction. The data source type of a computing engine must be the same as the computing engine type specified in your computation configuration. A computing engine must be assigned to each project. A computing engine is used to compute and store data models. You can configure a database engine that is in an Alibaba Cloud VPC. After whitelisting the IP address of Dataphin in the VPC, you can use this database engine to read and write data. Currently, you can only create database engines in VPCs deployed in China \(Shanghai\). The VPCs in other regions will be supported in the future.

A database that stores physical data is a database engine. It serves as the source or basis for data construction and is used for data synchronization during data ingestion.

1.  Log on to Dataphin.
2.  In the top navigation bar of the Dataphin homepage, choose **Planning**. Alternatively, you can go to the Planning page from the **Intelligent Data Warehouse Planning** quick access area.

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/148397/156135512941387_en-US.png)

3.  In the left-side navigation pane, choose **Database Engines**.

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135512941445_en-US.png)

4.  In the upper right corner of the page, click **Create Data Source** to open the database engine configuration dialog box.

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513041448_en-US.png)

5.  You must select a data source type and specify the required information about your data source. Currently, the supported data source types include MaxCompute, MySQL, SQL Server, PostgreSQL, Oracle, HDFS, Hive, FTP, Vertica, DRDS, AnalyticDB, Elasticsearch, HBase 1.1.x, HBase 0.94.x, and MongoDB.
    -   If the selected data source type is MaxCompute, enter an endpoint, a project name, an AccessKey ID, and an AccessKey Secret.

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513041450_en-US.png)

    -   If the selected data source type is MySQL, DRDS, or PostgreSQL, enter a JDBC connection URL, a username, and a password.

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513041451_en-US.png)

    -   If the selected data source type is SQL Server or Oracle, specify a JDBC connection URL, a schema, a username, and a password.

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513041452_en-US.png)

    -   If the selected data source type is Vertica, specify a JDBC connection URL, a schema, a username, and a password.

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513041453_en-US.png)

    -   If the selected data source type is HDFS, the configurations required are shown in the following figure. You need to specify a DefaultFS address and whether to enable Kerberos authentication. If you enable Kerberos authentication, you need to enter a KDC server endpoint, select a Keytab file, and enter a Kerberos principal name.

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513041454_en-US.png)

    -   If the selected data source type is FTP, the configurations required are shown in the following figure. You need to specify a protocol, a host address, a port number, a username, and a password.

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513141456_en-US.png)

    -   If the selected data source type is Hive, the configurations required are shown in the following figure.

        -   For cluster configuration, you need to specify a NameNode and whether to enable Kerberos authentication. If you enable Kerberos authentication, specify a KDC server endpoint.
        -   For HDFS configuration, you need to select a Keytab file and enter a Kerberos principal name.
        -   For Hive configuration: you need to enter a JDBC connection URL, a username, and a password used for Hive2 connection.
        -   For metadatabase configuration: you need to specify a database type, a JDBC connection URL, a username, and a password.
        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513141457_en-US.png)

    -   If the selected data source is Elasticsearch, enter an Elasticsearch URL, a username, and a password, as shown in the following figure.

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513141460_en-US.png)

    -   If the selected data source type is HBase, select either the HBase 0.94.x or HBase 1.1.x version. The configurations required are shown in the following figure, including an HBase endpoint and the parameters \(in JSON format\) for connecting to HBase.

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513141463_en-US.png)

    -   If the selected data source type is MongoDB, enter a JDBC connection URL, a username, and a password, as shown in the following figure.

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513141466_en-US.png)

    -   If the selected data source type is AnalyticDB \(formerly ADS\), enter a JDBC connection URL, a username, and a password, as shown in the following figure.

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/149041/156135513141469_en-US.png)

6.  Click **Test Connection** to run a database connectivity test. If the message **The data source is connected** is returned, your configurations are saved. Click **OK** to exit.
