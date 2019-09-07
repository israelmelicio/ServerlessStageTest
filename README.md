# Serverless Environment Variables per Stage

This project is a simple example using staging development on AWS Lambda (dev, staging, prod and also local) for environment variables.

# serverless-offline

To run locally, first install all dependences just typing:

    $ npm i

and then run:

    $ node_modules/.bin/serverless offline start

## Visual Studio Code

I recommend using [VSCode](https://code.visualstudio.com/)  for editing and run this test.
Follow the configuration to run this test offiline ON VSCode:

    {
	    "type": "node",  
    	"request": "launch",
    	"name": "Serverless AWS",
    	"program": "${workspaceFolder}/node_modules/.bin/serverless",
    	"args": ["offline", "start"]
    }

