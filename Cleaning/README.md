•	Download the NYC 311 Complaint Dataset from https://data.cityofnewyork.us/Social-Services/311/wpe2-h2i5

•	To clean the data and extract cleaned CSV file run the following command

              spark2-submit cleaning.py /user/sd3462/Project/311.csv	

  The last argument(311.csv) is the input file stored in the Hadoop folder

•	To get the output file run the following command

              hdfs dfs –get Cleaned_311.csv /home/sd3462/BDA/Project/

•	Below aliases are set in .bashrc file

	alias hfs='/usr/bin/hadoop fs '

	export HAS=/opt/cloudera/parcels/CDH-5.9.0-1.cdh5.9.0.p0.23/lib

	export HSJ=hadoop-mapreduce/hadoop-streaming.jar

	alias hjs='/usr/bin/hadoop jar $HAS/$HSJ'	
