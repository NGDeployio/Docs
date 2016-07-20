# Docs
Documentation library for ngDeploy. 
[Bower](https://github.com/NGDeployio/Docs#bower)  
[Grunt/Gulp](https://github.com/NGDeployio/Docs#grunt)  
[HTTPs](https://github.com/NGDeployio/Docs#HTTPs)  
[Custom Domains](https://github.com/NGDeployio/Docs#custom-domains)  

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

## Hosting
The resulting directory is then hosted. The initial site is available in the **development** stage. From here we can promote it to **staging** and onto **production**. 

## Multistage environments
We offer a multistage environment for a controlled development workflow. The application is not rebuild between steps.   

#### Development
#### Staging
#### Production

## Premium features

### HTTPs
Once the application is promoted, we can setup the HTTPs by visiting the Setup page. 

### Custom domains
To route a custom domain to ngDeploy add the domain using the Setup page. Then point a CNAME to the upgraded address.
