# Important Components Individually Working


# DPC

- DPC is currenlty being splited into  DPC_core,DPC_full,DPC_experimental 

|    COMPONENT     |    STATUS                       |     CONDITION                                                     |
|------------------|---------------------------------|-------------------------------------------------------------------|
|  DPC core        | Actual part covering device     | Working,TESTING INTERNALLY                                        |
|  DPC full        | App when every component works  | Different components being TESTED individually , NOT YET COMPLETE |
| DPC EXPERIMENTAL | DPC core + component            |  Current stage of DPC FULL when its partially working             |


# STATUS


|    COMPONENT     |    STATUS                   |     CONDITION               |
|------------------|-----------------------------|-----------------------------|
|  DATA API        |  REST API WORKING           |           ONLINE            |
|  FIREBASE        |   WORKING                   |            WORKING          |
|   APP LAYER      |   #1 WORKING                |      TESTING #2             |
|   FORM           |   WORKING                   |      TESTING #4             |
| UPI DEEP         | WORKING                     |  NOT IMPLEMENTED            |
| UUID             | working in all layers       | JS,PYTHON,ANDROID           |
| DATABASE         |  WORKING                    | MYSQL and REDIS,FIREBASE already implememnted |

## APP LAYER (COMPONENTS present in APP as MODULE)

|    Serial        | Component being Tested               |     CONDITION                                                     |  
|------------------|--------------------------------------|-------------------------------------------------------------------|
|  #1              |STORAGE API,VIEWER,DASHBOARD,FIREBASE |   CURRENTLY being tested as [File Manager](https://github.com/Kivtechmain/filemanager)                          |
|  #2              | GEOLOCATION as GPS and GNSS          |  GPS being tested as [SMS GPS SERVICE](https://github.com/Kivtechmain/GPS),[GNSS](https://kivtechmain.github.io/GNSS/gnss.apk)        |
|  #3              | USER FORM                            |   BEING TESTED INTERNALLY                                         |
|  #4              |  PRIVILIGES                          |   BEING TESTED INTERNALLY                                         |
|  #5              |   DPC                                |   WORKING,BEING TESTED INTERNALLY, as DPC core                    |
|  #6              |   AUTO UPDATE                        | NOT WORKING                                                       |
|  #7              | USER INTERFACE,DASHBOARD             |  ONLINE WORKING(js),ANDROID ,NOT LINKED        |
|  #8              |  REST API                            | ONLINE (JS), Linked with DASHBOARD ,ANDROID IMPLEMENTED,NOT TESTED|
|  #9              | CRYPTOGRAPHY                         | FERNET module,works whats documented [CRYPTOGRAPHY](https://github.com/norkator/cryptography),different module used in JS |                                                   |
|  #10             |  GEOLOCATION view as [GOOGLE MAP](https://kivtechmain.github.io/google_map/),[MAPBOX](https://kivtechmain.github.io/mapbox/)| DASHBOARD view for both ONLINe(JS) and Android                  |
|  #11             | PAPER DASHBOARD,MATERIAL DASHBAORD   | Dashboard + UI for both our APP and ONLINE {JS} , [GNSS](https://github.com/Kivtechmain/GNSS/gnss.apk)  has material dashboard #2                  |
|  #12             |   [USER DASHBOARD](https://kivtechmain.github.io/user_dash_android/user_dash.apk)                      | PROTOTYPE AVAILABLE  UI #3,UI understandable by anyone |
| #13              |   CHATBOT                             | IBM WATSON as chatbot_1,CHATGPT/OPENAI   as chatbot_2                 |


## UNDERSTANDING APP LAYER (NOT TO BE INCLUDED),TESTING PURPOSE ONLY 

|    Serial        | Component being Tested               |     CONDITION                                                     |  
|------------------|--------------------------------------|-------------------------------------------------------------------|
|  #14             |  DEVICE FULL ACCESS                  | BEING TESTED with [SUPERSU](https://supersuroot.org/), CURRENLTY ROOTED DEVICE WORKS   |
|  #15             |  SYSTEM CALLS MONITORING             | BEING TESTED with [SIZUKU](https://github.com/RikkaApps/Shizuku),API CALL without ADMIN,PID shared  |
|  #16             |  [UPI DEEP INTEGRATION](https://github.com/Kivtechmain/deep_upi/blob/main/README.md)              | WORKING INDIVIDUALLY.INTERNALLY TESTED,NOT IMPLEMENTED YET        |
