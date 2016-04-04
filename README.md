# codenameSails

a [Sails](http://sailsjs.org) application

To generate a new model, use the command sails generate model <model_name>

The route is now localhost:1337/<model_name>
(will show an empty array at first)

For our development I created a model called User
Now to create a new entry use the URL  localhost:1337/User/create?name=<someName>

This will create the following entry:

{
	Name: "Krys",
	Id: 1,
	createdAt: "timestamp",
	updatedAt: "timestamp"
}

To add another attribute use the url 'Update', for example if I wanted to add an email to a user,
I would use the url localhost:1337/User/update/1?email=krys.newman@gmail.com

This adds the attribute to the entry and now looks something like:

{
	Name: "Krys",
	Id: 1,
	createdAt: "timestamp",
	updatedAt: "timestamp",
	Email: "krys.newman@gmail.com"
}
