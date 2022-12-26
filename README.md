# Dataverse for NinjaOne

## What is this?
This is a custom connector for [Microsoft Power Apps](https://powerapps.microsoft.com/en-us) to connect to the data of [NinjaOne](https://www.ninjaone.com/).<br>
This is done using the [NinjaOne public API](https://app.ninjarmm.com/apidocs/) provided by NinjaOne.

## What does it do?
It allows you to get data from NinjaOne inside of you Microsoft Power App.

## Client App setup
1. In Ninja, navigate to `Administration` > `Apps` > `API` or click [here](https://eu.ninjarmm.com/#/administration/apps/api) (EU instance)<br>
and click on `Add` to create a new Client app
2. Fill in the Application Configuration as shown below<br>
![items](https://user-images.githubusercontent.com/47614276/209540565-18bf3063-1672-41bb-a89b-21bc285ca835.png)
3. Click on `Save` and take note of the client secret
4. Click on `Close` and then take note of the client ID

## Connector creation
1. Go to [make.powerapps.com](https://make.powerapps.com) and open `Dataverse` > `Custom Connectors`
2. Click on `New custom connector` > `Create from blank` then give your connector a name and click on `Continue`
3. Click on `Swagger Editor` and replace the contents ofthe swagger editor with the contents of NinjaOne.swagger.json
![items (1)](https://user-images.githubusercontent.com/47614276/209540649-ab70525a-dd4d-4c03-af57-814c52a790a4.png)
4. Close the swagger editor and fill in the `2. Security` tab as shown below<br>
![items (2)](https://user-images.githubusercontent.com/47614276/209540765-185bd034-3394-414d-a536-a54c9988b2d9.png)
5. Click on `Create connector` 

## Start using the connector
You can now use NinjaOne as a datasource in your Power Apps!<br>
Note that the data is not live, and it is best to store the data in a local collection and updating that collection when needed.<br>
![items (3)](https://user-images.githubusercontent.com/47614276/209540829-96a40893-29f7-471d-9912-0956409ef06c.png)
