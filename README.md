# Kandy salesforce
This salesforce package encapsulates Kandy’s JS SDK and Restful APIs. Kandy is a product by GENBAND (www.genband.com) that utilizes WebRTC to enable peer to peer audio/video calls, chat, SMS and PSTN.

With this package, you can enable video and audio calling between two users that are logged into your salesforce application.

Think of pages where you anticipate users collaborating with each other, possibly to discuss content on those pages. Your users could start a video call with other online users and enhance the collaboration experience. Home page: http://www.kandy.io/

***
# Install package

Create an account on salesforce.com. Use this link to install the Kandy package to your application: 
<https://login.salesforce.com/packaging/installPackage.apexp?p0=04t28000000MeJH> 

Alternatively, you can deploy this package to your Salesforce application by checking out source code from github and deploy by using Force.com plugin for Eclipse.

# Configure package

##### Assign home page layout

- From Setup, click __Customize__ | __Home__ | __Home Page Layouts__.
- Click __Page Layout Assignment__.
- Click __Edit Assignment__.
- Choose the appropriate page layout: __Kandy Admin Layout__ for System Admin profile and __Kandy Home Layout__ for others.
- Click Save.

##### Configure custom sidebar

- From Setup, click __Customize__ | __User Interface__.
- Check __Show Custom Sidebar Components on All Pages__.
- Click Save.

##### Configure Kandy pages access permissions

- From Setup, click __Develop__ | __Pages__ click the __Security__ link of __Kandy Address Book__, __Kandy Widget__, __Video Call Answer__ pages and then add the profile you want to grant access permission. 

##### Configure Kandy API
- From Setup, click __Security Controls__ | __Remote Site Settings__ . Click on __New Remote Site__. Add link <https://api.kandy.io> to the __Remote Site Url__ input, the __Remote Site Name__ is whatever you want. Click __Save__. 
- From the Kandy Links widget on sidebar, click __Kandy Setting__ to configure Kandy Project API key, Project API secret and domain name. Please note that the project api key is different from account api key. Each project has an api key, which usually starts with DAK.

##### Assign Kandy user for each Salesforce user
- Click on __Kandy Assignment__ link on the __Kandy Links__ Sidebar Widget. Kandy Users will be fetched from server and assign automatically for the first time. Since the 2nd time, you can Get new Kandy Users by click the __Get Kandy Users__ button and assign users manually.
- You can click on __Auto Assign Users__ to assign Kandy Users to Salesforce users automatically or you can assign manually by clicking __New Assignment__ button.
- When you add a new user to your salesforce application, he should be assigned with a Kandy user automatically.
