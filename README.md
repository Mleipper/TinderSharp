# TinderSharp
A .Net Standard 2.0 wrapper for the Tinder API

## License

You can use this library for free in any kind of project and distribute it however you want. The only thing you need to link or refer to this github project in any way possible.

## Contributions

* To develop this wrapper, initially I got the endpoints from https://github.com/fbessez/Tinder and https://gist.github.com/rtt/10403467

## Features

As of 28th of June 2020, most of the free functionalities of Tinder are working with this wrapper, with the notable exception of Authentication. 

### Authentication

As of now, If you want to use the API you have to [login](https://www.tinder.com) on your browser and look at any of the incoming network request. In any request coming from `api.gotinder.com` you have to look for the `X-Auth-Token`  header, that value will be the token you need to use in order to authenticate all your API calls.

From my initial testing, I can say that this token lasts a long time (more than 10 hours). I will try to enable Google OAuth, SMS Login or Facebook Authentication in the next days.

### Account

This wrapper allows you to reset or change your username, get updates on new messages or new matches and retrieve the information of your profile. For now you can only get the likes that you have left, account data and user data. 

I have not implemented other modules yet such as:

- Boost
- contact_cards
- plus_control
- travel
- tinderUniversity
- super_likes
- products
- instagram
- purchases
- EmailSettings
- read_recipts
- swipe_note
- tutorials

The reason behind this is that most of those modules are oriented to their app, I don't understand yet what they do or they are not free and I can't test them.

### Matches

Matches are fully working, you can get a list of match recomendations and like, pass or superlike the recomendation. You can also unmatch them.

### Messages

Messages are fully implemented and you can send written messages, gifs (from giphy) and songs from spotify. You can also retrieve a list of the messages from each match.





