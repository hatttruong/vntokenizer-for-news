# vntokenizer-for-news
use vntokenizer to tokenize VNese news

## Installation (on Windows)
(Ref: http://nishutayaltech.blogspot.com/2015/04/how-to-run-apache-spark-on-windows7-in.html, http://www.ics.uci.edu/~shantas/Install_Spark_on_Windows10.pdf)
  - Install Scala: 
    * Download Scala from the link: http://downloads.lightbend.com/scala/2.11.8/scala-2.11.8.msi
    * Set environmental variables:
      * User variable: SCALA_HOME = C:\Program Files (x86)\scala
      * system variable: PATH = C:\Program Files (x86)\scala\bin
    * checking on cmd, run "scala -version"
    
  - Install JAVA 8
    * download at http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
     * Set environmental variables:
      * User variable: JAVA_HOME = C:\Program Files\Java\jre1.8.0_77
      * system variable: PATH = C:\Program Files\Java\jre1.8.0_77\bin
    * checking on cmd, run "java -version"
    
  - Download Spark at https://spark.apache.org/downloads.html (I choose spark-2.1.0-bin-hadoop2.7.tgz)
    * Set environmental variables:
      + user variable: SPARK_HOME = C:\spark-2.1.0-bin-hadoop2.7
      + ystem variable: PATH = C:\spark-2.1.0-bin-hadoop2.7\bin
      
  - Install Python

  - Dowload Windows Utilities at https://github.com/steveloughran/winutils/blob/master/hadoop-2.6.0/bin/winutils.exe and put it in "C:\winutils\bin"
  - Using Spark Prebuilt Package:
    * Set HADOOP_HOME =C:\winutils in environment variable
    * Re run the command: C:\winutils\bin\winutils.exe chmod -R 777 C:\tmp\hive
    * Re run cmd "spark-shell"
  - Run Spark
    * For Spark UI : open http://localhost:4040/ in browser
    * For testing the successful setup you can run the example :
  - Add two new environment variables like before: (https://nerdsrule.co/2016/06/15/ipython-notebook-and-spark-setup-for-windows-10/)
    * PYSPARK_DRIVER_PYTHON = jupyter
    * PYSPARK_DRIVER_PYTHON_OPTS = notebook
  - RUN jupyter notebook:
    * follow: https://blog.duyet.net/2016/09/chay-apache-spark-voi-jupiter-notebook.html#.WPgq3tKGOM8
    * ERROR: AttributeError: module 'numpy' has no attribute 'core' ==> 
    
## 
