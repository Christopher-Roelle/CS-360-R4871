# CS-360-R4871
App Code Design - Inventorio

+ **Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?**

The requirements of the app were:
An inventory app that had a user sign in (or register an account), which they would be able to see inventory stock of a warehouse, store, etc.
The app would need to allow for CRUD of Inventory data, which means adding products, updating products, removing them, and reading their data.
The app would also need a notification system (handled via SMS) which would notify a user (or users) of low stock in regular intervals.

The app was designed to be used by Warehouses and stores, but could be adopted into Schools, and small businesses that need to keep track of products.

+ **What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?**
  
The app relied on a login screen and an inventory screen.
The login screen handled user registration and authentication.
The inventory screen handled displaying to the user, the products within a table with controls for incrementing/decrementing stock.
The screen also provided modals for notifications and adding new products.
Selecting an individual product within the table provided a modal that allows for Updating products.

I tried to keep the design simple and user friendly, which allowed for the design to be successful.

+ **How did you approach the process of coding your app? What techniques or strategies did you use? How could those be applied in the future?**

I designed the app first with a wireframe, which I then converted to a GUI.
Once the base GUI was designed, I wrote code to wire it together, and began adding the modals to handle communcations with the Database/Services.

I employed the MVC model when I wrote the app. This allowed for easy scaling and modification of my code, as the Business Logic and the logic that Controlled the app's GUI were not intermingled.
I would employ the MVC model to any further GUI-based apps going further as it greatly reduces code re-writes and makes scaling far easier.

+ **How did you test to ensure your code was functional? Why is this process important and what did it reveal?**

I would manually test to ensure that the code was functional. I also had other users test the code, since they were likely to use the app in a different method.
This allowed me to find a bug with adding products where the product could incorrectly add.

Testing is important to catch bugs in the code that could lead to undefined or incorrect behaviors. This ensures for good software, and reduces risk to the hardware and data it may contain.

+ **Considering the full app design and development process, from initial planning to finalization, where did you have to innovate to overcome a challenge?**

I feel that I had to get innovative with my modal designs. I wanted the modals to stay open when an error occured, to both display a message and retain the user-entered data.
Unfortunately the Positive/Negative buttons force close a modal when clicked. I ended up needing to manually code the logic for a pre-defined button in the modal xml to handle data validation
and keep the modal open if it was invalid or unable to be entered into the DB.

+ **In what specific component from your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?**

Anywhere that SQL was employed (login logic, product management and retrieval logic). I use SQL on a daily basis for work, and was able to write the SQL logic pretty easily and accurately.
Backend logic of the app (Java) was also very easy for me, since I write in Java on occasion.

The GUI (xml) was probably the only place I struggled a bit, because I am not a designer by trade, and have limitted experience with front-end development.
