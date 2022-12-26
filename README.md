![DataverseForNinjaOne](https://user-images.githubusercontent.com/47614276/209544038-e8faa894-a9a6-4f8f-997d-a2a5c0a680db.png)
<p align="center">
  <a href="https://www.paypal.com/donate/?hosted_button_id=PLM7Q4RRJK48N" target="_blank">
    <img src="https://img.shields.io/badge/Donate-PayPal-green.svg"/>
  </a>
</p>

---

# Dataverse for NinjaOne
## What is this?
This is a custom Dataverse connector for [Microsoft Power Apps](https://powerapps.microsoft.com/) and [Microsoft Power Automate](https://powerautomate.microsoft.com/) to connect to the data of [NinjaOne](https://www.ninjaone.com/).<br>
This is done using the [NinjaOne public API](https://app.ninjarmm.com/apidocs/) provided by NinjaOne.

## What does it do?
It allows you to get data from NinjaOne inside of you Microsoft Power App.

## Client App setup
1. In Ninja, navigate to `Administration` > `Apps` > `API` or click [here](https://eu.ninjarmm.com/#/administration/apps/api) (EU instance)<br>
and click on `Add` to create a new Client app
2. Fill in the Application Configuration as shown below<br>
![Screenshot 2022-12-26 122155](https://user-images.githubusercontent.com/47614276/209543481-de3b9030-fe69-489d-ad2c-4ed3b1aefa1a.png)
3. Click on `Save` and take note of the client secret
4. Click on `Close` and then take note of the client ID

## Connector creation
1. Go to [make.powerapps.com](https://make.powerapps.com) and open `Dataverse` > `Custom Connectors`
2. Click on `New custom connector` > `Import an OpenAPI file` and select the DataverseForNinjaOne.swagger.json file from this repo.
3. Fill the `1. General` tab with your NinjaOne URL and the `2. Security` tab as shown below:<br>
![items (2)](https://user-images.githubusercontent.com/47614276/209540765-185bd034-3394-414d-a536-a54c9988b2d9.png)
5. Click on `Create connector` 

## Start using the connector
You can now use NinjaOne as a datasource in your Power Apps and Power Automate!<br>
Note that the data link is not live, meaning you need to call the endpoints any time you want the latest data.<br>
![items (3)](https://user-images.githubusercontent.com/47614276/209540829-96a40893-29f7-471d-9912-0956409ef06c.png)
