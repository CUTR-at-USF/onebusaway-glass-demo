OneBusAway Glass demo
========================

This project is a demo to display OneBusAway real-time information on Google Glass.

See the issue on the main OneBusAway server project for details:
https://github.com/OneBusAway/onebusaway-application-modules/issues/60

## Setup

You must create an `oauth.properties` file in the `src/main/resources` directory, with the following format:

~~~
# Replace these with values for your project from the Google API Console:
# https://developers.google.com/console

client_id=1234567890.apps.googleusercontent.com
client_secret=SDIOJ#39v@Bv9@WHF
~~~

## Execution

You can start this project running in Jetty on `localhost` using the command:
`mvn clean jetty:run`

## Packaging

You can package this project as a WAR file for deployment to a web servlet container (e.g., Tomcat) using the commands:
`mvn clean compile`
`mvn war:war`

This will produce a WAR file in the `/target` directory.

## Troubleshooting

If you get oauth errors when deploying to Tomcat, try shutting down and restarting Tomcat.  Sometimes on initial deployment Tomcat doesn't seem to load the oauth libraries correctly.

## License
Code for this project is licensed under [APL 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)
and content is licensed under the
[Creative Commons Attribution 3.0 License](http://creativecommons.org/licenses/by/3.0/).
