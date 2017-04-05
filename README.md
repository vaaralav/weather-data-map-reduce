# MaxTemperature
Map-Reduce program to find out max air temperature in the USA in 1901 using NCDC weather data set.

## Compiling
```bash
javac *.java
jar cvf MaxTemperature1901.jar *.class
export HADOOP_CLASSPATH=MaxTemperature1901.jar
```

## Usage
Run the program:

```bash
hadoop MaxTemperature path/to/your/input/file/here path/to/your/output/directory/here
```

Read the result:

```bash
cat path/to/output/directory/*
```

## Requirements
- Java
- hadoop

## Input data
The input data for the program is NCDC weather data. Read more about the data set: [Hadoop: The Definitive Guide: Code and Data](http://hadoopbook.com/code.html).

The input format is one record per line. For example:
```
0029029070999991901010106004+64333+023450FM-12+000599999V0202701N015919999999N0000001N9-00781+99999102001ADDGF108991999999999999999999
```
