Readings: HEROKU

![o](https://qph.fs.quoracdn.net/main-qimg-f0f8b07f2c9cd08071b0bd8a78f192f0.webp)



Heroku is a cloud platform as a service 
One of the first cloud platforms, when it supported only the Ruby programming language, but now supports Java, Node.js, Scala, Clojure, Python, PHP, and Go. For this reason, Heroku is said to be a polyglot platform as it has features for a developer to build, run and scale applications in a similar manner across most languages.
Developers use Heroku to deploy, manage, and scale modern apps. It is flexible, and easy to use, offering developers the simplest path to getting their apps to market. 



![p](https://i.morioh.com/2020/04/28/51847824ff51.jpg)




installing steps :
install the Heruko app.
Deploying the app.
View logs.
Define a Procfile, which is a text file in the root directory of your application
Scale the app.
Declare app dependencies.
Run the app locally.
Push local changes.
Adding addons

Architecture

A diagrammatic view of the working of Heroku Platform
Applications that are run on Heroku typically have a unique domain used to route HTTP requests to the correct application container[15] or dyno.[16] Each of the dynos are spread across a "dyno grid" which consists of several servers. Heroku's Git server handles application repository pushes from permitted users.[17]

All Heroku services are hosted on Amazon's EC2 cloud-computing platform.


The Heroku Platform
The Heroku network runs the customer's apps in virtual containers which execute on a reliable runtime environment. Heroku calls these containers "Dynos." These Dynos can run code written in Node, Ruby, PHP, Go, Scala, Python, Java, or Clojure. Heroku also provides custom buildpacks with which the developer can deploy apps in any other language. Heroku lets the developer scale the app instantly just by either increasing the number of dynos or by changing the type of dyno the app runs in.
Heroku Postgres
Heroku Postgres is the Cloud database (DBaaS) service for Heroku based on PostgreSQL. Heroku Postgres provides features like continuous protection, rollback, and high availability; also forks, followers, and dataclips
