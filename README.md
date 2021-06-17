Get Users

`https://jsonplaceholder.typicode.com/users`

Create (Post) User

`https://jsonplaceholder.typicode.com/users`

Parameterize Requests:

1. Set your HTTP request to GET

2. Use: `https://jsonplaceholder.typicode.com/users`

3. Replace the first part of the link with a parameter such as `{{url}}`. Request url should now be `{{url}}/users`

Set the environment:

`https://jsonplaceholder.typicode.com` as `url`

How to Run Collections using Newman:

1. Install nodejs

2. In cmd run: `npm install -g newman`

Run a collection only (this can be used if there is no environment or test data file dependency):

`newman run <collection name>`

Run a collection and environment (the -e indicator is for environment):

`newman run <collection name> -e <environment name>`

Run a collection with desired no. of iterations:

`newman run <collection name> -n <no.of iterations>`

Run with data file:

`newman run <collection name> --data <file name>  -n <no.of iterations> -e <environment name>`


















