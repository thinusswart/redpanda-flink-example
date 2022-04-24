# redpanda-flink-example
Basic set up of Redpanda, Flink and an example Java application to demonstrate stream processing between the two.

First run Maven to create a quick skeleton of an Apache Flink job.
```
mvn archetype:generate                               \
      -DarchetypeGroupId=org.apache.flink              \
      -DarchetypeArtifactId=flink-quickstart-java      \
      -DarchetypeVersion=1.14.4
```

This repo only contains the files I modified for getting the streaming job to work, so `pom.xml` and `StreamingJob.java`.

Once you've modified the files, you can build the JAR file using: `mvn clean package`

The resulting JAR can be uploaded to Flink for processing data streams. It should provide a good starting point to do more complex stream processing.