this is project without the src directory 

all the pages will be built inside the app follder 

neon (data base ) and prims (orm)


lets make some of the changes for the github

## folder and file structure 

1. as we have choosen the app router but havent choosen the src so inside the `app folder`  each folder is a route 
2. the main page(home page) `page.tsx` is not in the any folder of  `appFolder` so that direct `/` route can easily trigger it 
3. `layout.tsx` is simialar to the app file in the mern folder structure. it is the start point all other pages are its child. the restriction which we want to apply on all the pages we can apply form here
4. Action folder inside the app folder contain the crud operation code 


## Component 
- for the component create a folder in the root directory, 
- and inside this we crete the files of diferent components

### Q what about those components that are the part of all pages like navbar ??
import and use navabar tag, just before the child tag inside the `layout.tsx`

## LIb folde 

the lib folder is similar to the servies folder here we got the db `connection` and `chechkUser` etc 

## Action folder 
all the crud operaton api are built under this folder like: get details etc etc in normal mern project we perfom this task using the routes or by the sockets but here we do this task using the the `Action folder in the App folder`

### Favcon.con file in the app folder
favicon.ico is taken by the browser to display it beside the website name in the browser tab, and it is picked automatically. this thing is for improving the sco score 
