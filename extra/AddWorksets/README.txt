Custom Node: AddWorksets.dyf
Author: Ilaria Giardiello
Datetime: 08/15/2016

Function:
	Add standard worksets to central file and set their default visibility
Input
	"Activate": {bool} Set to true to run the node
 		default value: "false"

	"AddWorksets": {{string, bool_string}, {string, bool_string}} List of worksets to add to the central file and their corresponding default visibility setting. Example: {{WorksetName, true}, {WorksetName, false}}
		optional: ignore this input then use the default value which embedded in the node (Sasaki standard worsets)
Output
	"NewWorksets": {string} Worksets successfully added to the central file. The node will only add worksets that are not existing yet

Revit Version: >= 2016
Dynamo Version: 1.0.0
Dependent Packages (version number): custom node
	None

Tested Projects: New generic project with 2016 Revit Standard Template, New generic file without Sasaki template
Reviewed By: Yueying Cui
Reference: 
	[1] http://revitapisearch.com/html/cc477191-cc03-6dbf-48b7-fd08f83d75b6.htm
	[2] http://forums.autodesk.com/t5/revit-api/revit-2016-workset-create-with-visible-in-view-set-to-off/td-p/5772531
