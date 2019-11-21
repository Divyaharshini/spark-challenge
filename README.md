<h1> Clean, Compile, Create fat jar files.</h1>
mvn clean
mvn compile
mvn assembly:single
<h1>Execute :</h1>
java -cp target/spark-challenge-1.0.0-jar-with-dependencies.jar edu.nwmissouri.bheemireddy.App "data.txt"
