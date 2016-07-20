# Docs
Documentation library for ngDeploy. 

## Build process for ngDeploy
- Bower/Gulp install
- Grunt build
- Hosting

## Bower
During the deployment process we execute a basic **bower install**. The process will currently fail if there are conflicts within the Bower file. 

## Grunt
After **Bower install** is executed we do a **Grunt build**. Here all of the files should be compiled into a central distribution directory. This is typically a **dist**  or **app** from which the files will be hosted. By default we host files from **./** unless otherwise specified. 

## Multistage environments
### Development
### Staging
### Production
