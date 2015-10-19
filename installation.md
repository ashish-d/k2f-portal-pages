### Installation

Create an account on salesforce.com. Use this '[link]' to install the Kandy package to your application.

##### Configure package

- **Assign home page layout**
  - From Setup, click `Customize | Home | Home Page Layouts`.
  - Click `Page Layout Assignment`.
  - Click `Edit Assignment`.
  - Choose the appropriate page layout: `Kandy Admin Layout` for System Admin profile and `Kandy Home Layout` for others.
  - Click Save.

- **Configure custom sidebar**
  - From Setup, click __Customize__ | __User Interface__.
  - Check __Show Custom Sidebar Components on All Pages__.
  - Click Save.

- **Configure Kandy pages access permissions**

  - From Setup, click __Develop__ | __Pages__ click the __Security__ link of __Kandy Address Book__, __Kandy Widget__, __Video      Call Answer__ pages and then add the profile you want to grant access permission. 

- **Configure Kandy API**

  - From Setup, click __Security Controls__ | __Remote Site Settings__ . Click on __New Remote Site__. 
  - Add link 'https://api.kandy.io' to the __Remote Site Url__ input, the __Remote Site Name__ is whatever you want. 
  - Click __Save__. 
  - From the Kandy Links widget on sidebar, click __Kandy Setting__ to configure Kandy Project API key, Project API secret and domain name. Please note that the project api key is different from account api key. Each project has an api key, which usually starts with DAK.

- **Assign Kandy user for each Salesforce user**

  - When the widget __Kandy Links__ | __Kandy Assignment__ loads for the first time, it assigns Kandy users to Salesforce users automatically. Going forward, an administrator can maintain these associations using this link __Kandy Assignment__.

  - When you add a new user to your salesforce application, an un-assigned Kandy user wil be automatically assigned. If all Kandy users are already assigned, a new kandy user will be created.

[link]: <https://login.salesforce.com/packaging/installPackage.apexp?p0=04t28000000MeJH>
