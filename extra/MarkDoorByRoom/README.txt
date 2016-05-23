Custom Node: MarkDoorByRoom.dyf
Author: Yueying Cui
Datetime: 05/19/2016

Input
	"RoomSource": mark door by From Room/To Room
		to: numbered by To Room
		from: numbered by From Room
	"LetterRequired": required to have letter as suffix
		True: e.g. 101A, 102A, 102B
		False: e.g. 101, 102A, 102B
	"Doors": doors to be marked by room
		optional: apply filter to the input door list
Output
	"DoorsNewMarks": successfully update Door marks
	"DoorsWithoutSourceRoom": doors without source room
		optional: click the green ID to view the door in Revit
	"DoorsRemarked": successfully updated Door elements
		optional: click the green ID to view the door in Revit
	"DoorsWithoutLocation": doors without location
		optional: click the green ID to view the door in Revit

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

Notes
	Make sure your door’s “from room” and “to room” properties are showing correctly. If you flip the door, both properties should be changed accordingly. If not, open the door family, then check on “room calculation point” in the Properties palette. [3]

Tested Projects: 56170.00, 56192.02, 56295.00, 56173.00
Example Revit Model: G:\56295.00\3.0_Working\3.8_Revit\Dynamo Test\56295.00_SEU_RES 
Reviewed By: Mengyao Yu
Reference: 
	[1] http://autodeskvasari.com/forum/topics/getting-a-door-s-from-room-and-to-room-numbers
	[2] http://archi-lab.net/doorwindow-numbering-with-dynamo/
	[3] https://knowledge.autodesk.com/support/revit-products/learn-explore/caas/CloudHelp/cloudhelp/2016/ENU/Revit-Model/files/GUID-D45D0FAD-E192-419C-8F58-0F39DAAAE774-htm.html