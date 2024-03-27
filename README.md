# Ex-02_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/b2520e34-8cd3-4673-b3ce-fe93a942c960)

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.




Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 ![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/ca43afcd-e3fb-421b-8dcc-004b1899ac2a)

 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/74b9d426-273b-400d-8dbc-0951341eccbf)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/063a343f-a1fe-4bf4-a5e7-d1347f6e82bf)

Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).
![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/3cf4637a-9130-4c7b-bb0c-96254ce1187c)



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.




Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
 ![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/a5a3bc48-b41c-4c50-8dba-977f799b1e7b)

 


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/d71e1675-b9c1-4cb7-80a0-472aa5c90111)


Step 6: An editing tab will open. Alter getHtml() method with the following.
 ![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/ac5a0bd8-9d3c-42ec-afd1-3b4be8f572f7)

 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/5538f2a8-0a6e-4089-90af-63612bc5d316)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 ![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/b4821522-4f3c-4130-baaf-9d0bdb97611e)

 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/8e62f1a3-08d0-4683-b2d0-21582885c77e)


Step 11: Save the project and build it.
![image](https://github.com/DhareeneRK/Ex-02_RESTful_Web_Services/assets/119434052/9c4ef959-3854-4817-9b8b-25bf54b6bf20)


Step 12: Run the JSP file and you should see the output in a new browser window.
 
 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
