# Slovolk (Private)
### A Russian Grammar Analysis Tool written with .NET MVC5, SQL Server and Sci-kit Learn

Slovolk uses a two-pronged approach to analysing Russian vocabulary:

First, it attempts to locate the word in <b>database</b> containing over 500,000 Russian words and their translations. This database has been denormalized for performance. 

If the word is not present in the database, Slovolk Core will make an api call to a Flask <b>microservice</b> that exposes several endpoints, feeding the word through pre-trained machine learning models (e.g. gender, grammar-type) and returning the best approximation for that word. 


![slovlkgif](https://user-images.githubusercontent.com/17185335/44863528-4135dc00-ac75-11e8-9e56-07d46cebbc2a.gif)
