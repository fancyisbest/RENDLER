FROM java:8
COPY target/rendler-1.0-SNAPSHOT-jar-with-dependencies.jar /render/
ADD http://10.64.219.150/libmesos.so   /usr/lib/libmesos.so
ADD http://10.64.219.150/libmesos-0.25.0.so   /usr/lib/libmesos-0.25.0.so
WORKDIR "/rendler"
CMD java -cp rendler-1.0-SNAPSHOT-jar-with-dependencies.jar com.mesosphere.rendler.main.RendlerMain

