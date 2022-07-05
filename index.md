## Healbar -- The Mental & Health Symptom Checker

Healbar is an app providing you with possibility to score your everyday health. This is made by an symptom checker engine which is used to recognize your state and possible illnesses. As a result you should get your overall _score_ of health and recommendations what to improve in order to put your score higher.

Healbar will work on several platforms including Web, Mobile and possibly wearables. This is explained later.

### Engine

The app engine is going to be provided by external REST API. After long debate it is decided that it's going to be **Infermedica API** which gives many opportunities including: symptom checker, chatbot, voice input and natural language recognition. This API is well known and reliable, as well as compliant with safety rules. For first 2000 calls/month API is free to use and limited to English localization. 

### Technology

**Web Stack**
To build the web app it is considered the best to build it upon **ReactJS** library within MUI framework or Syncfusion. Those UI frameworks provide multiple reusuable components, which help to build beautiful UI/UX layer with less work. The app will make API POST/GET calls to the engine in order to get all needed informations.

**Mobile Stack**
Mobile app will be based on **Flutter**, Dart language based, multiplatform framework. This way it's going to be possible to build an app for every most-used mobile OS within one codebase. 

**Backend**
User profiles and management will be done using **Firebase**. Later in the proccess, we will add Analytics support in-app and other insights addons to improve user experience.

### How deos it look like for the user? ###

App users will be able to create their unique profiles where they can store their basic informations and results. On web, it will be also possible to check your symptoms without signing up - in form of one time quiz.

After signing up user will fill in informations needed by the API algorithm: age, sex, occupation, etc. These will be remembered and used later everytime when calling the API. 

There are going to be several ways to provide Engine with data:
- Quiz (Web)
- Chatbot based symptom checker (Web & Mobile)
- Daily diary (Web & Mobile)
- Daily questions / Push notifications (Mobile only)
- State tiles / How do you feel now? (Web & Mobile)

User will have access to it's own dashboard. It will be possible to find there Quick Actions (Tiles/Take Quiz/Write in Diary), chart with actual Healbar Score (scale which makes it visually easy to know on which health level user is), user history and section with results and recommendations. 
Later it is possible to add an integration with healthcare providers in order to give those informations straight to the doctor to whom it will be possible to make an appointment through the app.

**Daily diary**
User will be able to provide the engine with handwritten or voice inputted diary. This will require him to explain how did he feel during the day, if there were any pains, problems or symptoms that made his attention. The engine, using natural language recognition, will highlight most important for algorithm informations and basing on those, present the diagnosis. Taking in consideration the _power_ of possible sickness will increase or decrease the health score. Also, if there will be any infomrations on positive behavior, they will also be taken into consideration in order to raise the score.

**Daily questions**
If agreed, user will get push notifications with CTA to fill the diary or answer few short questions in a survey. This way in fast way, the health score can be monitored regularly and in convenient way. 

User can also agree for tracking and get personalized notifications, for example: app detected that user spend 3 hours in a pub -> this will fire the notification after arriving home/in the end of the day/specified by the user time -> user will answer the question (e.g. How many drinks did you have?) -> basing on the answer adjust the score. In similar way it can also get sport activity from other apps or basing on built-in tracker.

**State Tiles**
Easy to access and understand tiles with the most relevant feelings/symptoms that user can pick on home screen of the app. By tapping/clicking the tile user provides the algorithm with good starting point to diagnose later. If the tile belongs to crucial symptoms it will fire more detailed health checkup (Quiz/Chatbot).



