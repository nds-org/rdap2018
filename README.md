# Labs Workbench Tutorial

## Workbench basics

This section will walk you through the basics of Labs Workbench including signing in, viewing the catalog, adding and starting applications.

Open a browser and go to https://www.workshop1.nationaldataservice.org

![](/images/01landing.png)

On the landing page, select one of the Sign In links. Enter the provided credentials. After logging in, you'll be taken to an empty dashboard. Select "Add an Application" or the Catalog link to view the available applications.

![](/images/02applications.png)

This catalog contains a number of applications. Clowder, Mongo, and RabbitMQ are all building blocks for the Clowder application. Jupyter, PostgresSQL Studio, RStudio Server, and Visualization tools are all example environments for accessing the DataDrivenAg data.

![](/images/03catalog.png)

## Using Jupyter

From the catalog page, select the "Add" link on the Jupyter card, then select "View" or "Applications" to go to your dashboard.

![](/images/04jupyter.png)

You will see a stopped instance of a Jupyter environment.  Select the "Launch" button to start it.

![](/images/05endpoint.png)

This will start a private instance of Jupyter with some tutorial materials and sample data. Browse to "work / tutorials / height_prediction" and load the "Height_Prediction_Example.ipynb" notebook.  

![](/images/06notebook.png)

This is a sample notebook provided by a machine learning collaborator on the TERRA-REF project to demonstrate how to build predictive models for plant heights from sample data.

Feel free to explore the Jupyter environment.  Browse back to "work / shared / terraref / sites / ua-mac" to view some of the data available to users. Beware -- some of the files and directories are quite large!

## Exploring Clowder

Clowder is an active data management, intended to support collaboration and sharing while collecting metadata along the way.  Clowder has an extensible "extractor" framework that can be used to extract metadata or process files automatically.  We'll just touch the surface with this example.

From the Catalog, select "Add" on the Clowder card.
![Landing](/images/07clowder.png)

On the dashboard select "Image Preview extractor" and "Add service". 
![Landing](/images/08addservice.png)

You'll be prompted to configure the service, but you can accept the defaults and save.

![Landing](/images/09configureservice.png)

Select launch and wait for the services to start.  This will take a minute (or 3).  Once started, select the endpoint link.

![Landing](/images/10endpoint.png)

This is now a private Clowder sandbox for you to explore.  Select the "Sign Up" link and enter your email (you'll go through a validation step, so check your mail)

![Landing](/images/11signup.png)

Click on the link in your email and enter your user information to Sign Up.
![Landing](/images/12signup.png)

Sign in and select "Create > Dataset" to create a sample dataset.

![Landing](/images/13createdataset.png)

Enter some sample metadata. 

![Landing](/images/14createdataset.png)

Since we've enable the preview extractor, select "Add Files" to upload an image (feel free to try the one in this repo).
![Landing](/images/15uploadfile.png)

View the dataset. Note the ability for users to add custom metadata at the dataset or file level.
![Landing](/images/16viewdataset.png)

Select the file link and note the extraction events. The extractors leave a provenance trail of all actions taken.

![Landing](/images/17viewevents.png)
