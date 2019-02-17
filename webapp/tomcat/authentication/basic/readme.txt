1. Update your conf/tomcat-users.xml with stuff in my tomcat-users.xml
2. You need to setup certificate for SSL because I am using the following (see web.xml):

   <user-data-constraint>
       <transport-guarantee>CONFIDENTIAL</transport-guarantee>
   </user-data-constraint>
   
   Alternatively, if you do not want to authenticate via SSL, use (not recommended):
   
   
   <user-data-constraint>
       <transport-guarantee>NONE</transport-guarantee>
   </user-data-constraint>
   
