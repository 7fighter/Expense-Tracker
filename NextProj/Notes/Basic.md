this is project without the src directory 

all the pages will be built inside the app follder 

neon (data base ) and prims (orm)


lets make some of the changes for the github

## folder and file structure 

1. as we have choosen the app router but havent choosen the src so inside the `app folder`  each folder is a route 
2. the main page(home page) `page.tsx` is not in the any folder of  `appFolder` so that direct `/` route can easily trigger it 
3. `layout.tsx` is simialar to the app file in the mern folder structure. it is the start point all other pages are its child. the restriction which we want to apply on all the pages we can apply form here


## Component 
- for the component create a folder in the root directory, 
- and inside this we crete the files of diferent components

### Q what about those components that are the part of all pages like navbar ??
import and use navabar tag, just before the child tag inside the `layout.tsx`

## LIb folde 

the lib folder is similar to the servies folder 