# Docs
Documentation library for ngDeploy. 

## Build process for ngDeploy
- Bower/Gulp install
- Grunt build
- Hosting

## Github Integration
Upon login we offer the ability to hook repositories to ngDeploy. Once hooked Github notifies us when the **Master** repository is updated and we kick off the build process.

## Bower
During the deployment process we execute a basic **bower install**. The process will currently fail if there are conflicts within the Bower file. 

## Grunt
After **Bower install** is executed we do a **Grunt build**. Here all of the files should be compiled into a central distribution directory. This is typically a **dist**  or **app** from which the files will be hosted. By default we host files from **./** unless otherwise specified. 

## Multistage environments
We offer a multistage environment for a controlled development workflow.
### Development
### Staging
### Production

