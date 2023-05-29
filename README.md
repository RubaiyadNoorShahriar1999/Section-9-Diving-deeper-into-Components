# Section-9-Diving-deeper-into-Components
Diving deeper into Components

Section 9 contains:

        1. Running...
        

<h2>To run this project</h2>

    1. Download the zip/ clone the repository
    2. Open with an IDE (Visual Studio Code recommended)
    3. Open terminal in VS Code and run - npm install
    4. Copy the server localhost link and open it in a browser/ ctrl + right click on the link

<h2>Special Instruction</h2>
Open package.json and replace the script section with this:

            "scripts": {
            "serve": "set NODE_OPTIONS=--openssl-legacy-provider &&  vue-cli-service serve",
            "build": "vue-cli-service build",
            "lint": "vue-cli-service lint"
          },
