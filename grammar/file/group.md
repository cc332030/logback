
# 分类存放

按日期
```xml
<!-- 输出到文件 常规 -->
<appender name="DEFAULT_FILE" class="ch.qos.logback.core.rolling.RollingFileAppender">

  <file>${logging.file.path}/${spring.application.name}/${logging.name.default}.log</file>

  <rollingPolicy class="ch.qos.logback.core.rolling.TimeBasedRollingPolicy">

    <fileNamePattern>${logging.file.path}/${logging.name.default}-%d{yyyy-MM-dd}.%i.log.gz</fileNamePattern>
    <maxHistory>${logging.file.max-history}</maxHistory>

    <timeBasedFileNamingAndTriggeringPolicy class="ch.qos.logback.core.rolling.SizeAndTimeBasedFNATP">
      <maxFileSize>${logging.file.max-size}</maxFileSize>
    </timeBasedFileNamingAndTriggeringPolicy>

  </rollingPolicy>

</appender>
```
