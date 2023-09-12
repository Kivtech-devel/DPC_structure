# Important Components Individually Working

- project halted as to internal design changes and API changes to ANDROID EMM API


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
|  DATA API        |  REST API WORKING           |           ONLINE,[mock api](https://firebase-link-nodejs.vercel.app/)            |
|  FIREBASE        |   WORKING                   |            WORKING,[mock api](https://firebase-link-nodejs.vercel.app/)           |
|   APP LAYER      |   #1 WORKING                |      TESTING #2             |
|   FORM           |   WORKING                   |      TESTING #4             |
| UPI DEEP         | WORKING                     |  NOT IMPLEMENTED            |
| UUID             | working in all layers       | JS,PYTHON,ANDROID           |
| DATABASE         |  WORKING                    | MYSQL and REDIS,FIREBASE already implememnted.Trying SQLITE as it can also work  |
| JSON             | DATA component,required     | PYTHON,JS,PHP supports its natively,android doesnt have any so utilizing packages [GSON](https://github.com/google/gson) , [JACKSON](https://www.baeldung.com/jackson) |
| DROPDOWN/ANDROID FORM|  REQUIRED,ANDROID           |Though forms can be build with tables,class,div using css and js for HTML and can be easily used by PHP by embedding it.In Android either we can use the same JS,CSS through WEBVIEW or optionally create a layout  |

## APP LAYER (COMPONENTS present in APP as MODULE)

|    Serial        | Component being Tested               |     CONDITION                                                     |  
|------------------|--------------------------------------|-------------------------------------------------------------------|
|  #1              |STORAGE API |   CURRENTLY being tested as [File Manager](https://kivtech-devel.github.io/filemanager)                          |
|  #2              |VIEWER,DASHBOARD |   CURRENTLY being tested as [File Manager](https://kivtech-devel.github.io/filemanager)                          ||  #3              |FIREBASE |   CURRENTLY being tested as [File Manager](https://kivtech-devel.github.io/filemanager) ,also using NODEjs,[mock api](https://firebase-link-nodejs.vercel.app/)                         |
|  #4              | GEOLOCATION as GPS and GNSS          |  GPS being tested as [SMS GPS SERVICE](https://kivtech-devel.github.io/GPS),[GNSS](https://kivtech-devel.github.io/GNSS/gnss.apk)        |
|  #5              | USER FORM                            |   BEING TESTED INTERNALLY                                         |
|  #6              |  PRIVILIGES                          |   BEING TESTED INTERNALLY                                         |
|  #7              |   DPC                                |   WORKING,BEING TESTED INTERNALLY, as DPC core                    |
|  #8              |   AUTO UPDATE                        | NOT WORKING                                                       |
|  #9              | USER INTERFACE,DASHBOARD             |  ONLINE WORKING(js),ANDROID ,NOT LINKED        |
|  #10              |  REST API                            | ONLINE (JS), Linked with DASHBOARD ,ANDROID IMPLEMENTED,NOT TESTED|
|  #11              | CRYPTOGRAPHY                         | FERNET module,works whats documented [CRYPTOGRAPHY](https://github.com/norkator/cryptography),different module used in JS |                                                   |
|  #12             |  GEOLOCATION view as [GOOGLE MAP](https://kivtech-devel.github.io/google_map/),[MAPBOX](https://kivtech-devel.github.io/mapbox/)| DASHBOARD view for both ONLINe(JS) and Android                  |
|  #13             | PAPER DASHBOARD,MATERIAL DASHBAORD   | Dashboard + UI for both our APP and ONLINE {JS} , [GNSS](https://kivtech-devel.github.io/GNSS/gnss.apk)  has material dashboard #2                  |
|  #14             | DATABASE#2                           | PHP/MYSQL|
|  #15             |   [USER DASHBOARD](https://kivtech-devel.github.io/user_dash_android/user_dash.apk)                      | PROTOTYPE AVAILABLE  UI #3,UI understandable by anyone [4*2](https://kivtech-devel.github.io/user_dash_android/user_dash.apk)  [5*2](https://kivtech-devel.github.io/user_dash_android/user_dash_10.apk)|
| #16              |   CHATBOT                             | IBM WATSON as chatbot_1,Currently testing as NODE js APP,PYTHON App and Android App ,CHATGPT/OPENAI   as chatbot_2,currently testing as PYTHON APP  |


## UNDERSTANDING APP LAYER (NOT TO BE INCLUDED),TESTING PURPOSE ONLY 

|    Serial        | Component being Tested               |     CONDITION                                                     |  
|------------------|--------------------------------------|-------------------------------------------------------------------|
|  #17             |  DEVICE FULL ACCESS                  | BEING TESTED with [SUPERSU](https://supersuroot.org/), CURRENLTY ROOTED DEVICE WORKS   |
|  #18             |  SYSTEM CALLS MONITORING             | BEING TESTED with [SIZUKU](https://github.com/RikkaApps/Shizuku),API CALL without ADMIN,PID shared  |
|  #19             |  [UPI DEEP INTEGRATION](https://github.com/Kivtechmain/deep_upi/blob/main/README.md)              | WORKING INDIVIDUALLY.INTERNALLY TESTED,NOT IMPLEMENTED YET        |


## Programming languages being USED


|    Serial        |    LANGUAGE                          |     PURPOSE/USED FOR                                              |  
|------------------|--------------------------------------|-------------------------------------------------------------------|
|  1               |  HTML                                | WEB PAGES/DASHBOARD                                               |
|  2               |  JS                                  | Logic in webpages/DASHBOARD and as NODEJS in REST API,NODEAPP     |
|  3               |  CSS                                 | Style Sheet for WEB PAGES/DASHBOARD                               |
|  4               |  PHP                                 | As SERVER,API,connection to MYSQL DATABASE                        |
|  5               |  SQL                                 | As  MYSQL SERVER/PHP,database                                     |
|  6               |  JAVA                                | For Android Studio/Android APPS                                   |
|  7               |  KOTLIN                              | For Android Studio/Android APPS                                   |
|  8               |  PYTHON                              | For testing using cases/AI/ML,logic and design                    |
