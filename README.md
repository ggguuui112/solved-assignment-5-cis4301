Download Link: https://assignmentchef.com/product/solved-assignment-5-cis4301
<br>
For this assignment, you will be asked to create an interface to query and edit data for a SQLite database. You will use the database maintained by the imaginary Southern Sierra Wildflower Club (SSWC), an organization whose members are interested in observing wildflowers in their native habitat in the southern part of the Sierra Nevada mountains of California. This is the same database as assignment 4.

The database maintained by the club has three tables:

SIGHTINGS (NAME, PERSON, LOCATION, SIGHTED)

FEATURES (LOCATION, CLASS, LATITUDE, LONGITUDE, MAP, ELEV)

FLOWERS (GENUS, SPECIES, COMNAME)

The database tables have the following semantics:

<ul>

 <li>SIGHTINGS gives information that describes every time that a member of the club observes one of the wildflowers described in the table FLOWERS. NAME tells the name of the flower observed, PERSON describes who saw the flower, LOCATION tells the name of a nearby geographical feature where the flower was seen, and SIGHTED tells the day when the flower was seen.</li>

 <li>FEATURES lists the various locations where flowers have been observed. LOCATION is the name of the place, CLASS is the type of place. There are several types such as Summit, Mine, Locale, etc. LATITUDE and LONGITUDE describe where on the surface of the earth the locations are found. MAP tells the name of the topographic map where the feature can be found and ELEV tells the height of the feature.</li>

 <li>FLOWERS lists all of the flowers that the members of the SSWC try to find. GENUS and SPECIES give the scientific name for the flower, and COMNAME gives the non-scientific name (NAME is a foreign key into FLOWER.COMNAME).</li>

</ul>

The database with the schema and initial data is attached to this assignment.

<h1>The Task (100 pts)</h1>

Create an interface that provides the following functionality:

<ul>

 <li><strong>Query </strong>– Allow the user to select from a list of flowers. Using the selected flower, display the 10 most recent sightings of the selected flower. Information should include the date, location, and who sighted the flower.</li>

 <li><strong>Update </strong>– Allow a user to select and update flower information.</li>

 <li><strong>Insert </strong>– Allow a user to insert a new sighting of a flower.</li>

</ul>

<strong>Note 1 </strong>You are not limited to any technology. You can use Python, PHP, etc as long as you meet the requirements outlined above.

<strong>Note 2 </strong>You must write the queries in SQL as opposed to using any ORM (object relational model) as supported by various web frameworks. You also need to use SQLite3 as the database.

<strong>What to turn in </strong>Submit all code and screenshots for each of the three requirements to canvas by the deadline. Alternatively, you can create a short video (3 minutes at most) demonstrating the application.

<strong>Group work </strong>You can work in groups of 2 for this assignment. Form groups using Canvas.

<h1>Extra Credit (100 pts)</h1>

<h2>1) Well Designed Web Interface (50 pts)</h2>

<ul>

 <li>10 pts – Aesthetically pleasing</li>

 <li>10 pts – User login</li>

 <li>10 pts – Allows creation, update, and delete through a graphical interface</li>

 <li>15 pts -Pictures of flowers are displayed with queries that return flower names</li>

 <li>5 pts – Sanitize any user generated query to prevent SQL injection</li>

</ul>

<h2>2) Back End (50 pts)</h2>

<ul>

 <li>5 pts – Create an index for each attribute in table SIGHTINGS</li>

 <li>15 pts – Create a trigger to log insertions, updates, and deletions from all tables</li>

 <li>5 pts – Have at least one user initiated input done as a transaction</li>

 <li>25 pts – Find a way to analyze your database’s performance; measure performance with and without triggers and indexes</li>

</ul>

<strong>If you attempt an extra credit item it must be documented in your video or write-up in order to receive credit.</strong>