# MOOC OpenLayers

## Get started with the project

Below are the instructions to get started with the development environment and the project on Ubuntu, Windows and other OSs.

### On Ubuntu, Debian, and related Linux distributions

- Install Node.js:
   ```
   sudo apt update
   sudo apt install nodejs
   sudo apt install npm
   ```

- Install Atom or any code editor of your choice:
   ```
   wget -qO - https://packagecloud.io/AtomEditor/atom/gpgkey | sudo apt-key add -
   sudo sh -c 'echo "deb [arch=amd64] https://packagecloud.io/AtomEditor/atom/any/ any main" > /etc/apt/sources.list.d/atom.list'
   sudo apt-get update
   sudo apt-get install atom
   ```

- Create an empty directory for the project
   ```
   mkdir my-project
   cd my-project
   ```

- In the newly created folder, initialize the Node.js project:
   ```
   npm init
   ```

- Add the OpenLayers and Parcel packages to the application:
   ```
   npm install ol
   npm install --save-dev parcel-bundler
   ```

### On Windows and other OSs

- Install Node.js:
   Download the installer from [[here]](https://nodejs.org/en/download/)

- Install Atom or any code editor of your choice:
   Download the installer from [[here]](https://atom.io/)

- Create an empty directory for the project

- In the newly created folder, initialize the Node.js project:
   ```
   npm init
   ```

- Add the OpenLayers and Parcel packages to the application:
   ```
   npm install ol
   npm install --save-dev parcel-bundler
   ```

After these steps, you will create two files:
- `index.html` containing the HTML, CSS and map container.
- `index.js` containing the JavaScript code for your map.

Once the code of these files will be written, you can test you code by running:
   ```
   npm start
   ```

in your project directory, and opening the URL [http://localhost:1234/](http://localhost:1234/) in your favorite browser.


## Essential concepts seen during the course

### OpenLayers Classes
* Map: https://openlayers.org/en/latest/apidoc/module-ol_Map-Map.html
* View: https://openlayers.org/en/latest/apidoc/module-ol_View-View.html
* Layer: https://openlayers.org/en/latest/apidoc/module-ol_layer_Layer-Layer.html
* Source: https://openlayers.org/en/latest/apidoc/module-ol_source_Source-Source.html

### Project Simplified Diagram
![alt text](https://github.com/faselm/mooc-openlayers-project/blob/main/diagrams/diagram-2.10.png "Diagram")

## Resources
* OpenLayers Homepage: https://openlayers.org
* OpenLayers API: https://openlayers.org/en/latest/apidoc/
* OpenLayers Examples: https://openlayers.org/en/latest/examples/
* OpenLayers Package: https://www.npmjs.com/package/ol
* OpenLayers on GitHub: https://github.com/openlayers/openlayers
* Node.js: https://nodejs.org
* Atom Editor: https://atom.io/
