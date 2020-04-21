# P2K
Spreadsheet to display paleomagnetic data


1. Introduction

This macro enabled Excel spreadsheet creates symbols to represent paleomagnetic data in a KML file for visualizing using virtual globes such as Google Earth. The spreadsheet is described in the following paper:
Mochales, T., Blenkinsop, T.G., 2014. Representation of paleomagnetic data in virtual globes (a case study from the Pyrenees). Comput. Geosci. 70, 56–62. doi:10.1016/j.cageo.2014.05.013

Download the P2K spreadsheets and the zipped cones and arches Folders and P2KBoltana.kml into a single folder onto your desktop. Unzip the cones and arches folders.

From your virtual globe, open the example file P2KBoltana.kml in the P2Kfolder. You can appreciate all the basic attributes of P2K from this example. If you additionally open S2KBoltana.kml, you can see structural symbols corresponding to the bedding orientations at each station.


2. Create a KML file from your own data

1.	Open the P2K workbook in Excel.
For Macintosh with the Catalina OS,: Use P2Kv2.xlsm
For Excel Windows or Macintosh 2011: Use P2K.xlsm
For Excel Windows 2007 and 2004 Macintosh: Use P2K.xls

Make sure that the macro is enabled:
Macintosh: Enable macros when asked by the dialogue box.
Windows 2011: File -> Options-> Trust Center-Trust Center settings-> Macro settings-> Enable all macros

2.	Enter a folder name in cell B1 of the first Worksheet. This name will become the name of a folder within the kml document. A worksheet may correspond to a particular lithology or a structural domain. Cells with thick black borders require entries. You can overwrite the values that are supplied in Blanksheet1.

3.	Enter the Scale and Height factors in cells D1 and F1: use the default values of 50 and 2000 to begin with.

4. 	Add your data, starting in row 3:
•	Column 1 is the Site Name
•	Columns A and B are UTM coordinates – these are optional.
•	Columns C and D are latitude and longitude as decimal degrees, negative latitudes in the southern hemisphere. The WGS84 datum must be used. No data are read from any row without an entry in column C.
•	Columns E and F are the Azimuth and Inclination. 
•	Column H is the Alpha95
•	Column I is the Polarity: N for Normal, |-R| indicates normalised reverse polarity (shown in black arrow in the kml file)
•	Column J is the Author. This appears in the pop-up of the site information
•	Column K is the Azimuth of the reference pole
•	Column L is the sense of rotation: C (clockwise) or A (anticlockwise)


8. 	Run the KMLCreator macro when you have entered and saved your data: 
Macintosh: Under Tools -> Macro -> Macros
Windows: View -> Macros -> View Macros
Select and run the KMLCreator macro

9. 	Open the kml file in your virtual globe. The kml document will be created in the S2K folder, with the same name as the workbook (e.g. P2K.kml). The kml file must reside in the same folder as the workbook and the Symbols folder.


Advanced Options

1.	You can edit any symbol by opening the model file from the SketchUpModels folder in Google SketchUp. Export the edited model to the Symbols folder as a Collada (.dae) model, with a similar name to those in the folder.
2.	You can create a stand-alone kmz file to export your results by selecting the kml file and the Symbols folder, and the Stereonet.jpg and Key.jpg files if you have them, and compressing them together. Replace the .zip suffix by .kmz


Additional References

Bentham, P.A., 1992. The tectono-stratigraphic development of the western oblique
 ramp of the south-central Pyrenean thrust system, Northern Spain. Ph.D. thesis,
 University of Southern California. 253 p.

Parés, J.M., Dinarès, J., 1993. Magnetic fabric in two sedimentary rock types from the
 Southern Pyrenees. J. Geomag. Geoelectr 45, 193-205.

Pueyo, E.L., 2010. Evaluating the paleomagnetic reliability in folds and thrust belt
 studies. In: Marcos, A., Poblet, J. (Eds.), Trabajos de Geologia, vol. 30, pp. 145-154 (1).


