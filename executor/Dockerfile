FROM mesosphere/mesos:0.22.1-1.0.ubuntu1404

ADD ./build/docker/logstash-executor-dependencies.jar /tmp/logstash-executor-dependencies.jar

ADD ./build/docker/logstash-executor.jar /tmp/logstash-executor.jar

ENTRYPOINT ["java", "-Djava.library.path=/usr/local/lib","-jar", "/tmp/logstash-executor.jar"]
