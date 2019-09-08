# Serverless Environment Variables per Stage
This project is a simple example using staging development on AWS Lambda (dev, staging, prod and also local) for environment variables.

# serverless-offline
To run locally, first install all dependences just typing:

    $ npm i

and then run:

    $ node_modules/.bin/serverless offline start

# serverless-stage-manager
This project uses `serverless-stage-manager` plugin. And it was based on a very useful article on **Jeremy Daily**:  https://www.jeremydaly.com/how-to-manage-serverless-environment-variables-per-stage/.


## Visual Studio Code
I recommend using [VSCode](https://code.visualstudio.com/)  for editing and run this test.
Follow the configuration to run this test offiline ON VSCode:

    {
	    "type": "node",  
    	"request": "launch",
    	"name": "Serverless AWS",
    	"program": "${workspaceFolder}/node_modules/.bin/serverless",
    	"args": ["offline", "start", "-s", "local"]
    }

**this code is contained on* `.vscode` *directory.*