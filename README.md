Instructions for using Github Codespaces
Prerequisites:
Github account (Both for you and the Candidate).

While not required it would be best for this to be a personal account
Access to the repository with all the projects setup (https://github.com/LGNDLeviathan/TechnologyAssessment)

LiveShare plugin

You can create a codespace from the repository or use the existing one. To create a new one, click on the code button and create codespace on main. Once this has been joined you should setup any necessary plugins such as LiveShare and any java or syntax highlighting plugins as suggested by Visual Studio.

Compilation and Running for the first time:
First unzip the required language using the following command unzip {filename.zip}
When running the projects for the first time ensure the tests can be run

Java
run ./gradlew test

If you get the error bash: ./gradlew: Permission denied then run the following command chmod +x ./gradlew. This will give gradlew execution permissions and allow it to be run. After running it the tests should run but fail.

Python
run python3 test_main.py

Javascript
To check npm is working, type npm -v into the Visual Studio Code terminal (note - npm commands will only work in the Node.js or Visual Studio Code terminal)

Run the following commands:

npm install
npm test or npm t to run all tests.
C Sharp
Download the .NET Core 3.0 SDK: wget https://download.visualstudio.microsoft.com/download/pr/7b1e6b8c-8f8e-4b1e-8b1e-8b1e8b1e8b1e/dotnet-sdk-3.0.100-linux-x64.tar.gz -O dotnet-sdk-3.0.100-linux-x64.tar.gz
Extract the SDK: mkdir -p $HOME/dotnet && tar zxf dotnet-sdk-3.0.100-linux-x64.tar.gz -C $HOME/dotnet
Then set up environment variables:
export DOTNET_ROOT=$HOME/dotnet
export PATH=$PATH:$HOME/dotnet
You can verify the installation was successful with the following command: dotnet --version

After doing this you can compile and run the project using the following two commands

dotnet build
dotnet test
If you need any further guidance each project has a readme with further information on how to run each project.

Setting up and running Liveshare:
Make sure that the live share plugin is installed in your Codespace. Click the Live Share button at the bottom of the screen and share the link to join with the Candidate. They will need to sign in to their personal github account to be able to edit. Guests only have read-only access. Once they have joined you will see a cursor with their position in the code.

You both can now edit the code freely and run commands as necessary.
