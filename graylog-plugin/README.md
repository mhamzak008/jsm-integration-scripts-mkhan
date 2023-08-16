# Jira Service Management Integration Graylog Plugin

Jira Service Management(JSM) has a specific integration plugin for Graylog. Using this plugin, Graylog sends stream alerts to JSM, with detailed information. JSM acts as a dispatcher for Graylog alerts, determining the right people to notify based on on-call schedules, using email, text messages (SMS), phone calls and iPhone &amp; Android push notifications, and escalating alerts until the alert is acknowledged or closed.

Building the Plugin
--------------
This project is using Maven 3 and requires Java 7 or higher. The plugin will require Graylog 1.0.0 or higher.

* Clone this repository.
* Run `mvn package` to build a JAR file.
* Optional: Run `mvn jdeb:jdeb` and `mvn rpm:rpm` to create a DEB and RPM package respectively.
* Copy generated JAR file in target directory to your Graylog plugin directory.
* Restart the Graylog.
