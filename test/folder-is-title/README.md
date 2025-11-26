# 이건 바로 본문 시작인듯

폴더명에 한글은 안되나? -> 되는데 공백때문에 안됐던듯
# H1

## H2

### H3

![](./images/pasted_image.png)

![](./images/intellij.png)

<div>
<img width="30%" src="./images/pasted_image.png">
<img width="30%" src="./images/intellij.png">
</div>

test2

```mermaid
flowchart TD
    FUS[FileUploadService<br/>비즈니스 로직 + DB 저장]
    FSS{{FileStorageService<br/>인터페이스}}
    LFSS[LocalFileStorageService]
    S3FSS[S3FileStorageService]
    S3FUS[S3FileUploadService<br/>저수준 S3 API]

    FUS --> FSS
    FSS --> LFSS
    FSS --> S3FSS
    S3FSS -->|Composition| S3FUS

    subgraph local["file.upload.mode=local"]
        LFSS
    end

    subgraph s3["file.upload.mode=s3"]
        S3FSS
        S3FUS
    end

```

```java
public void main() {
	log.info("test");
}
```

> [!NOTE]  
> Highlights information that users should take into account, even when skimming.

> [!IMPORTANT]  
> Crucial information necessary for users to succeed.
