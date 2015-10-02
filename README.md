# Kandy salesforce
This salesforce package encapsulates Kandy’s JS SDK and Restful APIs. Kandy is a product by GENBAND (www.genband.com) that utilizes WebRTC to enable peer to peer audio/video calls, chat, SMS and PSTN.

With this package, you can enable video and audio calling between two users that are logged into your salesforce application.

Think of pages where you anticipate users collaborating with each other, possibly to discuss content on those pages. Your users could start a video call with other online users and enhance the collaboration experience. Home page: http://www.kandy.io/

***
# Install package

Create an account on salesforce.com and using this link to install Kandy package to your application
<https://login.salesforce.com/packaging/installPackage.apexp?p0=04t28000000MeJH> 

You can either deploy this package to your Salesforce application by checking out source from github and deploy by using Eclipse Force.com plugin

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

##### Configure custom tab

- Kandy package has a custom tab to accessing Kandy Address Book page.
- From Setup, click __Manage Users__ | __Profiles__. Select the user profile you want to display the tab
- In __Tab settings__ section, change the value of __Kandy__ dropdown to __Default On__. Then click save.

- You can show Kandy custom tab by clicking the __(+)__ sign in the tab menu. 
- Click on __Customize my tabs__ button. Select the page you want Kandy tab to display, and then select __Kandy__ on the left panel and move tho the right panel.

##### Configure Kandy pages access permissions

- From Setup, click __Develop__ | __Pages__ click the __Security__ link of __Kandy Address Book__, __Kandy Widget__, __Video Call Answer__ pages (pages required to use Kandy functionalities) and then add the profile you want to grant access permission. 

##### Configure Kandy API
- From Setup, click __Security Controls__ | __Remote Site Settings__ , Click on __New Remote Site__ to add new Remote site, Add link <https://api.kandy.io> to the __Remote Site Url__ input, the __Remote Site Name__ is whatever you want. Click __Save__. 
- From the Kandy Links on sidebar, click __Kandy Setting__ (Or Access the link <https://YOUR_SALESFORCE_APP_URL/apex/KandySettings>) to configure Kandy API. Your need to provide __API_KEY__, __API_SECRET__, __DOMAIN_NAME__ exactly in order to Kandy work properly.

##### Assign Kandy user for each Salesforce user
- Next, You need to assign for each user in your App a Kandy Account
- Click on __Kandy Assignment__ link on the __Kandy Link__ Sidebar Widget. Kandy Users will be fetched from server and assign automatically  for the first time. Since the 2nd time, you can Get new Kandy Users by click the __Get Kandy Users__ button and assign user manually.
- You can click on __Auto Assign Users__ to assign Kandy Users to Salesforce users automatically or you can assign manually by clicking __New__ button.
- If you setup Kandy package correctly, when you add a new user to your application, he should be assigned with a Kandy user automatically.
