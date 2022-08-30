meet_app


Description.
This app provides a list of upcoming events for any given city, with data provided by Google Calendar. The app works offline using cached data from the last time it was used online. The user can search for events in a specific city or browse all events, customize how many events are shown on screen, click an event for more details, and see how many events are upcoming in certain cities.


How to Use This App.
When first opening the app, you will be prompted to sign in with Google in order to gain access to the Google Calendar API. Then, you can specify what city and how many events to view, and click on an event to view more details!


Dependencies
HTML5 CSS3 JavaScript (ES6) React API This app used the Google Calendar API to fetch information about upcoming events by location.


A Note On Privacy.
The Meetup app requires you to sign in with Google in order to access the data from its Google Calendar. This access goes both ways, as Meetup can also access the user's calendar, HOWEVER it DOES NOT and will never be given this functionality. Rest assured, the app does not attempt to do anything with the Google user's information in any way. The app is also currently in the process of being verified, but this may take some time; Google has a lot on their plate.





Filter Events by City

-Scenario 1: When the user hasn’t searched for a city, show upcoming events from all
cities.
Given user has not searched for a city from the search bar.
When the user opens the app.
Then the user should see a list of all the upcoming events.

-Scenario 2: The user should see a list of suggestions when they search for a city.
Given: the main page is open
When: the user starts typing in the city name of a city in the search bar.
Then: the user should see a list of suggestions (events) that match the city that they’ve typed.

-Scenario 3: The user can select a city from the suggested list.
Given: the user was typing “London” in the city search bar and the list of suggested events is
showing
When: the user selects a city (e.g. “London, England”)
Then: their city should be changed to that city (i.e., “London, England”) and the user should
receive a list of upcoming events in that city

-User story
As a user,
I should be able to view the events or hide them.
So that I can easily scan through the options that are available in the city



Show/Hide Details of an Event

-Scenario 1: An event element is collapsed by default.
Given: the main page has been opened.
When: nothing is selected.
Then: the current events from that city will be collapsed/hidden from the user

-Scenario 2: The user can expand an event to see its details.
Given: the user clicked on an event.
When: the user selects a specific event.
Then: the details of that event will be listed for the user to view.

-Scenario 3: The user can collapse an event to hide its details.
Given: the event element is opened.
When: the user closes the event element.
Then: the details will be hidden.

-User Story
As a user, I should be able to display and collapse event details so I can see more or less information depending on my preference.




Specify Number of Events

-Scenario 1: When the user hasn’t specified a number, 32 is the default number.
Given: the user searched for event results for a city.
When: the user chooses no specific amount of search results.
Then: the default amount of search results per city will be 32.

-Scenario 2: The user can change the number of events they want to see.
Given: the user opened the search results query
When: the user changes the default number
Then: the default number of results will be changed to what the user selects.

-User Story
As a user, I should be able to choose the number of events that are listed.





Use the App when Offline

-Scenario 1: Show cached data when there’s no internet connection.
Given: the app has no internet connection
When: the data is cached
Then: that data will still be displayed.

-Scenario 2: Show error when user changes the settings (city, time range).
Given: the user opened the settings tab
When: the user changes the settings
Then: an error will show

-User Story
As a user, I should be able to access the events even when offline.






Data Visualisation

-Scenario 1: Show a chart with the number of upcoming events in each city.
Given: the user selected a city 
When: the user clicks on the city’s upcoming events button
Then: a chart will list the upcoming events taking place in the city.

-User Story
As a user, I should be able to see a chart or list of events taking place.
So that I can easily sort through my options.



