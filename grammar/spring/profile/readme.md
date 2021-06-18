
# spring-profile 多环境配置

根据 spring 环境配置输出选项

根据 spring 环境配置日志输出
```xml
<springProfile name="proc">
  <root level="${logging.level.root}">
    <appender-ref ref="DEFAULT_FILE_ASYNC"/>
    <appender-ref ref="ERROR_FILE_ASYNC"/>
  </root>
</springProfile>
```
