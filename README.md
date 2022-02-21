# Fake-User-Prediction-Python

A marketplace is being attacked by bots that produce fake clicks and leads. The
marketplace reputation might be affected if sellers get tons of fake leads and receive
spam from bots. On top of that, these bots introduce noise to our models in
production that rely on user behavioural data. We need to save Adevinta's reputation
detecting these fake users.
To do so, we have a dataset of logs of a span of five minutes. Each entry contains
the user id (UserId), the action that a user made (Event), the category it interacted
with (Category) and a column (Fake) indicating if that user is fake (1 is fake, 0 is a
real user). An example of how the data looks like:
UserId Event Category Fake
XE321R click_ad Motor 1
ZE458P send_email Motor 0
XE321R click_ad Motor 1
