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
	"ViewportOrder": {{integer}} List of Viewport Numbers, i.e. successfully update view numbers
	"Succeed": {bool} Successfully updated Viewport Numbers
		
Revit Version: >= 2016
Dynamo Version: 1.2.1
Dependent Packages (version number): custom node
	Archi-lab (v2016.12.10, v2015.11.12)*: Get Builtin Parameter, Set Builtin Parameter
	Hollandaise (v2015.12.23): Viewport.Pts

Notes
	*	If you prefer installing Hollandaise manually than just including package path H:\BIM\Dynamo\Official Release\sasaki-dynamo-dependency-master\nodes: 
		Version of Archi-lab package higher than v2015.11.12 may cause issue when installing Hollandaise. If you have higher version of Archi-lab: 
		1)uninstall Archi-lab under Packages>Manage Packages; 
		2)restart Revit and Dynamo; 
		3)install Hollandaise, then Archi-lab (v2015.11.12) will be installed automatically.

Tested Projects: 66013.00, 56173.00, 56295.00
Reviewed By: Yuiying Cui
Reference: 
	[1] https://vimeo.com/150452601



