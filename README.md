# pikachu
MyCape iOS/Android Developer candidate screening.

## Objective
- Write a simple iOS/Android mobile app. There is no time limit to complete this test however your speed, quality, and creativity will be greatly considered in the assessment. 
- The app will have 2 views: The splashScreen, the homeScreen.

## SplashScreen
- The splashScreen should display the "ryanair" loading during 2sec before displaying the homeScreen. https://www.ryanair.com/gb/en/


## HomeScreen

- Clicking back button should close the app.
- The homeScreen should display a list view and a GoogleMapView.
- Swiping right from the listView brings to the GoogleMapView.
- Swiping left from the GoogleMapView brings to listView.
  - By listView, we mean a view with a list. Not required to use "ListView." 
- You need to choose the best View for this use.
- The listview should display the list of airports fetched by calling: https://raw.githubusercontent.com/mwgg/Airports/master/airports.json
- The list needs to be sorted relative to the the current location of the user.
- The googleMapView should display the airports.
- Clicking on an item on the list should ask you (in a popup) to: 
  - look for the airport in google
  - Save this airport to favorite.
- By clicking on "Look for" + airportName + " in google" should open google and search for this airport.
- By clicking on "Save this airport  to favorite" should save this airport locally. When launching the app and reloading the     - list, the saved item in the list should have a different background colour.
- The pin in the googleMap should have a different colour as well.
- Clicking on an saved item should display the popup with 2 options:
  - look for the airport in google
  - Remove this airport from favorite.
- Only 1 item can be saved. An error message will be displayed.
- You should have a perfect error handling. Use cocoapods to manage dependencies (optional).

### Tests (Android only)

You you need to add unit tests for the HomeScreen only.
Coverage should be above 90%.

### Build (Android only)

The apk name in debug mode should be "MyCapeTest-Debug".
The apk name in release mode should be "MyCapeTest".
The BASE_URL for the API in debug mode should be "https://raw.githubusercontent.com/mwgg/".
The BASE_URL for the API in release mode should be "https://raw.githubusercontent.com/release/" (it won't work, but we want to see how you handle the BASE_URL given the mode)

### Requirements (Android only)

- Native Android (Java or Kotlin)
- Dagger 
- RxAndroid
- MVP (Model - View - Presenter)
- The code needs to have comments and be well structured. We will be very careful on the code quality and error handling.


## Submission
- You should have fork this repository and send us a `Pull Request` 
- Assign @ceosilvajr, @rogermolas and @skategui as a reviewer.
- PR `Title` should be in this format `{Name}, [Android,iOS]`
