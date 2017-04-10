# Mozgalo-radionica
# SV Group d.o.o

Instalacija Sparka (Linux Ubuntu):

1. Skinuti Spark s http://spark.apache.org/, extractati ga u željeni direktorij te ga dodati u $PATH

2. Instalirati Jupyter i Toree naredbama

sudo apt-get update <br />


sudo apt-get install python-dev <br />


sudo python -m pip install -U pip <br />


sudo pip install futures==3.0.3 <br />


sudo pip install numexpr <br />


sudo pip install jupyter <br />


sudo pip install --pre toree <br />
 

sudo pip install https://dist.apache.org/repos/dist/dev/incubator/toree/0.2.0/snapshots/dev1/toree-pip/toree-0.2.0.dev1.tar.gz <br />


3. Namjestiti toree sa željenim Pathom te postavkama za Spark <br />


sudo jupyter toree install --spark_home=/usr/local/spark --interpreters=Scala,PySpark,SparkR,SQL --spark_opts='--master=local[2] --driver-memory=2g --packages com.sksamuel.scrimage:scrimage-core_2.11:2.1.8,com.sksamuel.scrimage:scrimage-filters_2.11:2.1.8,nu.pattern:opencv:2.4.9-7'