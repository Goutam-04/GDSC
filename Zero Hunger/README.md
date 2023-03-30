# FEED INDIA - An webpage that connects NGO and volunteers

<b> PROBLEM STATEMENT </b>

India has been grappling with the problem of zero hunger for decades, with millions of people facing food insecurity and malnutrition. Despite various government initiatives and interventions, the issue persists due to factors such as poverty, inequality, and lack of access to resources , whereas the food in the resturant is getting wasted.
All they need are volunteers and support from the resturant's co-operation to getting that wasted food.
Our website acts as an intermediary between an NGO and an individual resturant willing to contribute, thus easing out connectivity and accessibility.

<b> PROPOSED SOLUTION </b>

The Website asks users to register giving them options to log in as an NGO or as a Resturant and a special donate button for those who want to help with their money.
It first lists down the NGOs at a particular location giving access to two types of users of our app ie,<br>
1.Resturants<br>
2.Volunteer<br>
Resturants: A profile is made that allows resturant to upload the details of their remaining food and the location of the pick up point with contact details.
The resturants gets access to create, edit and update their food stock and pick up point details .<br>

Volunteer: A volunteer gets in to browse information about different pick up points with number of food packets in sorted manner according to the location.This view has two features
Chat Support/Helpdesk- This helps the volunteer to resolve any kind of queries.<br>
Contributor- This feature allows a doner to fill in personal details and donate fund for well being of people.<br>

![appscr](https://user-images.githubusercontent.com/65532996/148741171-831af6a3-3aa5-455e-a50e-aa60d517b515.jpg)
<br>

<b> FUNCTIONALITY AND CONCEPTS USED </b>

- Live Data and View Model: View Model is used to make the app flexible to changes and the reflected changes in the UI fragments are observed using LiveData.<br>
- Room Database: The user details are stored using Room Database.Also, it is used for user authentication.<br>
- Navigation Library: The bottom navigation in our app is implemented using the navigation library in order to ease out navigation between the Join, Donate and Chat options as separate fragments in our app.<br>
- Retrofit for the internet: The network requests to the API are done using the Retrofit library. When a user logs in or registers, the API returns a token that gets stored in the room database.On every subsequent request made, the token is passed as an authorization header using Retrofit in order to get other authentication datas like user profile details.<br>
- Recycler view: Recycler view is used to make the app lightweight. It is used to list down the NGOs in our app. Also,the horizontally scrollable gallery in the profile section of our app is created using the Recycler view.<br>
- setImageResource():This function is used in the  recyclerView adapters to bind the images.It was implemented while working with images.<br>
- GSON lib: .In our app it is used with retrofit to convert JSON into Kotlin objects for smooth transmission for data between server and our application.<br>
All the pages were implemented using Fragments and to prevent implementation of functions on the main thread, Coroutines were used.<br>

<b> APPLICATION AND FUTURE SCOPE </b>


The app is yet to be modified to be used in a broader spectrum.<br>
The organiser mode is yet to be worked on and is presently on the server side.<br>
You can access the link here:
<a href="https://drive.google.com/drive/folders/1im1f7it62AK0PkW96h-AUdx0nDBDJwYg?usp=sharing">Download apk</a>
<br>
We wish to further work on improvising our app, add some advanced features enabling chat and video features to work thus making it more flexible.Further,we plan to collaborate with a few local NGOs so that it can be widely used serving the purpose.<br>
We aim to associate our app with the National Service Scheme(NSS) group at our University who will be responsible for testing and providing us with improved scalability thus making our app ready for a robust launch to be service-ready.<br>
This app is definitely going to help the NGOs connect with contributors heading towards a more charitable society.

