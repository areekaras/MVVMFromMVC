# MVVMFromMVC

Learn how to convert an MVC app into MVVM. In addition, you’ll learn about the components and advantages of using MVVM.

[Checkout raywenderlich tutorial](https://www.raywenderlich.com/6733535-ios-mvvm-tutorial-refactoring-from-mvc)

## About MVVM

Model-View-ViewModel (MVVM)  is a design pattern that’s gained traction in the iOS development community in recent years. It involves a new concept called a  _view model_. In iOS apps, a view model is a companion object to a view controller.

[![Diagram that shows the layers of MVVM: Model, View, ViewModel](https://koenig-media.raywenderlich.com/uploads/2019/12/MVVM-Diagram-228x500.png)](https://koenig-media.raywenderlich.com/uploads/2019/12/MVVM-Diagram.png)

As shown above, the MVVM pattern consists of three layers:

-   _Model_: App data that the app operates on.
-   _View_: The user interface’s visual elements. In iOS, the view controller is inseparable from the concept of the view.
-   _ViewModel_: Updates the model from view inputs and updates views from model outputs.

MVVM offers some advantages over  _Model-View-Controller_, or  _MVC_, which is the de facto approach in iOS:

-   _Reduced complexity_: MVVM makes the view controller simpler by moving a lot of business logic out of it.
-   _Expressive_: The view model better expresses the business logic for the view.
-   _Testability_: A view model is much easier to test than a view controller. You end up testing business logic without having to worry about view implementations.

## What is in the project?

 1. Data binding using  box
 2. Create viewModel
 3. Format data
 4. Add functionality
 5. Unit testing 

## Getting started
The app fetches the latest weather information from weatherbit.io and presents a summary of the current weather.

To use the Weatherbit API, you need to register for a free API key. The app won’t work until you add your own Weatherbit API key. Go to  [https://www.weatherbit.io/account/create](https://www.weatherbit.io/account/create)  to register for your key.

After you get your API key, return to Xcode.

Under  _Services_, open  _WeatherbitService.swift_. Then replace the value for  _apiKey_  with your new key.
