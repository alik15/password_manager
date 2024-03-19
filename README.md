# password_manager
This is a weird password manager that my friend and I came up with and I am now trying to implement in perl(to be decided)
Here is the initial idea:
You have a password you use everywhere. That is a massive problem, despite IT staff trying to remedy this problem in offices with regular emails, it still causes thousands/millions of money in damages.
This is a way to fix that. You get to use the same password everywhere with a caviate. It will be used as a seed to generate a password using encryption at runtime.
The public key will be different for each website. 



A single .txt file will be kept in a public storage solution like github, docker, google drive, 
# Usage example


passmanager --website github.com --username alik15 --private_key<br/>
_this is an unsafe way to do it so only do it when not using it in public as anyone can see your private key_



list: lists all websites and its associated emails so that you can generate the password for each be selecting 
you can register new websites and emails with the register function 



# Things to add / notes

* the websites and the usernames and stored in a txt file and at runtime are loaded into memory? or can we also check the file 
* the cli app will probably be written in c or in bash and it will call functions from the main app/bin
* cli app
* the cli app can run and can also take arguments
* the cli app when running will not show the password or the length of your password when you are typing it ( as is done in linux sudo)
* a docker container can be downloaded which can be run and it can serve on a port on a website that does this 
  the encryption happens on the client side

* second private key
* different encryption for different websites or even usernames
* import: this allows you to import passwords from places like:
    - google password manager
    - firefox password manager
    - bitwarden


# Some Caveats
This solution outputs the same password for the same website and username, if someone finds out your password you will have to change your encryption code. (This can also be added to settings)
