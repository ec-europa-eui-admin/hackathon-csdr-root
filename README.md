# CSDR DEVELOPERS GUIDE 

### for eUI support : 
DIGIT-EUI-SUPPORT@EC.EUROPA.EU or slack : https://ec-eui.slack.com

## Quick start
1.  clone this root repo
2.  yarn --no-lockfile
3.  initialize local CSDR dev environment : 
    ##### mounting the api-manager project
    ````npm run init -- --project api-manager````
4.  start local app: 
    ````npm run am:start````

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

