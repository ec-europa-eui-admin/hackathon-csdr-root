# CSDR DEVELOPERS GUIDE 

## Quick start
0.  Install yarn
    ````npm install -g yarn@latest````
1.  clone this repo
2.  Install root dependency (@eui/tools) - bypass overwriting the provided yarn.lock
    ````yarn --no-lockfile````
3.  initialize the api-manager project
    ````npm run init -- --project api-manager````
4.  start local app: 
    ````npm run api-manager:start````

## Additional commands

````npm run upgrade:deps````

## Package operations

### Build package locally

##### default :
````npm run pkg:build <PACKAGE>````
##### skipping linting / test :
````npm run pkg:build <PACKAGE> -- --skipLint --skipTest````
##### package deps built first (as defined in .euirc-csdr-packages.json files "deps" array of package)
````npm run pkg:build <PACKAGE> -- --deps````

### for eUI support : 
https://ec-eui.slack.com
