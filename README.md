![Photo by Monika Grabkowska on Unsplash](https://user-images.githubusercontent.com/2342458/202707543-0d872d00-f686-4d84-860f-f0b9e3814d5e.png)

# Kinsta - Hello World - Static Site With Gatsby
An example of how to deploy a static site built with Gatsby on Kinsta App Hosting services.

---
Kinsta is a developer-centric cloud host / PaaS. We’re striving to make it easier for you to share your web projects with your users. Focus on coding and building, and we’ll take care of deployment and provide fast, scalable hosting. + 24/7 expert-only support.

- [Start your free trial](https://kinsta.com/signup/?product_type=app-db)
- [Application Hosting](https://kinsta.com/application-hosting)
- [Database Hosting](https://kinsta.com/database-hosting)

## Dependency Management
During the deployment process Kinsta will automatically install dependencies defined in your `package.json` file.

## Web Server Setup

### Port
Kinsta automatically sets the `PORT` environment variable. You should **not** define it yourself and you should **not** hard-code it into the application. The `serve` packageutilizes the port set by Kinsta automatically. 

### Start Command
When deploying an application Kinsta will automatically create a web process with `npm start` as the entry point. Make sure to use this command to run your server. 

## Deployment Lifecycle
Whenever a deployment is initiated (through creating an application or re-deploying due to an incoming commit) the `npm build` command is run, followed by the `npm start` command.  

sptestcommit
