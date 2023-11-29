# Github-Api-Demo-SmartOne
This is a test repository created as per the requirments laid down by SmartOne team.

###### The application uses the following components:
1. [Kotlin](https://kotlinlang.org/) as the base language.
2. [Retrofit]([https://developer.android.com/training/data-storage/room](https://square.github.io/retrofit/)) to fetch data from API.
3. [Dagger Hilt](https://dagger.dev/hilt/) as Dependency Injector.
4. [MVVM](https://developer.android.com/topic/architecture) with Clean architecture.
5. [Jetpack Compose](https://developer.android.com/jetpack/compose) for UI.
6. [Jetpack Navigation Compose](https://developer.android.com/jetpack/compose/navigation) for Navigation.
7. [Coil Compose](https://coil-kt.github.io/coil/compose/) for remote Image management.
8. [Splash Screen API](https://developer.android.com/develop/ui/views/launch/splash-screen) for Splash Screen.
9. [Mockito](https://github.com/mockito/mockito-kotlin) for Mocks.


## This is a simple application which uses internet permission in order to fetch user details from Github public API.

The flow is as following:
- On Start Up, the Splash Screen with animation is loaded.
- After that, default UserId is used to load my personal Github details and Repositories.
- On the same page i.e. Home Page, the user can also enter any other UserId in the TextField and click on Search button to fetch that user's Github details.
- If you click on any of the Repositories, then you will navigate to a new Compose Screen where details related to that repository is disaplyed.
- There are two buttons provided on this screen: 1. Visit Repository 2. Go Back.
  1. Visit Repository: This will open Github application as a Deeplink and navigate directly to the repository (if Github application is installed), else it will open the same in browser.
  2. Go Back: This will simply close the detail screen and go back to home screen.
 
Negative cases which are covered:
- If user clicks on Search button without entering anything in the TextField, an error will be shown.
- If there is no internet or the response fails, the corresponding error message will be shown.



   
