
# Smart Connected Signs for Improved Road Safety using IBM Cloud

Smart Connected Signs uses IOT by taking input from sensors
( initially takes random values as data instead of real sensor 
data ) and weather API to shows smart signs about divergence , 
speed to be slow , moderate or fast , and weather.




## Features

- To replace the static signboards, smart connected signs are used.
- Smart signs get speed limitation data from web apps using weather API and updates automatically.
- Based on weather changes shows to increase or decrease the speed.
- Based on traffic and fatal situations the diversion signs are displayed
- Guide(Schools), Warning and Service(Hospitals, Restaurant) signs are also displayed accordingly.



## Setting up the Project:

To deploy this project run

**IOT WATSON PLATFORM**

- Device on IBM Watson IOT platform:

  Catlog=> Sevices=>Search and click "IOT platform"=> Select region=> create

  This creates IBM Watson IOT platform

  Now click on launch to launch IBM Watson IOT platform.

  Device=> Add Device/ Create device
- Enter:
  Device Type: This is device name
  Device ID: Give unique numerical ID

- Device Information: (If integrating with real hardware devices)
  Skip this as we are not using any real sensor or hardware

- Security: Add Authentication Token: 
  Click next as it is auto generated or add your own Authentication
  toke between 8 to 36 number
- Finish

*COPY YOUR DEVICE CREDENTIALS AND SAVE IT SOMEWHERE**

**CONNECT DEVICE TO ANOTHER PLATFORM**
Create API keys and authentication token
- Go to Apps
- Click on "generate API key"
- Role: Select "standard application"
*SAVE THE API KEY AND AUTHENTICATION TOKEN SOMEWHERE*

**DEVICE STIMULATOR:**
As we are not dealing with hadware so we have internal stimulator.

- Create Device stimulation
- Device type=>event name=> schedule(in how much time span you want to send data)
- Upload python code [code.py] in csv file
- Click on "Save"
- Use registered device (device we already created)=> select device
- Click on Device


**SEND DATA TO NODE RED UI**

- Catlog=> Software=> Search:  Node-RED App and select it
-  Get started=>Create
Clodant db is associated with your NODE-RED to store node red flows
- Deploy your app as Cloudfoundary App
- Create API=> next=> create
- Status: Success

Go to Dashboard=> Cloudfoundary app=> select your app
Visit App URL
Go to NODE RED FLOW EDITOR

- Create Nodes as shown 
- In IBM IOT NODE=> Update your api key info
- Deploy

- Click on right side URL button => Node Red UI Opens
Here you can see the data processed in NODE-RED DASHBOARD UI


**CONNECT NODE-RED with MIT INVENTOR APP**





```bash
  
```


## Weather API Used : OpenWeatherMap

Link: https://openweathermap.org/api
## Tech Stack

**Main:** IBM Cloud, IBM Watson Platform, NODE-RED (Cloudfoundary App)

**App Frontend:** MIT Inventor App

**App Backend:** NODE-RED and MIT Inventor App

IBM Cloud: https://www.ibm.com/cloud

Node-Red: https://nodered.org/

MIT App Inventor: https://appinventor.mit.edu/





## Screenshots

![App Front End](https://github.com/anjali-singh22/Smart-Road-Signs-using-IOT/blob/main/images/MITappFrontEnd.png)
![App Backend](https://github.com/anjali-singh22/Smart-Road-Signs-using-IOT/blob/main/images/MITappBackEnd.png)
Link to Demo Video: [Video Link](https://drive.google.com/file/d/1YFFMtgcBEdfzPaRbvu-Fll5EilfyA0Lc/view?usp=sharing)
