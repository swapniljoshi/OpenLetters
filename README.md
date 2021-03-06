![open letters](https://raw.githubusercontent.com/nshntarora/OpenLetters/master/app/assets/images/logo.png)


```
Give a man a mask and he will tell you the truth.
                                     - Oscar Wilde
```


Every company, no matter the size, is making itself more transparent to all of its employees. Heck, some have even made their processes and revenues public.

The sole reason behind all of this being, transparency breeds trust.

To know more about this little app and why I even thought of it in the first place, check out [this Medium post].

There are two steps to using it.

###Step 1
All you need to do is, on your company’s LAN server, install rails, clone the repo, run bundle install, and change the password and username.

The app uses HTTP authentication so that if somehow someone gets onto your LAN he will have to enter a username and password which, only the employees of your company (are supposed to) know.

To change the password and username for your company, go the Letters controller (located in app/controllers).
```
http_basic_authenticate_with name: "acmecorp", password: "thisisakey"
```
Look for the above line, change ```acmecorp``` to your company’s name and ```thisisakey``` to the password you would like to set.
To remove the HTTP authentication just remove the whole line from the controller.

###Step 2
Add features to your copy, extend the functionalities, make it more secure, preferably in your free time. Then, create a pull request here :p

###Screenshots

![screenshot1](https://raw.githubusercontent.com/nshntarora/OpenLetters/master/app/assets/images/index.png)

![screenshot2](https://raw.githubusercontent.com/nshntarora/OpenLetters/master/app/assets/images/show.png)

![screenshot3](https://raw.githubusercontent.com/nshntarora/OpenLetters/master/app/assets/images/new.png)


###Cheers to a transparent workplace.

![cheers!](https://www.emojibase.com/resources/img/emojis/twitter/1f37a.png)

   [this Medium post]: <https://medium.com/@nshntarora/get-aside-slack-here-comes-another-future-of-workplace-communication-649c5cc19b0c>
