# Testing-Notes
Contains notes on software testing.

There are various types of testing, like Unit, Integration and Functional(E2E) testing.

## In a gist

* Unit Testing -> For testing any small _piece_ of code
* Integration Testing -> For testing any small _component_ of the application
* Functional Testing -> For testing the complete flow of the application(Basically automating the manual testing/ replicating the user actions)

## Unit Testing

* Generally for testing small piece of code, isolated and alone.
* If writing unit test is hard then it means your code is poorly designed. So it also helps  in writing better code.
* They are also great for preventing regressions - bugs that occur repeatedly.
* Unit testing is used in TDD. Its like a backbone.
* If an app needs to make a successful database connection then it can't be tested with unit testing.
* In procedural code, the units are often functions, in object oriented code, the units are classes.
* They are fast + cheap.

## Integration Testing

* Its to test how parts of the system work together - the integration of the parts.
* It's similar to unit test with one difference: while unit tests are isolated from other components, integration tests are not.
* They are complex and slower compared to unit test.
* You should have fewer integration test compared to unit test.
* If an app needs to make a successful database connection then it can be tested in integration testing.
* They are slow + expensive

## Functional Testing

* Testing the complete functionality of the application by using some tool to automated a browser/mobile.
* Do not make them fine-grained, as they can become a nightmare to maintain.
* They are used when you want to test a complete flow like registering a user, making a payment and redirecting to proper pages, etc
* They are slow + expensive
* They require less maintenance and cover a bigger part of your application with saving you a lot of time.

## Testing on Android

There are three types on android
1. Unit(test) - JUnit5/ Mockito
2. Intrumentation(androidTest) - JUnit/ Mockito
3. UI(androidTest) - Expresso(Internal)/ Appium(External)

#### 1. Unit

* Runs on Local Computer
* It runs on JVM
* Very fast because emulator is not needed.
* It's for testing java code

#### 2. Intrumentation

* Similar to local unit tests
* Used for testing android specific stuff like activity, fragments, context, serviecs, etc
* Need to run on real device or emulator(Roboelectric is used if you don't want to run it on emulator)

#### 3. UI

* Simulates the user flow  	
* Tests the complete user journey from  high level

### Mockito

* Mocks the RestAPI/Database part in the methods/functions

### Espresso vs Appium

| Criteria 	    	   | Espresso      | Appium        						    |
| :----------------------: | :-----------: | :------------------------------------------------------------: | 
| Language          	   | Java          | Many(Java, Python, Javascript, any that can make HTTP request) |
| Supports          	   | Android Only  | Web, Android and iOS 					    |
| Testing Philosopy 	   | Grey Box      | Black Box							    |
| Speed 	    	   | Fast	   | Slow compared to Espresso					    |
| Ease Of Setup     	   | Easy	   | Hard							    |
| Dependencies On Code     | Yes	   | No								    |
| Ease Of Writing Tests    | Easy for devs | Easy for testers						    |
| Backers		   | Goolge	   | Open Source						    |
| Suitable For		   | Android devs  | Testers/ QA testing Android & iOS apps			    |


## Resources

### Official Docs
* [Fundamental of Testing](https://developer.android.com/training/testing/fundamentals)

### Misc 
* [Appium vs Espresso](https://www.reddit.com/r/androiddev/comments/b50upz/appium_or_espresso_for_qa_team/)

### Videos
* [Testing Robots by Jake Wharton](https://academy.realm.io/posts/kau-jake-wharton-testing-robots/)
* [Android Testing Patterns](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc-6HWg_jyP0U1zrVLHn65b2)

### Podcasts
* [Welcome & Testing in Android](https://fragmentedpodcast.com/episodes/1/)
* [Corey Latislaw on TDD and Testing](https://fragmentedpodcast.com/episodes/13/)
* [Junit4 tricks with Parameterized Enclosing tests](https://fragmentedpodcast.com/episodes/052/)
* [Chiu-Ki Chan explains Mocking and Stubbing with Mockito](https://fragmentedpodcast.com/episodes/059/)

### Books

* [WorkingEffectivelyWithLegacyCode](https://archive.org/details/WorkingEffectivelyWithLegacyCode)
