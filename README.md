### Import Dependency

#### maven

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-minio</artifactId>
    <version>${spring-boot.version}</version>
</dependency>
```

#### gradle(groovy)

```groovy
implementation 'org.springframework.boot:spring-boot-starter-data-minio:${spring-boot.version}'
```

#### gradle(kotlin)

```kotlin
implementation("org.springframework.boot:spring-boot-starter-data-minio:${spring-boot.version}")
```

### Usage

1. application.properties

```properties
# application.properties
spring.minio.endpoint=http://localhost:9000
spring.minio.access-key=123456
spring.minio.secret-key=123456
```

2. ```MinioClient``` inject

```java
import io.minio.MinioClient;

public class Minio { 
    @Autowired
    private MinioClient client;
  	
  	....
}

```



