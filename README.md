This project demonstrates that without the javax.mail dependency, an application cannot use `HTTPResponse`.

To see the behavior, do:

```bash
mvn exec:java -Dexec.mainClass="WithoutJavaMail"
```

And you should see the message:

```bash
An exception occured while executing the Java class. javax/mail/internet/ParseException
```

as part of the build failure.
