INSERT INTO students   VALUES ("Mary","101");
INSERT INTO students   VALUES ("Jordan","102");
INSERT INTO students   VALUES ("Lisa","103") ;
INSERT INTO students   VALUES ("Mike","104") ;
INSERT INTO students   VALUES ("Bill","105") ;
INSERT INTO students   VALUES ("Polly","106") ;
INSERT INTO students   VALUES ("Jenna","107") ;
INSERT INTO students   VALUES ("Mitch","108") ;
INSERT INTO students   VALUES ("David","109") ;




INSERT INTO classes   VALUES ("java","B230", "MON_AM", "1103");
INSERT INTO classes   VALUES ("csharp","B122", "Tue_PM", "1247");
INSERT INTO classes   VALUES ("Math","A506", "WED_EV", "1389");
INSERT INTO classes   VALUES ("Database","B123", "TUE_PM", "1455");
INSERT INTO classes   VALUES ("projtMng","B125", "FRI_PM", "1203");
INSERT INTO classes   VALUES ("EmgTech","B122", "FRI_EV", "1103");
INSERT INTO classes   VALUES ("csharp","B125", "FRI_PM", "1451");
INSERT INTO classes   VALUES ("Math","E111", "WED_AM", "1673");



INSERT INTO enrollments   VALUES ("101","1103");
INSERT INTO enrollments   VALUES ("102","1247");
INSERT INTO enrollments   VALUES ("103","1389");
INSERT INTO enrollments   VALUES ("104","1455");
INSERT INTO enrollments   VALUES ("105","1203");
INSERT INTO enrollments   VALUES ("106","1158");




Select students.studentname,students.studentid,classes.classname,classes.datetime,classes.classid
from students,classes,enrollments
where students.studentid=enrollments.studentid and classes.classid=enrollments.classid
