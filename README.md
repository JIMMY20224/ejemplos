# ejemplos
MySQL / MariaDB (SQL):
python
Copy code
import mysql.connector

mydb = mysql.connector.connect(
  host="localhost",
  user="username",
  password="password",
  database="mydatabase"
)

# Resto de la operaciones con la base de datos
PostgreSQL (SQL):
python
Copy code
import psycopg2

conn = psycopg2.connect(
   dbname='mydatabase',
   user='username',
   password='password',
   host='localhost'
)

# Resto de la operaciones con la base de datos
SQLite (SQL):
python
Copy code
import sqlite3

conn = sqlite3.connect('example.db')

# Resto de la operaciones con la base de datos
MongoDB (NoSQL):
python
Copy code
from pymongo import MongoClient

client = MongoClient('mongodb://localhost:27017/')

# Resto de la operaciones con la base de datos
CouchDB (NoSQL):
python
Copy code
import couchdb

couch = couchdb.Server('http://localhost:5984/')

# Resto de la operaciones con la base de datos
Redis (NoSQL):
python
Copy code
import redis

r = redis.Redis(host='localhost', port=6379, db=0)

# Resto de la operaciones con la base de datos
Elasticsearch (NoSQL):
python
Copy code
from elasticsearch import Elasticsearch

es = Elasticsearch()

# Resto de la operaciones con la base de datos
Neo4j (NoSQL - Grafo):
python
Copy code
from neo4j import GraphDatabase

uri = "bolt://localhost:7687"
driver = GraphDatabase.driver(uri, auth=("username", "password"))

# Resto de la operaciones con la base de datos
Firebird (SQL):
python
Copy code
import fdb

conn = fdb.connect(
    dsn='localhost:C:/path_to_database/mydatabase.fdb',
    user='username', password='password'
)

# Resto de la operaciones con la base de datos
Apache Derby (SQL):
python
Copy code
import jpype
from jpype import java

# Configuración de jpype

Class.forName("org.apache.derby.jdbc.EmbeddedDriver")
conn = DriverManager.getConnection("jdbc:derby:mydatabase")

# Resto de la operaciones con la base de datos
HBase (NoSQL - Columnar):
python
Copy code
from starbase import Connection

c = Connection(host='localhost', port=8080)

# Resto de la operaciones con la base de datos
ArangoDB (NoSQL - Multimodelo):
python
Copy code
from pyArango.connection import *

conn = Connection(username="root", password="password")
db = conn["mydatabase"]

# Resto de la operaciones con la base de datos
Apache Cassandra (NoSQL):
python
Copy code
from cassandra.cluster import Cluster

cluster = Cluster(['127.0.0.1'])
session = cluster.connect('mydatabase')
