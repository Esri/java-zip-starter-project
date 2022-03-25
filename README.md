# java-zip-starter-project

Here is a starter project for the ArcGIS Runtime SDK for Java with the SDK zip.

Make sure you have downloaded the Runtime SDK for Java and OpenJFX 11.0.2.

The app launches a window displaying a map.

![screenshot](screenshot.png)

## Instructions

### IntelliJ IDEA

1. Open IntelliJ IDEA and select _File > Open..._.
2. Choose the java-zip-starter-project directory and click _OK_.
3. Copy the libs, jniLibs, and resources directories from the unpacked SDK zip into the project root.
4. Copy the unpacked Javafx SDK into the project.
5. Create a "bin" directory in the root of the project. This is where your compiled source will go.
6. Select _File > Project Structure..._ to bring up the _Project Structure_ dialog.
7. Under _Project_, ensure that the Project SDK and language level are set to use Java 11. Select the bin folder you created in the _Project compiler output_ field.
8. Under _Modules_, select the java directory under src/main and mark it as _Sources_.
9. Under _Libraries_, add a new _Java_ library. In the _Select Project Files_ dialog, select all of the jars inside the libs directory you copied earlier.
10. Add another _Java_ library. This time select all of the jars in the javafx-sdk-11.0.2/lib directory.
11. In the main menu, select _Run > Edit Configurations..._. Create a new _Application_ type configuration called `App`. In the _Main class_ field, enter `com.mycompany.app.App`. In the _VM options_ field, enter `--module-path ./javafx-sdk-11.0.2/lib --add-modules=javafx.controls,javafx.fxml,javafx.web,javafx.swing,javafx.media`. Then click _OK_.
12. Build the project by selecting _Build > Build Project_. You should see output created in the bin folder.
13. To run the app, select _Run > \`App\`.

### Eclipse

1. Open Eclipse and select _File > Open Projects from File System..._.
2. In the wizard, select the java-zip-starter-project in the _Import source_ field. Then click _Finish_.
3. Copy the libs, jniLibs, and resources directories from the unpacked SDK zip into the project root.
4. Copy the unpacked Javafx SDK into the project.
5. Create a "bin" directory in the root of the project. This is where your compiled source will go.
6. Right-click the project in the _Project Explorer_ or _Package Explorer_ and select _Build Path > Configure Build Path..._.
7. Under _Java Build Path_, in the _Source_ tab, choose _Add Folder..._ and select the java directory under src/main. In the _Default output folder_ field, choose the bin folder you created earlier.
8. In the _Libraries_ tab, select _Modulepath_ and click _Add Library..._. Add a JRE System Library pointing to your JDK 11 installation.
9. Select _Classpath_ and click _Add JARs..._. Select all of the jars from the libs folder you copied earlier and all of the jars in the javafx-sdk-11.0.2/lib directory.
10. Choose _Apply and Close_ to save the changes.
11. Make sure the project is set to build automatically: _Project > Build Automatically_ is checked.
12. In the main menu, select _Run > Run Configurations..._. Create a new _Java Application_ type configuration called `App`. In the _Main class_ field, enter `com.mycompany.app.App`. In the _Arguments_ tab, enter the following _VM arguments_: `--module-path ./javafx-sdk-11.0.2/lib --add-modules=javafx.controls,javafx.fxml,javafx.web,javafx.swing,javafx.media`.
13. Click _Run_ to run the app.

## Requirements

See the Runtime SDK's [system requirements](https://developers.arcgis.com/java/reference/system-requirements/).

## Resources

* [ArcGIS Runtime SDK for Java](https://developers.arcgis.com/java/)  
* [ArcGIS Blog](https://blogs.esri.com/esri/arcgis/)  
* [Esri Twitter](https://twitter.com/esri)  

## Issues

Find a bug or want to request a new feature?  Please let us know by submitting an issue.

## Contributing

Esri welcomes contributions from anyone and everyone. Please see our [guidelines for contributing](https://github.com/esri/contributing).

## Licensing

Copyright 2019 Esri

Licensed under the Apache License, Version 2.0 (the "License"); you may not 
use this file except in compliance with the License. You may obtain a copy 
of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software 
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT 
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the 
License for the specific language governing permissions and limitations 
under the License.

A copy of the license is available in the repository's license.txt file.
