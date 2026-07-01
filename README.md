# build the xxljob main docker image

```shell
cd xxl-job-admin && mvn package

docker build -t edwardg/xxl-job:admin-3.1.1 -f Dockerfile-self .

docker push edwardg/xxl-job:admin-3.1.1
```

# build the executor docker image

cd xxl-job-executor-samples, and do mvn package.
and

```shell
cd xxl-job-executor-samples/xxl-job-executor-sample-springboot && mvn package

docker build -t edwardg/xxl-job:xxl-job-executor-sample-springboot-3.1.1.2 -f Dockerfile-self .

docker push edwardg/xxl-job:xxl-job-executor-sample-springboot-3.1.1.2
```
