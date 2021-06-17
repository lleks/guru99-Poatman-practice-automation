Get Users
`https://jsonplaceholder.typicode.com/users`

Create (Post) User
`https://jsonplaceholder.typicode.com/users`
Body:
`[
    {
        "id": 11,
        "name": "Krishna Rungta",
        "username": "Bret",
        "email": "Sincere@april.biz",
        "address": {
            "street": "Kulas Light",
            "suite": "Apt. 556",
            "city": "Gwenborough",
            "zipcode": "92998-3874",
            "geo": {
                "lat": "-37.3159",
                "lng": "81.1496"
            }
        },
        "phone": "1-770-736-8031 x56442",
        "website": "hildegard.org",
        "company": {
            "name": "Romaguera-Crona",
            "catchPhrase": "Multi-layered client-server neural-net",
            "bs": "harness real-time e-markets"
        }
    }
]`

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

newman run <collection name> --data <file name>  -n <no.of `iterations> -e <environment name>`


















