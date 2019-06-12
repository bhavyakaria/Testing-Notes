# Testing-Notes
Contains notes on software testing.

There are various types of testing, like Unit, Integration and Functional(E2E) testing.

## Unit Testing

* Generally for testing  small piece of code, isolated and alone.
* If writing unit test is hard then it means your code is poorly designed. So it also helps  in writing better code.
* They are also great for preventing regressions - bugs that occur repeatedly.
* Unit testing is used in TDD. Its like a backbone.
* If an app needs to make a successful database connection then it can't be test with unit testing.
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


## Resources

* [Appium vs Espresso](https://www.reddit.com/r/androiddev/comments/b50upz/appium_or_espresso_for_qa_team/)
* [Testing Robots by Jake Wharton](https://academy.realm.io/posts/kau-jake-wharton-testing-robots/)
* [Fundamental of Testing](https://developer.android.com/training/testing/fundamentals)
* [Android Testing Patterns](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc-6HWg_jyP0U1zrVLHn65b2)

