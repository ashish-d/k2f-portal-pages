# Introduction
 
This Salesforce package encapsulates Kandy’s JavaScript SDK and REST APIs. With this package, you can enable video and voice calling between two users that are logged into your Salesforce applications. Kandy (http://www.kandy.io/)  is a communications Platform as a Service (PaaS) that quickly enhances software applications with real time communications to deliver a more human and context-based experience. Kandy's cloud-based features enable companies to seamlessly embed voice, video, rich messaging, presence, co-browsing, and screen sharing into Web and mobile applications.

With this package Salesforce users can collaborating with their colleagues, partners or customers on any page such as Accounts, Contacts or Chatter. Users can start a voice or video call with other online users and enhance the collaboration experience. They can send an SMS to other users having an SMS enabled phone and make PSTN phone calls.

***
# Install package

Create an account on <https://www.salesforce.com>. Use this link to install the Kandy package to your application: 
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
- When the widget __Kandy Links__ | __Kandy Assignment__ loads for the first time, it assigns Kandy users to Salesforce users automatically. Going forward, an administrator can maintain these associations using this link __Kandy Assignment__.
- When you add a new user to your salesforce application, an un-assigned Kandy user wil be automatically assigned. If all Kandy users are already assigned, a new kandy user will be created.
