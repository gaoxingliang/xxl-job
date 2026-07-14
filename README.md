# build the xxljob main docker image

```shell
cd xxl-job-admin && mvn clean && mvn package -DskipTests

docker build -t edwardg/xxl-job:admin-3.4.2 -f Dockerfile-self .

docker push edwardg/xxl-job:admin-3.4.2
```

# build the executor docker image

cd xxl-job-executor-samples, and do mvn package.
and

```shell
cd xxl-job-executor-samples/xxl-job-executor-sample-springboot && mvn clean && mvn package -DskipTests

docker build -t edwardg/xxl-job:xxl-job-executor-sample-springboot-3.4.2.1 -f Dockerfile-self .

docker push edwardg/xxl-job:xxl-job-executor-sample-springboot-3.4.2.1
```
