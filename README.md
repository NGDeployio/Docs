# Docs
Documentation library for ngDeploy.   

[NPM](#npm-install)  
[Bower](#bower)  
[Grunt](#grunt)  
[Teams](#teams)
[HTTPs](#HTTPs)  
[Custom Domains](#custom-domains)  
[Caching with KeyCDN](#caching-with-keycdn)

## Github Integration
Upon login we offer the ability to hook repositories to ngDeploy. Once hooked Github notifies us when the **Master** repository is updated and we kick off the build process. 

One of the benefits of an integrated build process is the ability to update web applications directly from Github.

## Build process for ngDeploy
- NPM install
- Bower install
- Grunt build
- Hosting

## NPM
The first part of the build process installs any npm modules listed in the **package.json** using **npm install**. This is where we specify any Grunt or Gulp dependencies.

## Bower
During the deployment process we execute a basic **bower install**. The process will currently fail if there are conflicts within the Bower file. 

## Grunt
Then we do a **grunt build**. Here all of the files should be compiled into a central distribution directory. This is typically a **dist**  or **app** from which the files will be hosted. By default we host files from **./** unless otherwise specified in ![App Settings](http://res.cloudinary.com/ngdeploy/image/upload/c_fit,h_24/v1469102560/Screen_Shot_2016-07-21_at_8.02.25_AM_qkjgfu.png) **sync settings** 

## Hosting
The resulting directory is then hosted. The initial site is available in the **development** stage. From here we can promote it to **staging** and onto **production**. 

## Multistage environments
We offer a multistage environment for a controlled development workflow. The initial push to development runs through the build process and might take a couple of seconds. However all promotions from then on are nearly instant. 

> Development  
> Staging  
> Production  

## Teams
Teams on ngDeploy allow app creators to delegate promotions and environment configurations.

## Premium features
There are a number of benefits to upgraded apps. For example HTTPs, Custom domains, and Caching with KeyCDN. 

### HTTPs
Once the application is promoted, we can setup the HTTPs by visiting the Setup page. 

### Custom domains
To route a custom domain to ngDeploy add the domain using the Setup page. Then point a CNAME to the provided address.

### Caching with KeyCDN
We use KeyCDN to cache all of the websites. This way users get the fastest version of your website for their location. We also have a **cache purge** functinality to clear the cache. 
