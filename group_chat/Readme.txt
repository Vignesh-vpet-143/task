#Group-chat application

 -This applications utilizes HTML,CSS,Javascript and PHP techniques. The database used is mySQL. 
 -Author: Vignesh M
 -Reference: Codepen,Stackoverflow

---------------------------------------------------------------------------------------------------------------------
Prerequisites to run the code:
---------------------------------------------------------------------------------------------------------------------
*mySQL database table with three fields : uname,msg,dt.(uname-sender,msg-message sent,dt-timestamp)
*XAMPP server for running Apache server and mySQL.
*text editors like Notepad or any framework for building frontend.
----------------------------------------------------------------------------------------------------------------------

->Database name used: chat_app
->Table name used: chats
->Fields in the table: uname (varchar),msg (varchar),dt (datetime)

----------------------------------------------------------------------------------------------------------------------

#Technical details:

-The HTML,CSS and Javascript is responsible for UI and the effects in it.
-The PHP code is written for storing the message in the database and retrieving it for displaying in the UI.

-----------------------------------------------------------------------------------------------------------------------

#Working of the application:

-Multiple users are allowed to comment in this application. 
-When the first user (A) comments, the comment is aligned to left side.
-If the same user (A) comments again (no intermediate chats), the comment is again aligned to left.
-If the user A comments, then user B comments, the comment of B will appear in right.Now if user A comments again, The previous sender is checked, if it is not the same user, then the current new chat will appear in the direction opposite to previous one.
-Thus chats will appear based on the previous chat bubble's alignment.

-----------------------------------------------------------------------------------------------------------------------

#Steps to run the code

-Cut this Group_chat.php file, paste on the following folder ---> C:\xampp\htdocs\newfolder\
-Open your browser.
-Type localhost/newfolder. The index of this directory will appear.
-Choose the Group_chat.php file.
-Type the name in 'from' text box, message in the nearby text box and click send.

-----------------------------------------------------------------------------------------------------------------------

#internal working

-Once you type and send a message, it will be uploaded into the database.
-On each page load, the messages will be retrieved from the database and will appear on the UI based on the conditions.

-----------------------------------------------------------------------------------------------------------------------