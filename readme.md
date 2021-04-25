# emdis

An embeded, reliable key-value store for Java


## 模块说明

### leveldb-java-api模块
   - leveldb的api封装
   - 基于guava+leveldb的结合，实现guava接口
   - cache注解  *todo*

### leveldb-java-emdis模块
   - 类redis数据结构的本地嵌入式KV结构数据库实现 *todo*
 
### emdis-spring-boot-starter 模块
   - emdis的springboot启动器实现 *todo*  

## 使用说明

-  leveldb-java-api 缓存使用说明

```java
 Cache<String, UUID> emdisCache =
                 EmdisCacheBuilder.newBuilder()
                         .maximumSize(100)
                         .softValues()
                         .build();
```

## 待优化项

- 基于guava的Leveldb 的接口实现，需要考虑批量操作，增加并发性能

