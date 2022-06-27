# Letters Nginx

## default.conf

- front 주소
- api 주소
- chat 주소

{{URL}} 설정

---

## 실행

```shell
docker build -t nginx:lb .
docker run -d -p 80:80 --name nginx_letters nginx:lb
```


### Node Exporter Metric -> Prometheus
```shell
docker run -d -p 9113:9113 nginx/nginx-prometheus-exporter:0.10.0 -nginx.scrape-uri=http://{IP}/metrics
```