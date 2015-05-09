#Java timeago library

This is a Java port of the [jquery-timeago](https://github.com/rmm5t/jquery-timeago) plug-in.  Please visit the [jquery-timeago](http://rmm5t.github.com/jquery-timeago/) project page to read more about fuzzy timestamps.

##Building
The timeago project contains a Maven pom.xml file that builds a jar containing the TimeAgo class.
To build and run the included unit tests:
$ mvn clean install

##Usage

```java
TimeAgo time = new TimeAgo();
long current = System.currentTimeMillis();
String minutes = time.timeAgo(current - (15 * 60 * 1000));  // returns "15 minutes ago"
String hours = time.timeUntil(current - (6 * 60 * 60 * 1000));  // returns "6 hours from now"
```


##Contribution

If you would like to contribute locale-specific properties files please fork this repository and open a pull request.

##Other

[MIT License](http://www.opensource.org/licenses/mit-license.html)
