# vrse-utilities
This is the central codebase for vrse. It includes all template logic and threeJS utilities which go into building the templates. The 'utilities' folder contains all js modules and is therefore the most important folder, hence the name of this repo. This repo also contains, however, all template model files and baked lighting files. It also contains all available font files. The reason for this is because all template logic is included in the templates folder in utilities - therefore we include all template dependencies here so that they can be self-contained. 

## More notes: 

- The builder app is the only place which contains the full utilities folder, upon actually building a deployed site (user site with user data) npm build will only take the modules and dependencies (.gltf files and baked lighting jpgs). 

- This repo contains no user data. 

- In the future we will axe this way of storing files in favor of AWS buckets and dynamically loading files.

- When adding to the utilities folder always (1) make sure you code is broken up into javascript modules (2) make sure all your file dependencies are in the appropriate static folder (3) make a test html file and script, which uses any template and shows how your addition works.
