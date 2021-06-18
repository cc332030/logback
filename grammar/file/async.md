
# 异步输出

```xml
<!-- 异步日志 -->
<appender name="DEFAULT_FILE_ASYNC" class="ch.qos.logback.classic.AsyncAppender">
  <!-- 设置为不丢失日志,默认如果队列的80%已满,则会丢弃TRACT、DEBUG、INFO级别的日志 -->
  <discardingThreshold >0</discardingThreshold>
  <!-- 更改默认的队列的深度,默认值为256 -->
  <queueSize>1000</queueSize>

  <!-- 文件输出配置可直接写到这里，或者写到其他 appender，如：按日期分组的 appender -->
  <!--<appender-ref ref ="DEFAULT_FILE"/>-->
</appender>
```
