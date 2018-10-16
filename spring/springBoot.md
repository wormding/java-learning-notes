# SpringBootApplication.java
## 1.code
```
@Target(ElementType.TYPE)
@Retention(RetentionPolicy.RUNTIME)
@Documented
@Inherited
@SpringBootConfiguration
@EnableAutoConfiguration
@ComponentScan(excludeFilters = {
        @Filter(type = FilterType.CUSTOM, classes = TypeExcludeFilter.class),
        @Filter(type = FilterType.CUSTOM, classes = AutoConfigurationExcludeFilter.class) })
public @interface SpringBootApplication {
...
}
```
## 2.explaination
```
可以看到这个主要注解由三部分构成
1. SpringBootConfiguration = Configuration
2. ComponentScan 扫描指定目录，或者扫描该类所在目录下的所有文件
3.
https://www.cnblogs.com/shamo89/p/8184960.html
