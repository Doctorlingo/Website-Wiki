## Development

We recommend [starting with the API project first](https://code.doctorlingo.com/doctorlingo/api.doctorlingo.com/-/wikis/Development), since the website will show a spinner until it can connect to the API.

1. First thing to do is make sure your `code.doctorlingo.com` account has your SSH key for access through git. Here's some documentation on how to create an SSH key, and add it to your account:
    - https://code.doctorlingo.com/help/ssh/README#generating-a-new-ssh-key-pair
2. Make sure you have the necessary programs
    - NodeJS: https://nodejs.org/en/download/ v12 or higher
3. Clone the repository to a known location, and go into the folder
    - `cd /users/mark/code/doctorlingo`
    - `git clone git@code.doctorlingo.com:doctorlingo/doctorlingo.com.git`
    - `cd website`
4. Install the project
    - `npm install`
5. Start the project
    - `npm start`

That's it! The website is much simpler because we don't have to set up the database, and we have a local environment file with our environment variables that should be pointing to the local API by default.

Please also view our [Developer Flow](https://docs.google.com/presentation/d/101-nxl0kIHe65SANeXf-Ub-5C54Hwiz3084Z8bfi0PI/edit#slide=id.p)