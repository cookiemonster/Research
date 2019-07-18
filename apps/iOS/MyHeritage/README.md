# MyHeritage app

version: 5.1.0
App store link: https://apps.apple.com/nl/app/myheritage/id477971748?l=en


## Overview
The popular app for building your family tree, testing your DNA, and exploring your ancestry. 
MyHeritage is almost similair to AncestryDNA. It has DNA comparison with relatives feature and 
the ability to upload DNA from other providers. It has a 93 million userbase.

## Networking
The traffic between the app and the servers all using SSL/HTTPS.

#### Privacy

The app uses these tracking service:

#### [Localytics](https://localytics.com)
Specialized in "Attribution Evaluation, Profiles Integration, Data Mining & Analysis and Remarketing."
They track the [user activity](https://raw.githubusercontent.com/cookiemonster/research/master/apps/iOS/MyHeritage/https%3A/analytics.localytics.com.json) in the app.

#### Security

The application does not check if the certificate in question is a specific certificate from MyHermitage.
Because of the lack of certificate pinning creates a security hole. The device’s trust store can easily be compromised by using certificates, and allowing a man-in-the-middle attack on the device itself. This can be easiliy remediated with 
certificate pinning by including the certificate known to be used by the server in the app. Most decent banking apps and 
the AAA-Style games phones and tablets have these.
