# Thanks to the original creator of the imp-template2 project
https://glitch.com/edit/#!/imp-template2
# What I, [MG]Octo#9071 have changed
- FPS Improvements
- Moved Token Imput
- Added a functional server selector
- Fixed outdated connection stuff for things like Heroku
- Few Little Things
- More like original arras.io changelog
# How to add your server(s)
- Go to line 3339 in bundle.js
- You'll see there are multiple things that look like this:
```
          {
            visible: 0,
            id: "1",
            type: "game",
            code: "glitch-worldwide-f",
            at: p.glitch('your-server'),
            prefer: !0,
           // featured: 1, // For Featured Status.
          },
```
- Now, lets break it down. The first thing you'll see is `visable 0,`. Don't worry, it is.
- The next thing is id. This is what will appear in the web address. I like to have them start at 1 and numarically have them go up
- The thing after that is "type". This is used for indentifying the gamemode but it doesnt really matter what you put in cuase it wont effect the game, only the server does that
- Under that, is `code: "glitch-worldwide-f",`. This effects how it'll show in the server selector. Lets break this down too.
- First of all, it sais "glitch". This is the server provider your using. Say if your using Heroku instead, you would put Heroku
- After that it sais "worldwide". This is the region. Just keep it at worldwide unless your really gonna set up servers in different locations
- at the end, it sais "f". This is the gamemode that displays in the server selector. Here is a list of gamemodes you can choose from
- (note; This is just what it displays, if you want it to actally be say domination, you gotta do that in your server code.)
```
p=private
e=word
w=words
o=open
m=maze
f=ffa
2=2TDM
3=3TDM
4=TDM
d=domination
m=mothership
a=assault
```
- Next we got ``at: p.glitch('your-server'),``. This is where you'll put in to connect to your server.
- The p.glitch is what server hoster its gonna attempt to connect to. If we want heroku, we would put in p.heroku instead of p.glitch.
- Afterwards, theres ``prefer: !0,``. I wouldnt mess with it but it makes you automaiticly connect to that server by default
- Horray! You are now done doing the informational reading. Lets put this knowledge into use.
- What were gonna try to do;
- Have a server that connects to my glitch server that is 2TDM.
- The first thing were gonna do is find the server selector code in bundle.js on line 3339.
- Next, where gonna look at the code and figure out what to do.
```
          {
            visible: 0,
            id: "1",
            type: "game",
            code: "glitch-worldwide-f",
            at: p.glitch('your-server'),
            prefer: !0,
           // featured: 1, // For Featured Status.
          },
```
- Now that you are there, lets edit some things. 
- We want to connect to our glitch project, "swift-checkered-wildebeest".
- What where gonna do is replace the "your-server" with "swift-checkered-wildebeest".
- After that, were gonna change ``code: "glitch-worldwide-f",`` to ``code: "glitch-worldwide-2"``. 
- What i did is this: Keep it as glitch cause thats what where using; Keep at as worldwide cause why not; replace the "f" with "2" becuase we want 2TDM. Remember, a list of all the gamemodes is listed above.
- And there we go, we should know have a working, custom client with a server selector! Horray!
### If you need any help, DM me on discord:
- [MG]Octo#9071

# CHANGELOG
-fixed heroku and repl.it unable to connect