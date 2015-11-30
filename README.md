# CAS OAuth

### Installation and Initial Testing

1. Install JDK 7 from [Oracle](http://www.oracle.com/technetwork/java/javase/downloads/index.html). Follow the instructions at that site to download and install Java SE Development Kit 7u45.

1. Open 2 terminals to run the CAS server and the sample application

	* For CAS OAuth:

		```shell
		cd cas-oauth
		./gradlew :cas:run
		```

	* For sample resource:

		```shell
		cd cas-oauth-resource
		./gradlew :resource:run
		```

1. Test initial configuration of App by going to (resource)[http://localhost:8080]. Click the CAS OAuth link to get key. Log in with username `jj` and password `jj`. Click allow. You should be redirected back to the application with a page showing the mock user's profile attributes.

### Stopping and starting

#### CAS Server

This should be run in its own terminal

Start:
```sh
cd $APP_HOME
./gradlew -q :cas:run
```

Stop:
`ctrl-c` in the terminal

#### Resource

This should be run in its own termial

Start:
```sh
cd $APP_HOME
./gradlew -q :resource:run
```

Stop:
`ctrl-c` in the terminal
