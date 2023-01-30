# Fisher Reese 
I am from Memphis, MO and went to Adair County RII high school in Brashear, MO. <br>
Some interesting facts about me would be I played basketball, baseball, track, academic bowl, and <br>
participated in clubs such as FFA, FBLA, NHS. Outside of high school some of my hobbies are working <br>
on cars, hunting, fishing, and driving a racecar on the weekends. 
![PicOfMe](images/PicOfMe.PNG)<br>
**[PicOfMeLink](images/PicOfMe.PNG)**

***

### Countries To Visit
I have been to quite a few different countries over the years, some I had alot of fun in whereas others were <br>
scary at times and dangerous. When traveling it is a great idea to checkout the neighborhood/area you are going<br> to and not just the resort you are staying at. The resort could look very nice and pretty but when you adventure<br>
outside your resort it could be very dangerous and unwelcoming. 
| Mexico | Italy | Spain | Greece |
|:------------:|:------------:|:------------:|:------------:|
| Cheap and Fun | Good Food | Good Hiking Trails | Rich Heritage |
| 7 days | 4 days | 5 days | 4 days|

***

### Funny Quotes 
>"If you aint first your last" ~ **Ricky Bobby** <br>
>"Life's a garden, dig it" ~ **Joe Dirt**

***

### Code Snippet
>I'm kinda new in PHP, but I was told to create a login form that connects to Mysql database.
I tried the following code to connect to the database, tried it with, and without the database. I tried mysql_connect and something else, but always got the same error: (hidden:servername and others are the proper information of the server, just it is not pulbic.)<br>

Go to Article <https://stackoverflow.com/questions/55143102/how-to-connect-to-mysql-database-in-php> 

~~~php
<?php

$hostname = 'localhost';
$user = 'username';
$pass = 'password';
$database = 'database_name';

$db_connection = new PDO( "mysql:host=" . $hostname . ";dbname=" . $database, $user, $pass );

$results = $db_connection->query( 'SELECT testimonial, author FROM recommendations WHERE 1 ORDER by rand() LIMIT 1' );

foreach ( $results as $row ) {
	echo '<p id="quote">' . $row['testimonial'] . '</p>';
	echo '<p id="author">&ndash;' . $row['author'] . '</p>';
}

// Close the connection
$db_connection = null;
~~~
Link to css-tricks <https://css-tricks.com/snippets/php/basic-database-connection-random-query-display-result>

