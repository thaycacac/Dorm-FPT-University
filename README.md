# **DATABASE SYSTEM OF DORM FPT UNIVERSITY**

STUDENT NAME: PHAM NGOC HOA   | SE05740  
STUDENT NAME: NGUYEN HAI NAM  | SE05817

### **Describe the problem**
**Nowadays, Students in FPT University almost live in five Dom, there are A, B, C, D, F and have some guard to manager it. But, it is still have not database system for manage dorm. After the actual survey, the result are as follows:**
- Student live in room of dom, each  room have one or more student, however at one point an student is only live in one room.
- The head of each room is an student who is the head of the department. And every student is managed by an guard.
- Guard records information about students, including: student code, first name, last name, email, phone, gender, course, roles. Character of the student are  M(Boy) of  F (Girl). Phone number can not greater than 11 digits.
- Gender of student have to equal gender of room.
- Guard also needs to manager number penalize to calculate fines by day or month. Calculate the amount of money owed by the student due to violation of regulations.
- Each penalty include: name of student is fined, type of penalize and quantity. 
- Student can register live in a room when number of bed is empty, that student have to pay for register.  Check Price are 1(have paid) or 0(not paid).
- Information for register include: room code, student code, date that student was check in.
- Each guard can manager one or more room and room can managed one or more guard.
- Room code is combination by Name Dome and Floor and number of room and number of bed. Example: a2055, it mean dome a, floor 2, room 05, bed 5.
- Information of room include: room code, location, number bed, gender, status bed.
- Location of the room are Trai(Left) or Phai (Right).
- Status bed of room are 1 (This bed is empty, student can register live in this bed) or  0 (This bed is registered, student can not register in this bed).
- Guard also need to manager facilities in FPT University to call fixer to fix the rooms are broken to student continue to live safe.
- Items of room can need fix example: light bulb, table, ect. Each item inclue: Item code, name of things need fix, content of device and price of that device.
- Fix detail include: room code, item code, name of fixer because have only 2 fixer is  H*ng  and  *?ng so we can't create new object fixer, day reported malfunction, day fix malfunction, quantity the same thing is broken.
- Guard manager every room in common dom, so manager room has a attribute is name room and every room in dom have to common guard.
- Information of guard include: guard code, first name of guard, last name of guard, email of guard, phone of guard.
- Information of manager room include: name of dom, Room ID , Guard Id, price have to pay for each semester.
### **Request:** 
-  Daily, guard need to caculate the total sutdent fined, caculate the total money.
-  Guard need check day student check-in, check out, day report item broken.
-  Monthly, guard need to count and display student not pay money for room.
-  Monthly, guard need cacule total amount collected.
-  Guard can check information of student.
- Guard can check room is emty for student register.
- Guard can check item broken in dom, in room to call fixer.
-  Check student register in room valid or invalid
- Check room valid in condition special when student register in room.
### **Entity relationship (ER)**
**Base on the problem description and management objectives, we can present several entities and attributes of the entity as follow:**
- Student: StudentID, GuardID, First Name, Last Name, Email, Phone, Gender, Course, Role, Country.
- Register: RoomID, StudentID, Check-In, CheckPrice.
- Room: RoomID , Name Dom, Floor, Location, Number Bed, Gender, Status.
- Fix Detail: RoomID, ItemID, Fixer, Date Report, Date Dix, Quantity.
- Items: ItemID, Name, Content, Price.
- Student Penalize: StudentID, PenalizeID, Date, Quantity.
- Penalize: PenalizeID, Name, Price.
- Guard: GuardID, First Name, Last Name, Email, Phone.
- Manager room: RoomID, GuardID, Name Dom, Price.

LINK:  HTTPS://GOO.GL/U4X3JO


