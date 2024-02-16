# Intermediate-project-facial-authentication-system
the web face detector can also be designed to view faces in a video call. We need to get started with this project using an OpenCV and a webcam. OpenCV is a real-time computer vision tool. This project can be extended for use cases like user authentication in meetings, exams, police force, face unlock feature of phones, etc


#initialize_.py:



import datetime
from sqlalchemy import create_engine
from sqlalchemy.orm import sessionmaker
from tabledef import *

 
# create a Session
Session = sessionmaker(bind=engine)
session = Session()
 
user = User("admin@gmail.com","password")
session.add(user)
 
user = User("susanta@gmail.com", "1234")
session.add(user)
 
user = User("aditya@gmail.com","python")
session.add(user)
 
# commit the record the database
session.commit()
 
session.commit()






