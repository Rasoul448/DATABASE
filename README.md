import mysql.connector
db=mysql.connector.connect(
     host="localhost",
     user="root",
     password="",
     database="regstu12"
)
# print(db.is_connected())

mycur=db.cursor()
# mycur.execute("create database Regstu12")
# mycur.execute("create table Schoolsama(Studentcode VARCHAR(11),fname VARCHAR(40),lname VARCHAR(50), address VARCHAR(60),degree VARCHAR(70), Phonenumberintprovince VARCHAR(11))")
# mycur.execute("insert into schoolsama(Studentcode,fname,lname,address,degree,Phonenumberintprovince)values('2803474179','ilya','gare ly','khoy','the eleventh','0914720035')")

mycur.execute("select * from Regstu12 where = Studentcode : ")

mycursor = db.cursor()

for x in mycur:
  print(x)
