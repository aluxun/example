## exe目录(http协议例子)
   ### 操作步骤
   1. 解压http_exe.rar文件,双击运行http.exe或https.exe
   2. 打开浏览器输入http://127.0.0.1(https://127.0.0.1)或者http://127.0.0.1/index.html(https://127.0.0.1/index.html),即可看到exe同目录下web目录中的index.html
   3. 输入http://127.0.0.1/img.jpg(https://127.0.0.1/img.jpg)即可看到图片
   4. 输入http://127.0.0.1/web.rar(https://127.0.0.1/web.rar)即可下载web.rar文件
   5. 支持自定义http、https的自定义get post请求和响应.(Lx_httpServer.rar解压出来里面有个httpClient目录就是自定义post请求例子)
***
## Lx_MInIO.rar
   [minio中文官网](https://www.minio.org.cn/?bd_vid=6839495683016526177)  
   [RocketMq官网](https://rocketmq.apache.org/zh/)
   ### 对象存储(Minio)和消息队列(消息中间件Kafka、Rocketmq )  注:在腾讯云产品服务上我就比较关注这两个产品(腾讯短信的请求参数生成是真的恶心人 太麻烦了 还好有调试工具 最终成功)
   这是一个关于对象存储(minio)的例子，其编译环境是 msvc x64,官方说世界上最快的对象存储,没有之一。支持文件的断点续传、分片上传、桶支持有效时间(对象上传之后开始 超过有效期之后自动删除对象)
   
***
## Lx_httpServer.rar和vs_httpServer.rar
   http.exe、https.exe source_code
***
## Lx_SqlDatabase.rar
  这是纯c的数据库接口  支持mysql、sqlite两种数据库 特点:和qt有相同的api接口名 如果是控制台应用，也就是不需要gui的 且又需要数据库支持的  支持跨平台.
    
  NoSql数据库：  
  redis    
  [HBase官网](https://hbase.apache.org/)  
  [Cassandra官网](http://www.cassandra.com.cn/) 
  NewSql数据库:
    TiDB数据库[TiDB官网](https://cn.pingcap.com/)  
  后面两个和消息中间件(Kafka、Rocketmq)是java语言实现 Apache软件基金会的产品  想要编译这两个的c++ Thrift 客户端sdk有点难度

  数据存储和分布式数据存储
     数据持久化可以保存在 txt文件 二进制文件(序列化结构体到二进制文件中) 注册表以及数据库 等  
     想要存储海量数据只能采用分布式存储  类似把一个大文件分成多个小文件保存在不同的计算机(节点)上  minio和hbase Cassandra TiDB都支持分布式存储  把多个hbase服务端集群运行在不同的节点上  
     然后通过客户端的sdk访问这些服务端集群 这些服务端集群可能有中心(主)节点  也可能没有主节点  采用某种负载均衡算法将各个服务端节点连接起来。
     

  
