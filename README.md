# coursera-daily-selfie-screencast
Peer asignment screencast for "Programming Mobile Applications for Android Handheld Systems: Part 2" 

I made a big mistake on my last submission in DailySelfie.java:
```java
private void setUpList() {
    ((ListView) findViewById(R.id.selfies_list)).setAdapter(new SelfiesAdapter(this));
  }
```
should be replaced by:   
```java
private void setUpList() {
    selfiesAdapter = new SelfiesAdapter(this);
    ((ListView) findViewById(R.id.selfies_list)).setAdapter(selfiesAdapter);
  }
```

It shows the different features of the app:
* A click on the camera icon on the ActionBar open up a picture-taking app.
* It displays a list of all the selfies already taken.
* A click on the small view open up a large view.
* The image data is stored on the device. 
* An alarm can be set to remind the user to take a selfie.
