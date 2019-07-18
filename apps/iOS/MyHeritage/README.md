# MyHeritage app

version: 5.1.0
App store link: https://apps.apple.com/nl/app/myheritage/id477971748?l=en


## Overview
The popular app for building your family tree, testing your DNA, and exploring your ancestry. 
MyHeritage is almost similair to AncestryDNA. It has DNA comparison with relatives feature and 
the ability to upload DNA from other providers. It has a 93 million userbase.

## Networking
The traffic between the app and the servers all using SSL/HTTPS to these domains:

![traffic](https://raw.githubusercontent.com/cookiemonster/research/master/apps/iOS/MyHeritage/MyHeritage-_domains_2019-07-18_18.00.23.png)



#### Privacy

The app uses these tracking services. Because the applicattion is a wrapped webapplication all the content of the screen can passed on to these tracking services.

#### Google Analytics
Google Analytics is a web analytics service offered by Google that tracks and reports website trafic.

#### [Localytics](https://localytics.com)
Specialized in "Attribution Evaluation, Profiles Integration, Data Mining & Analysis and Remarketing."
They track the [user activity](https://raw.githubusercontent.com/cookiemonster/research/master/apps/iOS/MyHeritage/https%3A/analytics.localytics.com.json) in the app.

### [Taboola](https://taboola.com)
Taboola is a private advertising company headquartered in New York City. They track 


#### Security

The application does not check if the certificate in question is a specific certificate from MyHermitage.
Because of the lack of certificate pinning creates a security hole. The device’s trust store can easily be compromised by using certificates, and allowing a man-in-the-middle attack on the device itself. This can be easiliy remediated with 
certificate pinning by including the certificate known to be used by the server in the app. Most decent banking apps and 
the AAA-Style games phones and tablets have these.
