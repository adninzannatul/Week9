# Week9
1. Username Enumeration: For an existed username wrong input for password shows an error message in bold. But, for an username that does not exist the error message is not showed in bold. Thus a hacker can figure out if an username is existed. 
   - Gif walkthrough
         
 ![alt-text](User_Enumeration_1.gif)
 
 2. Insecure Direct Object Reference: It reveals staff info by directly eccessing the staff pages by their id
    - Gif walkthrough
   
 ![alt-text](IDOR.gif)
 
 3.  SQL Injection: 'OR SLEEP(8)=2--' extention in the url for staff info messes up with sql query to discover a vulnerability.
    - Gif walkthrough
    
 ![alt-text](sql_injection.gif)
 
 4. Cross-Site Scripting: Left a feedback in the contact option and wrote <script>alert("Zannat found XSS")</script> to for xss exploit.     Then logged in as admin and clicked on feedback which showed the alert message.
     - Gif walkthrough
                
![alt-text](Cross_Site_Scripting.gif)

5. Cross-Site Request Forgery: Left a link that is actually a hidden form in feedback. Then logged in as admin and went to the feedback. When the link is visited as an admin, the form gets submitted hacking the database.
     - Gif walkthrough
     
![alt-text](CSRF.gif)

6. Session Hijacking/Fixation: The website is visited from two different browsers. One is logged in as admin. Added the extention 'hackertools/change_session_id.php' in the existing url. It gave the logged in session id of the admin. The id is copied. Then same extention is used in the other browser which is not logged in as admin. The session id is changed to the admin's session id that was copied. Now, the user can press the login option and can access the account without having admin info. 
     - Gif walkthrough
     
  ![alt-text](Session_Hijacking.gif)   
