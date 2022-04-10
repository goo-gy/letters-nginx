# Letters Nginx

### default.conf

- front 주소
- api 주소
- chat 주소

{{URL}} 설정

---

### 실행

```shell
docker build -t nginx:lb .
docker run -d -p 80:80 --name nginx_letters nginx:lb
```
