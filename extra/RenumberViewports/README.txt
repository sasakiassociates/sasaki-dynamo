Custom Node: RenumberViewports.dyf
Author: Mengyao Yu
Datetime: 09/19/2016

Input
	"SheetNumber": sheet to be worked on, type in sheet number same as shown on the sheet
	"SortOrder": either x or y as sort order
		x: sort view numebrs vertically (sasaki standard)
		y: sort view number horizontally (works better on elevation sheets)
	"TitleBlockMargins": right, left, top, bottom margins of title block, measured in feet.
		Sasaki Standard Title Block Margins are:
			Right: 0.36
			Left: 0.13
			Top: 0.04
			Bottom: 0.04
Output
	"ViewportOrder": 
		List of Viewport Numbers: successfully update view numbers
		List of "1"s: failed update view numbers**
		
Revit Version: >= 2016
Dynamo Version: 1.2.1
Dependent Packages (version number): custom node
	Archi-lab (v2015.11.12)*: Get Builtin Parameter, Set Builtin Parameter
	Hollandaise (v2015.12.23): Viewport.Pts, Sheet.GetViewports

Notes
	*	Higher Version of Archi-lab package may cause issue in Dynamo versions previous to V1.2. If you have higher version of Archi-lab: 
		1)uninstall Archi-lab under Packages>Manage Packages; 
		2)restart Revit and Dynamo; 
		3)install Hollandaise, Archi-lab (v2015.11.12) will be installed automatically.
	**	If you get a list of "1"s as output, it may be caused by:
		1)Packages are not installed correctly, please make sure all packages are in the correct version.
		2)Some of the nodes are not activated.To manually activate it, double click on the custom node to open it, manually open the dyf file shown as red. Save and close.
		  Downloaded dyf files could be found here: C:\Users\name\AppData\Roaming\Dynamo\0.9\packages
		3)The custom node is not activated. To manually activate it, double click on the custom node to open it, unlink and relink any note. Save and close.

Tested Projects: 66013.00, 56173.00, 56295.00
Reviewed By: Yuiying Cui
Reference: 
	[1] https://vimeo.com/150452601



