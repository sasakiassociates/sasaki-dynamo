Custom Node: NumberRoomByGrid.dyf
Author: Yueying Cui
Datetime: 05/19/2016

Input
	"Prefix": grid name prefix
		default value: ""
		optional: have a special grid for room numbering, e.g. prefix by "_"
	"Rooms": rooms to be updated
		optional: apply filter to the room list
	"LevelNumbers": the shortname to present the level name in the room number
	"LevelNames": all level names
Output
	"RoomsWithoutLocation": room(s) without location information, e.g. doesn't delete from the room schedule
		optional: click the green ID to view the room in Revit
	"RoomNumbers": successfully set room numbers

Revit Version: >= 2015
Dynamo Version: 0.9.1
Dependent Packages (version number): custom node
	Archi-lab (v2016.2.1): Get Elements by Category/level
	Clockwork for Dynamo (v0.9.x 0.90.5)
	If Equal Return Index (v0.1.0): If Equal Return Index
	LunchBox for Dynamo (v2015.11.28)
	Rhythm (v2016.2.1)
	If Null Replace with New Value (v0.0.1)
	Phasing Stuff (v0.1.5)
	Get To-From Room (v2.0.0)

Tested Projects: 56170.00, 56192.02, 56295.00, 56173.00
Example Revit Model: G:\56295.00\3.0_Working\3.8_Revit\Dynamo Test\56295.00_SEU_RES 
Reviewed By: Ilaria Giardiello
Reference: 
	[1] http://dynamobim.org/forums/topic/numbering-doors-based-on-a-grid/