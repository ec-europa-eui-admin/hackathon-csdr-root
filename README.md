# CSDR DEVELOPERS GUIDE 

follow the documentation on Confluence : 

https://webgate.ec.europa.eu/fpfis/wikis/display/eUI/Developer%27s+guide

### for eUI support : 
DIGIT-EUI-SUPPORT@EC.EUROPA.EU or slack : https://ec-eui.slack.com

### for MyWorkplace / CC support : 
EC-MYWORKPLACE-SUPPORT@EC.EUROPA.EU or slack : https://compass-corporate.slack.com


## Quick start
0.  Register the functional user on ecdevops.eu
1.  clone the root repository - MASTER branch for eUI 7 / CSDR 7
2.  yarn
3.  initialize options : 
    ##### interactive
    ````npm run init => select your project / team```` 
    ##### command line if project / team id are known
    ````npm run init -- --project <PROJECT> --team <TEAM>````
    ##### to mount a package on top of an existing initialized CSDR
    ````npm run init -- --pkg <PACKAGE> --pkgOnly````
4.  start mwp: 
    ````npm run mywp:start-local-openid````


## Re-sync local dependencies

ALWAYS execute this before starting any apps : 

````npm run upgrade:deps````


## Package operations

### Build package locally

##### default :
````npm run pkg:build <PACKAGE>````
##### skipping linting / test :
````npm run pkg:build <PACKAGE> -- --skipLint --skipTest````
##### package deps built first (as defined in .euirc-csdr-packages.json files "deps" array of package)
````npm run pkg:build <PACKAGE> -- --deps````

