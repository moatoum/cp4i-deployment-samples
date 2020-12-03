# Configuring the ServiceNow Connector

This is a placeholder for instructions to configure the ServiceNow Connector.

## Setting up the Service Now

To get started you will require admin level access to your ServiceNow
account. If you want to create a free ServiceNow account to test out App
Connect, you'll have to
[register](https://developer.servicenow.com/dev.do#!/home)
(https://developer.servicenow.com/) for a ServiceNow Account. Once your
account is activated, you can request a ServiceNow personal developer
instance.

Once your account is activated, you can request a ServiceNow free
developer instance.

![Graphical user interface, website Description automatically
generated](images/image1.png)

Click on 'Request an Instance' and select the location of your instance.

![Graphical user interface Description automatically
generated](images/image2.png)

Click on 'Request'. This will only take a few seconds.

![Graphical user interface, application Description automatically
generated](images/image3.png)

Please note your instance URL and credentials. You will need these later
when we configure the ServiceNow connector.

![Graphical user interface, text, application, email Description
automatically generated](images/image4.png)

Click on 'Open Instance'

![Graphical user interface, text Description automatically
generated](images/image5.png)

Search for Registry in 'Filter Navigator' search bar and then select
'Application Registry'.

![A screenshot of a cell phone Description automatically
generated](images/image6.png)

We will create an OAuth API endpoint for external clients. Click on
'New'.

![Graphical user interface, application Description automatically
generated](images/image7.png)

Select 'Create an OAuth API endpoint for external clients'.

![Graphical user interface, text, application, chat or text message
Description automatically
generated](images/image8.png)

In the config panel give it a unique name and hit submit.

![Graphical user interface, text, application, email Description
automatically generated](images/image9.png)

This will create a new OAuth endpoint with Client ID and Client Secret
generated. You can view these details by clicking and viewing the new
endpoint. You will be providing Client ID and Client Secret

![Graphical user interface, text, application, email Description
automatically generated](images/image10.png)

Great! We've now a running ServiceNow instance with an Oauth
app/endpoint registered for it which represents our App Connect!

Please keep in mind that this is a free developer instance, it will be
reclaimed in 10 Days and also to support the developer program,
instances hibernate when they are idle. But you can easily restore
instance from the reclaimed instance\'s backup. Similarly, you can
easily wake up a hibernating instance. (Learn more;
<https://developer.servicenow.com/dev.do#!/guides/orlando/now-platform/pdi-guide/understanding-pdis>)

You'll be later asked for the following details about your ServiceNow
instance and Oauth endpoint to integrate with the service. Please keep
them safe.

-   The URL of your ServiceNow instance, in the following form:
    https://\<servicenow-id\>.service-now.com/

-   The username and password that you use to log in to the instance.

-   ClientID and Secret of your ServiceNow application (Oauth endpoint).
