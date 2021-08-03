# MOOC OpenLayers

## Get started with the project

Below are the instructions to get started with the development environment and the project on Ubuntu, Windows and other OSs.

### On Ubuntu, Debian, and related Linux distributions

- Install Node.js:
   ```shell
   sudo apt update
   sudo apt install nodejs
   sudo apt install npm
   ```

- Install Atom or any code editor of your choice:
   ```bash
   wget -qO - https://packagecloud.io/AtomEditor/atom/gpgkey | sudo apt-key add -
   sudo sh -c 'echo "deb [arch=amd64] https://packagecloud.io/AtomEditor/atom/any/ any main" > /etc/apt/sources.list.d/atom.list'
   sudo apt-get update
   sudo apt-get install atom
   ```

- Create an empty directory for the project
   ```bash
   mkdir my-project
   cd my-project
   ```

- In the newly created folder, initialize the Node.js project:
   ```bash
   npm init
   ```

- Add the OpenLayers and Parcel packages to the application:
   ```bash
   npm install ol
   npm install --save-dev parcel-bundler
   ```

### On Windows and other OSs

- Install Node.js: download the installer from [[here]](https://nodejs.org/en/download/)

- Install Atom or any code editor of your choice: download the installer from [[here]](https://atom.io/)

- Create an empty directory for the project.

- In the newly created folder, initialize the Node.js project using the command line:
   ```bash
   npm init
   ```

- Add the OpenLayers and Parcel packages to the application:
   ```bash
   npm install ol
   npm install --save-dev parcel-bundler
   ```

### After the installation

After having followed the above steps, create two files:
- `index.html` containing the HTML code, CSS styles, and the map container;
- `index.js` containing the JavaScript code for your mapping application.

You also have to add a start script line in the `package.json` file (the file is automatically created with `npm init` in the previous steps) to easily run your application with Parcel:

```json
...
"scripts": {
  "test": "echo \"Error: no test specified\" && exit 1",
  "start": "parcel index.html",
  "build": "parcel build --public-url . index.html"
},
...
```

Once some code has been written in the `index.html` and `index.js` files, you will be able to test you code by running:

```bash
npm start
```

in your project directory. You can now test your web mapping application opening the URL [http://localhost:1234/](http://localhost:1234/) in your favorite browser.


## Essential concepts seen during the course

### OpenLayers Classes
* Map: https://openlayers.org/en/latest/apidoc/module-ol_Map-Map.html
* View: https://openlayers.org/en/latest/apidoc/module-ol_View-View.html
* Layer: https://openlayers.org/en/latest/apidoc/module-ol_layer_Layer-Layer.html
* Source: https://openlayers.org/en/latest/apidoc/module-ol_source_Source-Source.html

### Project Diagram

This diagram represent the various classes and attributes used in the project as well as their interrelations:

![alt text](https://github.com/faselm/mooc-openlayers-project/blob/main/diagrams/diagram-2.10.png "Diagram")

## Web Resources
* OpenLayers Homepage: https://openlayers.org
* OpenLayers API: https://openlayers.org/en/latest/apidoc/
* OpenLayers Examples: https://openlayers.org/en/latest/examples/
* OpenLayers Package: https://www.npmjs.com/package/ol
* OpenLayers on GitHub: https://github.com/openlayers/openlayers
* Node.js: https://nodejs.org
* Atom Editor: https://atom.io/
