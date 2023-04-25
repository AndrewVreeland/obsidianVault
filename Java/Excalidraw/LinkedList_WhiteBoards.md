---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
1 ^tChXbpS7

2 ^C2CSer7M

3 ^HZTaUfkS

4 ^zCEp81xy

I need to add to the end of a link list ^MISTHn40

1. check to see if link list is null
2. create temp node and equate it to head
3. use a while loop and loop through the linked list
4. set the truthy value to be temp.next != null
5. when null is = to next assign temp.next to newNode ^rImK9ueP

what to do if the head is null
what to do if the list is null 
are there anymore edge cases that I did not cover?  ^eYl3NsxI

Temp ^ylhBVFW0

newNode ^3JUaWdfG

when temp is = to 4 newNode goes here ^RexV0ix3

Node newNode = new Node()
if (newNode == null){
head = newNode;
}else{
Node temp = head;
while(temp.next != null){
temp = temp.next;
}
temp.next = newNode;
} ^E50t6tWh

The Time complexity will be O(n) due to the fact that 
    the time to complete will relate to the length of
the Linked list, into infinity.

The space complexity will be O(1) due to the fact that 
the nodes will take up the same space for each node 
created.
 ^xWUXqUIO

1 ^qdNLs9dm

2 ^ELs5BNO2

3 ^JmHTDAwY

4 ^2lel1EqP

INPUT(3,8) ^67mQuzfH

8 ^MBFClbng

Insert Before ^D6waXs4I

1. Check to see if Linked list is null
2. check to see if the first value of the input is null 
3. create temp node & create prevTemp node
5. assign temp node to list.head
6. use while loop to loop through linked list 
7. set truthy statement for while top to temp != null
8. the temp needs to be one ahead then the previous temp
9. when temp hits the value after  ^xYwU66HG

public void insertBefore(int value, int newValue)
throw IllegalArgumentException{   
 if(head == null){
        throw new IllegalArgumentException("value not in list")
}
Node temp = head;
Node prevNode = null;
Node newNode = new Node(newValue)

if (temp.value == value){
    newNode.next = temp;
    head = newNode;
    return;
}

while(temp.next != null){
prevTemp = temp;
temp = temp.next;
if(temp.value == value){
newNode.next = temp;
prevTemp.next = newNode;
return;
}
}

} ^GFr8aOXv

This is an edge case incase the value is the first node in the LinkedList. ^RTbc1zm9

Insert after! ^czYakp4V

1 ^S0hMYnUg

2 ^kmG4Hbh1

3 ^7UaSmko6

4 ^iJ5qusjB

5 ^v0rjeYWP

input(3,5) ^6GHh6vRF

The Time complexity will be O(n) due to the fact that 
    the time to complete will relate to the length of
the Linked list, into infinity.

The space complexity will be O(1) due to the fact that 
the nodes will take up the same space for each node 
created.
 ^lJKuSIw4

public void insertBefore(int value, int newValue)
throw IllegalArgumentException{   
 if(head == null){
        throw new IllegalArgumentException("value not in list")
}
Node temp = head;
Node prevNode = null;
Node newNode = new Node(newValue)

if (temp.value == value){
    newNode.next = temp;
    head = newNode;
    return;
}

while(temp.next != null){
prevTemp = temp;
temp = temp.next;
if(prevTemp.value == value){
newNode.next = temp;
prevTemp.next = newNode;
return;
}
}

} ^PVbPGUa4

This is an edge case incase the value is the first node in the LinkedList. ^p3JxAlkY

The Time complexity will be O(n) due to the fact that 
    the time to complete will relate to the length of
the Linked list, into infinity.

The space complexity will be O(1) due to the fact that 
the nodes will take up the same space for each node 
created.
 ^k8gUkxQJ

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/1.8.26",
	"elements": [
		{
			"type": "ellipse",
			"version": 274,
			"versionNonce": 1438220541,
			"isDeleted": false,
			"id": "sM5csOd8VfdjttSPSS14v",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -469.75,
			"y": -151.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 75,
			"height": 60,
			"seed": 451623261,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"id": "Se4xXVpo29vf_iVkt4fTT",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "tChXbpS7"
				}
			],
			"updated": 1682458359844,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 238,
			"versionNonce": 492362067,
			"isDeleted": false,
			"id": "tChXbpS7",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -434.9765033789682,
			"y": -133.95539093559643,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 5.4199981689453125,
			"height": 25,
			"seed": 759588893,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "1",
			"rawText": "1",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "sM5csOd8VfdjttSPSS14v",
			"originalText": "1",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 515,
			"versionNonce": 1208589203,
			"isDeleted": false,
			"id": "Se4xXVpo29vf_iVkt4fTT",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -386.7502600460526,
			"y": -122.24219695622008,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 55.0096496354509,
			"height": 2.000350895834572,
			"seed": 845609619,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682458381655,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "sM5csOd8VfdjttSPSS14v",
				"gap": 8.01549034712371,
				"focus": -0.08839357992163818
			},
			"endBinding": {
				"elementId": "1Tl8tvbtDDVeNl9t9H3tk",
				"gap": 9.665429596346641,
				"focus": 0.1609851129154152
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					55.0096496354509,
					2.000350895834572
				]
			]
		},
		{
			"type": "ellipse",
			"version": 330,
			"versionNonce": 372782835,
			"isDeleted": false,
			"id": "1Tl8tvbtDDVeNl9t9H3tk",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -322.75,
			"y": -143.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 78,
			"height": 59,
			"seed": 1475630707,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"id": "DjhAIIy0jolxJfuL7IKI-",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "C2CSer7M"
				},
				{
					"id": "Se4xXVpo29vf_iVkt4fTT",
					"type": "arrow"
				}
			],
			"updated": 1682458359844,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 238,
			"versionNonce": 834741693,
			"isDeleted": false,
			"id": "C2CSer7M",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -290.94715958346285,
			"y": -126.10183754500315,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 14.239990234375,
			"height": 25,
			"seed": 2064052637,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2",
			"rawText": "2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "1Tl8tvbtDDVeNl9t9H3tk",
			"originalText": "2",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 700,
			"versionNonce": 706130227,
			"isDeleted": false,
			"id": "DjhAIIy0jolxJfuL7IKI-",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -231.75106106860852,
			"y": -112.2421725553717,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 71.00106106860852,
			"height": 1.0000149446283046,
			"seed": 172324147,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682458381656,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "1Tl8tvbtDDVeNl9t9H3tk",
				"gap": 13.031308994320469,
				"focus": 0.07566127010811387
			},
			"endBinding": {
				"elementId": "UIX1tn8ZBtjphQkH5mjH3",
				"gap": 12,
				"focus": 0.03368932271850751
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					71.00106106860852,
					-1.0000149446283046
				]
			]
		},
		{
			"type": "ellipse",
			"version": 315,
			"versionNonce": 292513309,
			"isDeleted": false,
			"id": "UIX1tn8ZBtjphQkH5mjH3",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -148.75,
			"y": -141.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 110,
			"height": 56,
			"seed": 1267617779,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"id": "DjhAIIy0jolxJfuL7IKI-",
					"type": "arrow"
				},
				{
					"id": "9eOudjUL2tgZz45izdEEr",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "HZTaUfkS"
				}
			],
			"updated": 1682458359844,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 238,
			"versionNonce": 204953139,
			"isDeleted": false,
			"id": "HZTaUfkS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -100.45087052385387,
			"y": -125.54117737322332,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 13.6199951171875,
			"height": 25,
			"seed": 2060630931,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "3",
			"rawText": "3",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "UIX1tn8ZBtjphQkH5mjH3",
			"originalText": "3",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 490,
			"versionNonce": 1575764083,
			"isDeleted": false,
			"id": "9eOudjUL2tgZz45izdEEr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -26.78391231291687,
			"y": -116.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 84.10720474441858,
			"height": 0,
			"seed": 1031248829,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682458381657,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "UIX1tn8ZBtjphQkH5mjH3",
				"gap": 12.15377611482355,
				"focus": -0.10714285714285715
			},
			"endBinding": {
				"elementId": "DfUSOYaYD7qdABGejkcQH",
				"gap": 8.52428312128886,
				"focus": 0.17647058823529413
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					84.10720474441858,
					0
				]
			]
		},
		{
			"type": "ellipse",
			"version": 276,
			"versionNonce": 569645011,
			"isDeleted": false,
			"id": "DfUSOYaYD7qdABGejkcQH",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 65.25,
			"y": -137.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 119,
			"height": 51,
			"seed": 1726266707,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "zCEp81xy"
				},
				{
					"id": "9eOudjUL2tgZz45izdEEr",
					"type": "arrow"
				}
			],
			"updated": 1682458359844,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 238,
			"versionNonce": 953696989,
			"isDeleted": false,
			"id": "zCEp81xy",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 118.27715262291605,
			"y": -124.27341042025697,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 12.79998779296875,
			"height": 25,
			"seed": 1776553501,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "4",
			"rawText": "4",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "DfUSOYaYD7qdABGejkcQH",
			"originalText": "4",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "freedraw",
			"version": 263,
			"versionNonce": 300393843,
			"isDeleted": false,
			"id": "cMUgrD14xIVNPAbgS05bb",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -432.75,
			"y": -26.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 17,
			"height": 32,
			"seed": 1539016509,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1
				],
				[
					0,
					-3
				],
				[
					2,
					-6
				],
				[
					3,
					-10
				],
				[
					5,
					-14
				],
				[
					6,
					-17
				],
				[
					7,
					-20
				],
				[
					7,
					-22
				],
				[
					8,
					-23
				],
				[
					8,
					-24
				],
				[
					9,
					-25
				],
				[
					9,
					-26
				],
				[
					9,
					-27
				],
				[
					9,
					-29
				],
				[
					10,
					-31
				],
				[
					10,
					-32
				],
				[
					11,
					-32
				],
				[
					13,
					-29
				],
				[
					14,
					-25
				],
				[
					15,
					-21
				],
				[
					15,
					-17
				],
				[
					16,
					-13
				],
				[
					17,
					-9
				],
				[
					17,
					-7
				],
				[
					17,
					-5
				],
				[
					17,
					-4
				],
				[
					17,
					-4
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 244,
			"versionNonce": 501604157,
			"isDeleted": false,
			"id": "QrqoRNjzAMJJDy4ipOTMd",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -427.75,
			"y": -38.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 9,
			"height": 0,
			"seed": 1228892627,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					4,
					0
				],
				[
					5,
					0
				],
				[
					7,
					0
				],
				[
					8,
					0
				],
				[
					9,
					0
				],
				[
					9,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 244,
			"versionNonce": 56131347,
			"isDeleted": false,
			"id": "qrRo2bCazuEZmzVAVEBi7",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -403.75,
			"y": -47.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 2,
			"height": 17,
			"seed": 2032395763,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					1
				],
				[
					1,
					5
				],
				[
					2,
					8
				],
				[
					2,
					11
				],
				[
					2,
					14
				],
				[
					2,
					16
				],
				[
					2,
					17
				],
				[
					2,
					17
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 254,
			"versionNonce": 1539370909,
			"isDeleted": false,
			"id": "NqmXggUBsvONAtpm4eHz_",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -403.75,
			"y": -49.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 13,
			"height": 7,
			"seed": 303484435,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					-1
				],
				[
					3,
					-1
				],
				[
					5,
					-2
				],
				[
					8,
					-2
				],
				[
					10,
					-2
				],
				[
					11,
					-2
				],
				[
					13,
					-2
				],
				[
					13,
					-1
				],
				[
					13,
					1
				],
				[
					13,
					3
				],
				[
					13,
					4
				],
				[
					12,
					5
				],
				[
					10,
					5
				],
				[
					7,
					5
				],
				[
					4,
					5
				],
				[
					3,
					5
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 245,
			"versionNonce": 1891443891,
			"isDeleted": false,
			"id": "QOvKtgtKH1w_tTxLQfpTx",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -381.75,
			"y": -51.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 1,
			"height": 19,
			"seed": 927588947,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					3
				],
				[
					0,
					6
				],
				[
					1,
					10
				],
				[
					1,
					13
				],
				[
					1,
					16
				],
				[
					1,
					17
				],
				[
					1,
					18
				],
				[
					1,
					19
				],
				[
					1,
					19
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 253,
			"versionNonce": 1620767741,
			"isDeleted": false,
			"id": "5iYldYMRHAEZIDXi6wRgN",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -380.75,
			"y": -51.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 10,
			"height": 8,
			"seed": 843155005,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1
				],
				[
					2,
					-2
				],
				[
					3,
					-2
				],
				[
					5,
					-3
				],
				[
					6,
					-3
				],
				[
					7,
					-3
				],
				[
					8,
					-3
				],
				[
					9,
					-3
				],
				[
					10,
					-1
				],
				[
					10,
					0
				],
				[
					9,
					1
				],
				[
					8,
					2
				],
				[
					6,
					3
				],
				[
					4,
					4
				],
				[
					3,
					5
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 264,
			"versionNonce": 1102845523,
			"isDeleted": false,
			"id": "HqiuTVwua9bLxbKUMzaja",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -355.75,
			"y": -39.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 23,
			"height": 16,
			"seed": 88287923,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					4,
					0
				],
				[
					6,
					0
				],
				[
					9,
					-1
				],
				[
					11,
					-2
				],
				[
					12,
					-3
				],
				[
					13,
					-4
				],
				[
					13,
					-6
				],
				[
					13,
					-7
				],
				[
					11,
					-7
				],
				[
					9,
					-7
				],
				[
					6,
					-7
				],
				[
					2,
					-5
				],
				[
					-1,
					-3
				],
				[
					-2,
					0
				],
				[
					-2,
					1
				],
				[
					-2,
					3
				],
				[
					-1,
					4
				],
				[
					2,
					6
				],
				[
					5,
					8
				],
				[
					9,
					8
				],
				[
					13,
					9
				],
				[
					16,
					9
				],
				[
					19,
					9
				],
				[
					20,
					9
				],
				[
					21,
					9
				],
				[
					21,
					9
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 257,
			"versionNonce": 1484090461,
			"isDeleted": false,
			"id": "sSZdPn6M_WxDGlYYu5etU",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -330.75,
			"y": -39.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 14,
			"height": 15,
			"seed": 896614163,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					1,
					1
				],
				[
					1,
					3
				],
				[
					1,
					4
				],
				[
					1,
					5
				],
				[
					1,
					4
				],
				[
					1,
					2
				],
				[
					2,
					-1
				],
				[
					3,
					-4
				],
				[
					5,
					-7
				],
				[
					6,
					-7
				],
				[
					7,
					-7
				],
				[
					9,
					-7
				],
				[
					11,
					-6
				],
				[
					13,
					-4
				],
				[
					14,
					-1
				],
				[
					14,
					2
				],
				[
					14,
					4
				],
				[
					14,
					7
				],
				[
					14,
					8
				],
				[
					14,
					8
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 267,
			"versionNonce": 623629299,
			"isDeleted": false,
			"id": "kS-jcqoMyO_TViEtejc0d",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -294.75,
			"y": -36.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 10,
			"height": 40,
			"seed": 1304087485,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					-1,
					1
				],
				[
					-3,
					2
				],
				[
					-4,
					2
				],
				[
					-6,
					2
				],
				[
					-7,
					2
				],
				[
					-8,
					2
				],
				[
					-9,
					2
				],
				[
					-10,
					2
				],
				[
					-10,
					0
				],
				[
					-9,
					-2
				],
				[
					-6,
					-6
				],
				[
					-4,
					-7
				],
				[
					-3,
					-7
				],
				[
					-2,
					-7
				],
				[
					-1,
					-7
				],
				[
					-1,
					-6
				],
				[
					0,
					-3
				],
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					2
				],
				[
					0,
					3
				],
				[
					-1,
					3
				],
				[
					-1,
					1
				],
				[
					-1,
					-3
				],
				[
					-1,
					-9
				],
				[
					0,
					-16
				],
				[
					0,
					-26
				],
				[
					0,
					-33
				],
				[
					0,
					-37
				],
				[
					0,
					-37
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 312,
			"versionNonce": 1931598013,
			"isDeleted": false,
			"id": "MISTHn40",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -505.75,
			"y": -15.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 392.79974365234375,
			"height": 25,
			"seed": 1487246483,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "I need to add to the end of a link list",
			"rawText": "I need to add to the end of a link list",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "I need to add to the end of a link list",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "text",
			"version": 509,
			"versionNonce": 722656659,
			"isDeleted": false,
			"id": "rImK9ueP",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -548.75,
			"y": 19.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 537.1595458984375,
			"height": 125,
			"seed": 1755025693,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "1. check to see if link list is null\n2. create temp node and equate it to head\n3. use a while loop and loop through the linked list\n4. set the truthy value to be temp.next != null\n5. when null is = to next assign temp.next to newNode",
			"rawText": "1. check to see if link list is null\n2. create temp node and equate it to head\n3. use a while loop and loop through the linked list\n4. set the truthy value to be temp.next != null\n5. when null is = to next assign temp.next to newNode",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "1. check to see if link list is null\n2. create temp node and equate it to head\n3. use a while loop and loop through the linked list\n4. set the truthy value to be temp.next != null\n5. when null is = to next assign temp.next to newNode",
			"lineHeight": 1.25,
			"baseline": 118
		},
		{
			"type": "freedraw",
			"version": 248,
			"versionNonce": 1782692125,
			"isDeleted": false,
			"id": "KolYcaZjjlT_DY0reqBz1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -527.75,
			"y": 209.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 503,
			"height": 9,
			"seed": 1270431197,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					5,
					0
				],
				[
					12,
					0
				],
				[
					21,
					0
				],
				[
					32,
					0
				],
				[
					45,
					0
				],
				[
					57,
					0
				],
				[
					66,
					0
				],
				[
					75,
					0
				],
				[
					84,
					0
				],
				[
					94,
					0
				],
				[
					105,
					0
				],
				[
					115,
					0
				],
				[
					123,
					0
				],
				[
					129,
					0
				],
				[
					137,
					0
				],
				[
					147,
					0
				],
				[
					159,
					0
				],
				[
					172,
					0
				],
				[
					185,
					0
				],
				[
					194,
					0
				],
				[
					206,
					0
				],
				[
					214,
					0
				],
				[
					226,
					0
				],
				[
					235,
					-1
				],
				[
					244,
					-2
				],
				[
					253,
					-2
				],
				[
					260,
					-2
				],
				[
					267,
					-2
				],
				[
					276,
					-2
				],
				[
					287,
					-3
				],
				[
					299,
					-3
				],
				[
					313,
					-3
				],
				[
					326,
					-4
				],
				[
					337,
					-4
				],
				[
					347,
					-4
				],
				[
					356,
					-4
				],
				[
					362,
					-4
				],
				[
					368,
					-5
				],
				[
					373,
					-5
				],
				[
					377,
					-5
				],
				[
					383,
					-5
				],
				[
					390,
					-6
				],
				[
					397,
					-6
				],
				[
					404,
					-7
				],
				[
					411,
					-7
				],
				[
					419,
					-7
				],
				[
					428,
					-8
				],
				[
					437,
					-8
				],
				[
					446,
					-8
				],
				[
					455,
					-8
				],
				[
					465,
					-8
				],
				[
					472,
					-8
				],
				[
					480,
					-8
				],
				[
					486,
					-8
				],
				[
					490,
					-9
				],
				[
					494,
					-9
				],
				[
					495,
					-9
				],
				[
					496,
					-9
				],
				[
					499,
					-9
				],
				[
					502,
					-9
				],
				[
					503,
					-9
				],
				[
					503,
					-9
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 274,
			"versionNonce": 514306867,
			"isDeleted": false,
			"id": "tal91tFJxcbm4qK4Wweg4",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -458.75,
			"y": -28.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 236,
			"height": 7,
			"seed": 1438273139,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					3,
					0
				],
				[
					5,
					0
				],
				[
					8,
					0
				],
				[
					12,
					1
				],
				[
					17,
					1
				],
				[
					25,
					1
				],
				[
					34,
					1
				],
				[
					44,
					2
				],
				[
					52,
					2
				],
				[
					60,
					3
				],
				[
					67,
					3
				],
				[
					74,
					3
				],
				[
					82,
					4
				],
				[
					89,
					4
				],
				[
					96,
					4
				],
				[
					103,
					5
				],
				[
					109,
					5
				],
				[
					116,
					5
				],
				[
					123,
					5
				],
				[
					130,
					5
				],
				[
					137,
					5
				],
				[
					144,
					5
				],
				[
					151,
					5
				],
				[
					159,
					4
				],
				[
					168,
					4
				],
				[
					176,
					3
				],
				[
					183,
					3
				],
				[
					189,
					2
				],
				[
					196,
					2
				],
				[
					204,
					2
				],
				[
					213,
					1
				],
				[
					223,
					1
				],
				[
					230,
					0
				],
				[
					234,
					-2
				],
				[
					236,
					-2
				],
				[
					236,
					-2
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 246,
			"versionNonce": 1195806077,
			"isDeleted": false,
			"id": "PqaBUol5HfrGv2su5JlEZ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -516.75,
			"y": 163.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 1,
			"height": 30,
			"seed": 1617979613,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					4
				],
				[
					0,
					8
				],
				[
					0,
					14
				],
				[
					0,
					19
				],
				[
					0,
					23
				],
				[
					-1,
					27
				],
				[
					-1,
					29
				],
				[
					-1,
					30
				],
				[
					-1,
					30
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 244,
			"versionNonce": 542168275,
			"isDeleted": false,
			"id": "1hVVDZXoxJO3dzHXoUq5m",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -516.75,
			"y": 161.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 15,
			"height": 0,
			"seed": 1191534365,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					3,
					0
				],
				[
					5,
					0
				],
				[
					8,
					0
				],
				[
					11,
					0
				],
				[
					13,
					0
				],
				[
					15,
					0
				],
				[
					15,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 246,
			"versionNonce": 1769067997,
			"isDeleted": false,
			"id": "kqP42G8LGSIqLGdckTEMZ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -520.75,
			"y": 177.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 0,
			"seed": 475352317,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					3,
					0
				],
				[
					5,
					0
				],
				[
					8,
					0
				],
				[
					12,
					0
				],
				[
					14,
					0
				],
				[
					15,
					0
				],
				[
					16,
					0
				],
				[
					16,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 243,
			"versionNonce": 2141504115,
			"isDeleted": false,
			"id": "9M4kI5GSavQrdM8d_2_Lg",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -516.75,
			"y": 192.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 1,
			"seed": 674802493,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					3,
					1
				],
				[
					6,
					1
				],
				[
					11,
					1
				],
				[
					14,
					1
				],
				[
					16,
					1
				],
				[
					16,
					1
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 271,
			"versionNonce": 1272255037,
			"isDeleted": false,
			"id": "jeOXimsru5AX1dKVDn015",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -481.75,
			"y": 182.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 31,
			"seed": 1267257747,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					1,
					1
				],
				[
					1,
					2
				],
				[
					1,
					3
				],
				[
					0,
					5
				],
				[
					-1,
					6
				],
				[
					-2,
					7
				],
				[
					-3,
					8
				],
				[
					-4,
					8
				],
				[
					-5,
					8
				],
				[
					-6,
					7
				],
				[
					-7,
					4
				],
				[
					-7,
					2
				],
				[
					-7,
					1
				],
				[
					-7,
					-1
				],
				[
					-6,
					-2
				],
				[
					-4,
					-3
				],
				[
					-2,
					-4
				],
				[
					-1,
					-4
				],
				[
					0,
					-4
				],
				[
					1,
					-4
				],
				[
					2,
					-4
				],
				[
					2,
					-3
				],
				[
					3,
					-2
				],
				[
					3,
					0
				],
				[
					3,
					1
				],
				[
					4,
					1
				],
				[
					4,
					0
				],
				[
					5,
					-3
				],
				[
					6,
					-9
				],
				[
					7,
					-15
				],
				[
					7,
					-20
				],
				[
					9,
					-22
				],
				[
					9,
					-23
				],
				[
					9,
					-23
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 271,
			"versionNonce": 1433009171,
			"isDeleted": false,
			"id": "CTsPzwE-eLydRRMnDlbMp",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -453.75,
			"y": 175.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 21,
			"height": 24,
			"seed": 808732637,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					-1,
					1
				],
				[
					-3,
					1
				],
				[
					-5,
					1
				],
				[
					-6,
					0
				],
				[
					-7,
					0
				],
				[
					-7,
					-1
				],
				[
					-7,
					-2
				],
				[
					-7,
					-3
				],
				[
					-5,
					-4
				],
				[
					-2,
					-6
				],
				[
					0,
					-6
				],
				[
					2,
					-6
				],
				[
					3,
					-7
				],
				[
					4,
					-7
				],
				[
					6,
					-7
				],
				[
					7,
					-6
				],
				[
					8,
					-4
				],
				[
					8,
					-1
				],
				[
					8,
					1
				],
				[
					8,
					4
				],
				[
					7,
					7
				],
				[
					5,
					9
				],
				[
					3,
					11
				],
				[
					0,
					13
				],
				[
					-1,
					15
				],
				[
					-3,
					16
				],
				[
					-4,
					17
				],
				[
					-6,
					17
				],
				[
					-7,
					17
				],
				[
					-9,
					17
				],
				[
					-11,
					17
				],
				[
					-12,
					15
				],
				[
					-13,
					15
				],
				[
					-13,
					15
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 274,
			"versionNonce": 189907613,
			"isDeleted": false,
			"id": "smUKspYbp-lhiJLmfC2px",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -440.75,
			"y": 177.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 28,
			"height": 22,
			"seed": 170518963,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					3,
					0
				],
				[
					5,
					0
				],
				[
					9,
					0
				],
				[
					11,
					0
				],
				[
					14,
					0
				],
				[
					17,
					0
				],
				[
					19,
					-1
				],
				[
					20,
					-2
				],
				[
					21,
					-4
				],
				[
					21,
					-5
				],
				[
					21,
					-6
				],
				[
					20,
					-6
				],
				[
					19,
					-6
				],
				[
					16,
					-6
				],
				[
					13,
					-6
				],
				[
					10,
					-6
				],
				[
					8,
					-6
				],
				[
					6,
					-5
				],
				[
					3,
					-3
				],
				[
					1,
					-1
				],
				[
					-1,
					1
				],
				[
					-2,
					3
				],
				[
					-3,
					5
				],
				[
					-3,
					7
				],
				[
					-3,
					8
				],
				[
					-2,
					10
				],
				[
					1,
					11
				],
				[
					5,
					13
				],
				[
					9,
					14
				],
				[
					13,
					15
				],
				[
					17,
					16
				],
				[
					19,
					16
				],
				[
					22,
					16
				],
				[
					23,
					16
				],
				[
					24,
					16
				],
				[
					25,
					16
				],
				[
					25,
					16
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 257,
			"versionNonce": 1570177459,
			"isDeleted": false,
			"id": "ZXfbbFUX_07BzGkNEDsb-",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -383.75,
			"y": 174.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 31,
			"height": 20,
			"seed": 1803137587,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					0
				],
				[
					-2,
					0
				],
				[
					-5,
					0
				],
				[
					-9,
					2
				],
				[
					-11,
					4
				],
				[
					-14,
					6
				],
				[
					-18,
					9
				],
				[
					-20,
					12
				],
				[
					-20,
					14
				],
				[
					-20,
					16
				],
				[
					-20,
					17
				],
				[
					-18,
					17
				],
				[
					-15,
					18
				],
				[
					-11,
					19
				],
				[
					-5,
					19
				],
				[
					1,
					20
				],
				[
					5,
					20
				],
				[
					8,
					20
				],
				[
					10,
					20
				],
				[
					11,
					20
				],
				[
					11,
					20
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 261,
			"versionNonce": 748250877,
			"isDeleted": false,
			"id": "C9I2duw70rtNeMxYMRo66",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -362.75,
			"y": 189.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 19,
			"height": 13,
			"seed": 1763288733,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359844,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					0
				],
				[
					-2,
					1
				],
				[
					-4,
					2
				],
				[
					-5,
					2
				],
				[
					-6,
					2
				],
				[
					-6,
					0
				],
				[
					-6,
					-4
				],
				[
					-5,
					-6
				],
				[
					-2,
					-9
				],
				[
					0,
					-10
				],
				[
					1,
					-11
				],
				[
					2,
					-11
				],
				[
					2,
					-10
				],
				[
					2,
					-9
				],
				[
					2,
					-5
				],
				[
					2,
					-4
				],
				[
					2,
					-2
				],
				[
					2,
					-1
				],
				[
					2,
					0
				],
				[
					3,
					0
				],
				[
					4,
					0
				],
				[
					7,
					0
				],
				[
					11,
					0
				],
				[
					13,
					-1
				],
				[
					13,
					-1
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 271,
			"versionNonce": 290607955,
			"isDeleted": false,
			"id": "e-E5KxDKT4LaEUd06fFzY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -341.75,
			"y": 170.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 7,
			"height": 23,
			"seed": 1021717203,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					0
				],
				[
					-2,
					0
				],
				[
					-3,
					-1
				],
				[
					-3,
					0
				],
				[
					-2,
					0
				],
				[
					-2,
					1
				],
				[
					-2,
					2
				],
				[
					-1,
					4
				],
				[
					-1,
					5
				],
				[
					-1,
					6
				],
				[
					-2,
					6
				],
				[
					-2,
					7
				],
				[
					-3,
					8
				],
				[
					-4,
					9
				],
				[
					-5,
					9
				],
				[
					-5,
					10
				],
				[
					-5,
					11
				],
				[
					-5,
					12
				],
				[
					-4,
					12
				],
				[
					-3,
					12
				],
				[
					-2,
					12
				],
				[
					-1,
					12
				],
				[
					0,
					12
				],
				[
					1,
					12
				],
				[
					1,
					13
				],
				[
					2,
					13
				],
				[
					2,
					14
				],
				[
					2,
					15
				],
				[
					2,
					17
				],
				[
					1,
					18
				],
				[
					0,
					19
				],
				[
					-1,
					21
				],
				[
					-2,
					21
				],
				[
					-2,
					22
				],
				[
					-2,
					22
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 271,
			"versionNonce": 573407069,
			"isDeleted": false,
			"id": "vw5ileJ4QyncWfvdT-6Dr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -324.75,
			"y": 178.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 21,
			"height": 18,
			"seed": 2117005981,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					1,
					1
				],
				[
					2,
					1
				],
				[
					4,
					1
				],
				[
					5,
					1
				],
				[
					7,
					1
				],
				[
					9,
					1
				],
				[
					10,
					0
				],
				[
					11,
					-1
				],
				[
					11,
					-2
				],
				[
					11,
					-3
				],
				[
					11,
					-4
				],
				[
					10,
					-5
				],
				[
					9,
					-5
				],
				[
					8,
					-5
				],
				[
					7,
					-4
				],
				[
					4,
					-3
				],
				[
					2,
					0
				],
				[
					0,
					2
				],
				[
					-1,
					4
				],
				[
					-1,
					6
				],
				[
					-1,
					7
				],
				[
					-1,
					8
				],
				[
					-1,
					10
				],
				[
					-1,
					11
				],
				[
					1,
					12
				],
				[
					3,
					13
				],
				[
					5,
					13
				],
				[
					7,
					13
				],
				[
					9,
					13
				],
				[
					13,
					13
				],
				[
					19,
					12
				],
				[
					20,
					12
				],
				[
					20,
					12
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 267,
			"versionNonce": 15888627,
			"isDeleted": false,
			"id": "PIg4acSDhMkPez-tmiONQ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -291.75,
			"y": 169.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 9,
			"height": 24,
			"seed": 1124455773,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					0
				],
				[
					-2,
					0
				],
				[
					-3,
					0
				],
				[
					-5,
					1
				],
				[
					-5,
					2
				],
				[
					-6,
					3
				],
				[
					-6,
					5
				],
				[
					-7,
					6
				],
				[
					-7,
					7
				],
				[
					-7,
					8
				],
				[
					-6,
					9
				],
				[
					-4,
					9
				],
				[
					-3,
					10
				],
				[
					-2,
					10
				],
				[
					0,
					10
				],
				[
					0,
					11
				],
				[
					1,
					11
				],
				[
					1,
					12
				],
				[
					2,
					13
				],
				[
					2,
					15
				],
				[
					2,
					17
				],
				[
					2,
					19
				],
				[
					0,
					22
				],
				[
					-1,
					23
				],
				[
					-2,
					24
				],
				[
					-3,
					24
				],
				[
					-4,
					24
				],
				[
					-5,
					24
				],
				[
					-6,
					24
				],
				[
					-7,
					24
				],
				[
					-7,
					24
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 248,
			"versionNonce": 308251581,
			"isDeleted": false,
			"id": "0lafGJBr4r2SMf7P99G7W",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -262.75,
			"y": 158.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 20,
			"height": 31,
			"seed": 1151644915,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					-2,
					3
				],
				[
					-5,
					7
				],
				[
					-9,
					11
				],
				[
					-12,
					16
				],
				[
					-15,
					20
				],
				[
					-17,
					24
				],
				[
					-19,
					27
				],
				[
					-20,
					29
				],
				[
					-20,
					30
				],
				[
					-20,
					31
				],
				[
					-20,
					31
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 282,
			"versionNonce": 1845353107,
			"isDeleted": false,
			"id": "RQnOVsgQnjk_GEuaV2y3u",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -233.75,
			"y": 188.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 28,
			"height": 28,
			"seed": 2093110355,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					1,
					3
				],
				[
					1,
					5
				],
				[
					1,
					6
				],
				[
					1,
					7
				],
				[
					0,
					7
				],
				[
					-1,
					7
				],
				[
					-3,
					7
				],
				[
					-6,
					6
				],
				[
					-8,
					4
				],
				[
					-10,
					2
				],
				[
					-10,
					1
				],
				[
					-11,
					0
				],
				[
					-11,
					-3
				],
				[
					-11,
					-6
				],
				[
					-11,
					-10
				],
				[
					-11,
					-12
				],
				[
					-9,
					-15
				],
				[
					-6,
					-17
				],
				[
					-2,
					-19
				],
				[
					1,
					-20
				],
				[
					4,
					-21
				],
				[
					5,
					-21
				],
				[
					6,
					-21
				],
				[
					8,
					-21
				],
				[
					9,
					-21
				],
				[
					11,
					-21
				],
				[
					13,
					-21
				],
				[
					14,
					-20
				],
				[
					16,
					-18
				],
				[
					17,
					-16
				],
				[
					17,
					-13
				],
				[
					17,
					-9
				],
				[
					16,
					-5
				],
				[
					14,
					-1
				],
				[
					12,
					2
				],
				[
					10,
					4
				],
				[
					8,
					5
				],
				[
					6,
					6
				],
				[
					5,
					6
				],
				[
					2,
					7
				],
				[
					1,
					7
				],
				[
					-1,
					7
				],
				[
					-2,
					7
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 245,
			"versionNonce": 1565592605,
			"isDeleted": false,
			"id": "mDlmjow6a--UwWgdVdtOR",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -230.75,
			"y": 180.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 21,
			"height": 11,
			"seed": 1900284755,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2,
					0
				],
				[
					3,
					0
				],
				[
					7,
					3
				],
				[
					10,
					5
				],
				[
					14,
					8
				],
				[
					18,
					10
				],
				[
					19,
					11
				],
				[
					21,
					11
				],
				[
					21,
					11
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 264,
			"versionNonce": 623579187,
			"isDeleted": false,
			"id": "yo2lUTB-4BDoW5P3vJFOs",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -192.75,
			"y": 170.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 11,
			"height": 26,
			"seed": 61476157,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					0
				],
				[
					-2,
					0
				],
				[
					-3,
					0
				],
				[
					-5,
					1
				],
				[
					-6,
					2
				],
				[
					-8,
					4
				],
				[
					-9,
					6
				],
				[
					-9,
					7
				],
				[
					-9,
					8
				],
				[
					-9,
					9
				],
				[
					-9,
					10
				],
				[
					-9,
					11
				],
				[
					-8,
					12
				],
				[
					-7,
					13
				],
				[
					-6,
					14
				],
				[
					-5,
					14
				],
				[
					-4,
					15
				],
				[
					-4,
					16
				],
				[
					-3,
					16
				],
				[
					-3,
					17
				],
				[
					-3,
					18
				],
				[
					-3,
					20
				],
				[
					-4,
					22
				],
				[
					-6,
					24
				],
				[
					-8,
					25
				],
				[
					-10,
					26
				],
				[
					-11,
					26
				],
				[
					-11,
					26
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 245,
			"versionNonce": 1660125309,
			"isDeleted": false,
			"id": "dsGP6b6FlJEnKQzcSR28G",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -204.75,
			"y": 153.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 3,
			"height": 10,
			"seed": 1453217501,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					2
				],
				[
					0,
					3
				],
				[
					-1,
					5
				],
				[
					-2,
					6
				],
				[
					-2,
					8
				],
				[
					-3,
					9
				],
				[
					-3,
					10
				],
				[
					-3,
					10
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 407,
			"versionNonce": 408981971,
			"isDeleted": false,
			"id": "eYl3NsxI",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -553.75,
			"y": 227.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 535.2196044921875,
			"height": 75,
			"seed": 2016141107,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "what to do if the head is null\nwhat to do if the list is null \nare there anymore edge cases that I did not cover? ",
			"rawText": "what to do if the head is null\nwhat to do if the list is null \nare there anymore edge cases that I did not cover? ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "what to do if the head is null\nwhat to do if the list is null \nare there anymore edge cases that I did not cover? ",
			"lineHeight": 1.25,
			"baseline": 68
		},
		{
			"type": "text",
			"version": 259,
			"versionNonce": 151546077,
			"isDeleted": false,
			"id": "ylhBVFW0",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -449.75,
			"y": -186.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 49.539947509765625,
			"height": 25,
			"seed": 602711667,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Temp",
			"rawText": "Temp",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Temp",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "freedraw",
			"version": 275,
			"versionNonce": 951377779,
			"isDeleted": false,
			"id": "IzsPjmfmAGgJ2u_YOe7Q1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -389.75,
			"y": -170.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 80,
			"height": 29,
			"seed": 676311763,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					1,
					-1
				],
				[
					4,
					-4
				],
				[
					7,
					-6
				],
				[
					13,
					-9
				],
				[
					19,
					-12
				],
				[
					24,
					-14
				],
				[
					26,
					-15
				],
				[
					27,
					-15
				],
				[
					30,
					-15
				],
				[
					36,
					-15
				],
				[
					42,
					-14
				],
				[
					49,
					-14
				],
				[
					54,
					-14
				],
				[
					57,
					-13
				],
				[
					60,
					-12
				],
				[
					62,
					-11
				],
				[
					65,
					-10
				],
				[
					67,
					-9
				],
				[
					69,
					-7
				],
				[
					71,
					-5
				],
				[
					72,
					-3
				],
				[
					74,
					0
				],
				[
					75,
					2
				],
				[
					76,
					5
				],
				[
					77,
					8
				],
				[
					78,
					10
				],
				[
					79,
					12
				],
				[
					79,
					13
				],
				[
					79,
					14
				],
				[
					80,
					14
				],
				[
					79,
					14
				],
				[
					75,
					13
				],
				[
					70,
					11
				],
				[
					66,
					9
				],
				[
					62,
					7
				],
				[
					59,
					6
				],
				[
					56,
					5
				],
				[
					55,
					4
				],
				[
					54,
					4
				],
				[
					54,
					4
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 244,
			"versionNonce": 18957629,
			"isDeleted": false,
			"id": "cqj6nJltedpgXWFYFI5sI",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -309.75,
			"y": -157.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 1,
			"height": 31,
			"seed": 202552253,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					1,
					-4
				],
				[
					1,
					-9
				],
				[
					1,
					-15
				],
				[
					1,
					-20
				],
				[
					1,
					-24
				],
				[
					1,
					-27
				],
				[
					1,
					-29
				],
				[
					1,
					-31
				],
				[
					1,
					-31
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 222,
			"versionNonce": 275675411,
			"isDeleted": false,
			"id": "tOhqnLkTtJczVeJcQmilz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -282.75,
			"y": -158.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 136,
			"height": 44,
			"seed": 2146042365,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1
				],
				[
					0,
					-2
				],
				[
					2,
					-3
				],
				[
					4,
					-7
				],
				[
					8,
					-11
				],
				[
					14,
					-16
				],
				[
					23,
					-21
				],
				[
					33,
					-25
				],
				[
					44,
					-29
				],
				[
					55,
					-31
				],
				[
					65,
					-33
				],
				[
					74,
					-34
				],
				[
					82,
					-34
				],
				[
					91,
					-34
				],
				[
					97,
					-32
				],
				[
					103,
					-31
				],
				[
					110,
					-28
				],
				[
					116,
					-26
				],
				[
					121,
					-23
				],
				[
					125,
					-20
				],
				[
					128,
					-17
				],
				[
					130,
					-15
				],
				[
					131,
					-12
				],
				[
					132,
					-9
				],
				[
					133,
					-5
				],
				[
					133,
					-1
				],
				[
					134,
					2
				],
				[
					135,
					5
				],
				[
					135,
					7
				],
				[
					136,
					9
				],
				[
					136,
					10
				],
				[
					135,
					10
				],
				[
					133,
					8
				],
				[
					129,
					7
				],
				[
					125,
					4
				],
				[
					121,
					2
				],
				[
					119,
					2
				],
				[
					117,
					1
				],
				[
					117,
					0
				],
				[
					117,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 246,
			"versionNonce": 1319081373,
			"isDeleted": false,
			"id": "c_4-rXV9NN-GcPnFmtsxK",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -147.75,
			"y": -148.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 12,
			"height": 25,
			"seed": 1936083421,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					3,
					-2
				],
				[
					4,
					-6
				],
				[
					5,
					-11
				],
				[
					6,
					-15
				],
				[
					8,
					-18
				],
				[
					9,
					-21
				],
				[
					11,
					-23
				],
				[
					12,
					-24
				],
				[
					12,
					-25
				],
				[
					12,
					-25
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 263,
			"versionNonce": 486792883,
			"isDeleted": false,
			"id": "Nel2Qr2lHZoWw2WE23CLk",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -109.75,
			"y": -148.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 205,
			"height": 40,
			"seed": 1983018109,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					-2
				],
				[
					3,
					-4
				],
				[
					6,
					-8
				],
				[
					12,
					-14
				],
				[
					16,
					-17
				],
				[
					23,
					-21
				],
				[
					31,
					-25
				],
				[
					39,
					-28
				],
				[
					72,
					-35
				],
				[
					103,
					-36
				],
				[
					130,
					-36
				],
				[
					138,
					-36
				],
				[
					165,
					-30
				],
				[
					172,
					-27
				],
				[
					182,
					-22
				],
				[
					186,
					-19
				],
				[
					190,
					-15
				],
				[
					194,
					-10
				],
				[
					198,
					-6
				],
				[
					201,
					-2
				],
				[
					203,
					1
				],
				[
					205,
					3
				],
				[
					205,
					4
				],
				[
					204,
					4
				],
				[
					201,
					4
				],
				[
					198,
					3
				],
				[
					194,
					2
				],
				[
					191,
					1
				],
				[
					191,
					1
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 246,
			"versionNonce": 213178877,
			"isDeleted": false,
			"id": "TOvCmlkwSeeV7zT0YyDqt",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 99.25,
			"y": -145.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 3,
			"height": 21,
			"seed": 1191614003,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1
				],
				[
					0,
					-3
				],
				[
					0,
					-5
				],
				[
					0,
					-8
				],
				[
					0,
					-10
				],
				[
					0,
					-13
				],
				[
					0,
					-15
				],
				[
					1,
					-17
				],
				[
					2,
					-20
				],
				[
					3,
					-20
				],
				[
					3,
					-21
				],
				[
					3,
					-21
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 215,
			"versionNonce": 1763414099,
			"isDeleted": false,
			"id": "Wpe_F3vMJujoPe6lOPBXS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 156.25,
			"y": -146.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 142,
			"height": 49,
			"seed": 1133125011,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					7,
					-9
				],
				[
					9,
					-11
				],
				[
					14,
					-15
				],
				[
					23,
					-22
				],
				[
					32,
					-30
				],
				[
					41,
					-36
				],
				[
					51,
					-40
				],
				[
					60,
					-44
				],
				[
					68,
					-46
				],
				[
					75,
					-48
				],
				[
					80,
					-49
				],
				[
					86,
					-49
				],
				[
					92,
					-49
				],
				[
					100,
					-46
				],
				[
					108,
					-44
				],
				[
					116,
					-42
				],
				[
					123,
					-39
				],
				[
					127,
					-37
				],
				[
					130,
					-35
				],
				[
					132,
					-34
				],
				[
					132,
					-33
				],
				[
					133,
					-31
				],
				[
					134,
					-30
				],
				[
					135,
					-27
				],
				[
					136,
					-24
				],
				[
					137,
					-20
				],
				[
					139,
					-17
				],
				[
					140,
					-14
				],
				[
					141,
					-12
				],
				[
					141,
					-10
				],
				[
					142,
					-9
				],
				[
					142,
					-9
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 256,
			"versionNonce": 1952617053,
			"isDeleted": false,
			"id": "pfQfLADcYjDUvlcjUrhHr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 276.25,
			"y": -104.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 18,
			"height": 25,
			"seed": 113390461,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1
				],
				[
					0,
					-4
				],
				[
					0,
					-9
				],
				[
					0,
					-14
				],
				[
					3,
					-18
				],
				[
					5,
					-21
				],
				[
					8,
					-24
				],
				[
					9,
					-25
				],
				[
					10,
					-25
				],
				[
					11,
					-25
				],
				[
					12,
					-23
				],
				[
					13,
					-21
				],
				[
					13,
					-17
				],
				[
					13,
					-14
				],
				[
					13,
					-12
				],
				[
					13,
					-10
				],
				[
					14,
					-9
				],
				[
					15,
					-9
				],
				[
					16,
					-9
				],
				[
					17,
					-9
				],
				[
					18,
					-9
				],
				[
					18,
					-9
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 257,
			"versionNonce": 1720454643,
			"isDeleted": false,
			"id": "2m1svs-0AXWkp0TogAYb9",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 297.25,
			"y": -131.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 15,
			"height": 14,
			"seed": 1990688765,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					4
				],
				[
					0,
					6
				],
				[
					0,
					8
				],
				[
					1,
					10
				],
				[
					2,
					10
				],
				[
					3,
					12
				],
				[
					4,
					12
				],
				[
					5,
					13
				],
				[
					6,
					13
				],
				[
					7,
					13
				],
				[
					9,
					13
				],
				[
					11,
					13
				],
				[
					12,
					13
				],
				[
					13,
					13
				],
				[
					14,
					12
				],
				[
					15,
					10
				],
				[
					15,
					7
				],
				[
					15,
					5
				],
				[
					15,
					2
				],
				[
					15,
					0
				],
				[
					15,
					-1
				],
				[
					15,
					-1
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 242,
			"versionNonce": 578436797,
			"isDeleted": false,
			"id": "aIfKvwat5cLHf4WE-Eu3v",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 317.25,
			"y": -137.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 1,
			"height": 18,
			"seed": 419743187,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					1,
					3
				],
				[
					1,
					7
				],
				[
					1,
					11
				],
				[
					1,
					15
				],
				[
					1,
					16
				],
				[
					1,
					18
				],
				[
					1,
					18
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 244,
			"versionNonce": 140236691,
			"isDeleted": false,
			"id": "EGwCSEdFqwCrV5zx0qf4B",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 326.25,
			"y": -137.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 6,
			"height": 22,
			"seed": 1980744179,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					2,
					2
				],
				[
					3,
					6
				],
				[
					3,
					10
				],
				[
					3,
					14
				],
				[
					3,
					18
				],
				[
					4,
					20
				],
				[
					6,
					22
				],
				[
					6,
					22
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 242,
			"versionNonce": 496852765,
			"isDeleted": false,
			"id": "IRzNC2tUMebMzAdbH0wQF",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 297.25,
			"y": -155.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 12,
			"height": 3,
			"seed": 976252851,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					0
				],
				[
					-3,
					-1
				],
				[
					-5,
					-2
				],
				[
					-8,
					-3
				],
				[
					-10,
					-3
				],
				[
					-11,
					-3
				],
				[
					-12,
					-3
				],
				[
					-12,
					-3
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 278,
			"versionNonce": 482438451,
			"isDeleted": false,
			"id": "zDCYXejkJAl3c2eLv61NY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 302.25,
			"y": -159.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 8,
			"height": 19,
			"seed": 22364115,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					-4
				],
				[
					3,
					-8
				],
				[
					5,
					-11
				],
				[
					7,
					-14
				],
				[
					8,
					-16
				],
				[
					8,
					-18
				],
				[
					8,
					-19
				],
				[
					8,
					-19
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "ellipse",
			"version": 348,
			"versionNonce": 473789309,
			"isDeleted": false,
			"id": "k8fYByjGWrJhaloP1_KVJ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 183.25,
			"y": -42.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 130,
			"height": 85,
			"seed": 1357924285,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "3JUaWdfG"
				},
				{
					"id": "4vGrsEc4q2IX5beNklycF",
					"type": "arrow"
				}
			],
			"updated": 1682458359845,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 327,
			"versionNonce": 1730367187,
			"isDeleted": false,
			"id": "3JUaWdfG",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 208.91809462326503,
			"y": -12.294225700428271,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 78.73992919921875,
			"height": 25,
			"seed": 18184093,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "newNode",
			"rawText": "newNode",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "k8fYByjGWrJhaloP1_KVJ",
			"originalText": "newNode",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "text",
			"version": 152,
			"versionNonce": 177994717,
			"isDeleted": false,
			"id": "RexV0ix3",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 125.25,
			"y": -230.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 391.8597106933594,
			"height": 25,
			"seed": 339661757,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "la7kBCV_ezxubWPvJpIry",
					"type": "arrow"
				}
			],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "when temp is = to 4 newNode goes here",
			"rawText": "when temp is = to 4 newNode goes here",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "when temp is = to 4 newNode goes here",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 63,
			"versionNonce": 2048392307,
			"isDeleted": false,
			"id": "la7kBCV_ezxubWPvJpIry",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 387.25,
			"y": -190.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 47,
			"height": 36,
			"seed": 301314515,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "RexV0ix3",
				"focus": -0.480439382044842,
				"gap": 15
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					-47,
					36
				]
			]
		},
		{
			"type": "arrow",
			"version": 41,
			"versionNonce": 1984721981,
			"isDeleted": false,
			"id": "4vGrsEc4q2IX5beNklycF",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 286.2223584632976,
			"y": -55.06844069787062,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 7.02764153670239,
			"height": 44.17374680212938,
			"seed": 1483600275,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682458381658,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "k8fYByjGWrJhaloP1_KVJ",
				"gap": 19.442445633637774,
				"focus": 0.4463677902775953
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					7.02764153670239,
					-44.17374680212938
				]
			]
		},
		{
			"type": "freedraw",
			"version": 45,
			"versionNonce": 1365636627,
			"isDeleted": false,
			"id": "pWNFY7flHq0OjTx38qOf4",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -257.75,
			"y": -34.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 27,
			"height": 45,
			"seed": 2043527581,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1
				],
				[
					1,
					-1
				],
				[
					3,
					-5
				],
				[
					5,
					-11
				],
				[
					8,
					-19
				],
				[
					13,
					-31
				],
				[
					16,
					-35
				],
				[
					19,
					-41
				],
				[
					21,
					-45
				],
				[
					22,
					-45
				],
				[
					23,
					-45
				],
				[
					24,
					-44
				],
				[
					25,
					-41
				],
				[
					27,
					-36
				],
				[
					27,
					-30
				],
				[
					27,
					-24
				],
				[
					27,
					-19
				],
				[
					27,
					-16
				],
				[
					27,
					-14
				],
				[
					27,
					-13
				],
				[
					27,
					-12
				],
				[
					27,
					-12
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 32,
			"versionNonce": 1487562909,
			"isDeleted": false,
			"id": "wPNTOi85w9vtKVRq2AdTM",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -246.75,
			"y": -56.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 19,
			"height": 2,
			"seed": 1056103965,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1
				],
				[
					1,
					-1
				],
				[
					5,
					-1
				],
				[
					10,
					-1
				],
				[
					14,
					-1
				],
				[
					16,
					-2
				],
				[
					18,
					-2
				],
				[
					19,
					-2
				],
				[
					19,
					-2
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 35,
			"versionNonce": 738442163,
			"isDeleted": false,
			"id": "Nv1My0Gzj8mZVezu9b9ag",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -216.75,
			"y": -78.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 4,
			"height": 34,
			"seed": 927407699,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					1
				],
				[
					3,
					4
				],
				[
					4,
					8
				],
				[
					4,
					14
				],
				[
					4,
					19
				],
				[
					3,
					26
				],
				[
					2,
					29
				],
				[
					2,
					32
				],
				[
					2,
					34
				],
				[
					1,
					34
				],
				[
					1,
					34
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 55,
			"versionNonce": 1408060669,
			"isDeleted": false,
			"id": "4VjC65CVM04bK1oFT5BFc",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -194.75,
			"y": -65.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 25,
			"height": 32,
			"seed": 391842227,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					0
				],
				[
					-4,
					-2
				],
				[
					-5,
					-2
				],
				[
					-5,
					-5
				],
				[
					-6,
					-8
				],
				[
					-6,
					-11
				],
				[
					-5,
					-13
				],
				[
					-2,
					-15
				],
				[
					0,
					-15
				],
				[
					4,
					-15
				],
				[
					8,
					-13
				],
				[
					13,
					-9
				],
				[
					16,
					-5
				],
				[
					18,
					-2
				],
				[
					19,
					2
				],
				[
					19,
					6
				],
				[
					19,
					8
				],
				[
					19,
					11
				],
				[
					17,
					14
				],
				[
					16,
					16
				],
				[
					15,
					17
				],
				[
					13,
					17
				],
				[
					12,
					17
				],
				[
					9,
					17
				],
				[
					7,
					17
				],
				[
					3,
					16
				],
				[
					1,
					16
				],
				[
					-1,
					15
				],
				[
					-3,
					14
				],
				[
					-4,
					13
				],
				[
					-4,
					12
				],
				[
					-4,
					12
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 31,
			"versionNonce": 639094099,
			"isDeleted": false,
			"id": "JOyJfP1GAgbxmM_7akAyc",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -194.75,
			"y": -66.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 11,
			"height": 0,
			"seed": 789239123,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					3,
					0
				],
				[
					5,
					0
				],
				[
					7,
					0
				],
				[
					8,
					0
				],
				[
					10,
					0
				],
				[
					11,
					0
				],
				[
					11,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 58,
			"versionNonce": 1108649309,
			"isDeleted": false,
			"id": "SQ83Z5b7_QTiovgbDDetH",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -152.75,
			"y": -57.2421875,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 19,
			"height": 16,
			"seed": 1759256947,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					1
				],
				[
					2,
					2
				],
				[
					2,
					3
				],
				[
					1,
					4
				],
				[
					0,
					5
				],
				[
					-1,
					5
				],
				[
					-5,
					5
				],
				[
					-6,
					4
				],
				[
					-9,
					2
				],
				[
					-11,
					-1
				],
				[
					-12,
					-3
				],
				[
					-12,
					-5
				],
				[
					-12,
					-9
				],
				[
					-12,
					-10
				],
				[
					-11,
					-11
				],
				[
					-10,
					-11
				],
				[
					-8,
					-11
				],
				[
					-6,
					-11
				],
				[
					-3,
					-11
				],
				[
					0,
					-11
				],
				[
					1,
					-11
				],
				[
					3,
					-10
				],
				[
					4,
					-9
				],
				[
					5,
					-8
				],
				[
					6,
					-6
				],
				[
					7,
					-5
				],
				[
					7,
					-2
				],
				[
					7,
					0
				],
				[
					7,
					2
				],
				[
					6,
					4
				],
				[
					5,
					5
				],
				[
					4,
					5
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 49,
			"versionNonce": 318286579,
			"isDeleted": false,
			"id": "KAKNk7TUxShQ-3pfEl2YO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -432.75,
			"y": 329.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 55,
			"height": 34,
			"seed": 1926045181,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1
				],
				[
					-3,
					-1
				],
				[
					-8,
					-1
				],
				[
					-16,
					-1
				],
				[
					-24,
					1
				],
				[
					-32,
					6
				],
				[
					-40,
					12
				],
				[
					-43,
					18
				],
				[
					-44,
					22
				],
				[
					-43,
					24
				],
				[
					-40,
					26
				],
				[
					-35,
					28
				],
				[
					-30,
					30
				],
				[
					-25,
					31
				],
				[
					-19,
					32
				],
				[
					-13,
					32
				],
				[
					-9,
					33
				],
				[
					-7,
					33
				],
				[
					-5,
					33
				],
				[
					-4,
					33
				],
				[
					-1,
					32
				],
				[
					1,
					31
				],
				[
					5,
					30
				],
				[
					9,
					28
				],
				[
					11,
					28
				],
				[
					11,
					28
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 61,
			"versionNonce": 913437117,
			"isDeleted": false,
			"id": "8gRulHVyC1IWtS0ioTDUT",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -394.75,
			"y": 351.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 23,
			"height": 19,
			"seed": 1633808189,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					1,
					1
				],
				[
					1,
					2
				],
				[
					1,
					3
				],
				[
					-1,
					4
				],
				[
					-3,
					5
				],
				[
					-5,
					5
				],
				[
					-7,
					5
				],
				[
					-10,
					5
				],
				[
					-12,
					5
				],
				[
					-13,
					5
				],
				[
					-15,
					3
				],
				[
					-16,
					1
				],
				[
					-17,
					-2
				],
				[
					-18,
					-5
				],
				[
					-18,
					-8
				],
				[
					-18,
					-11
				],
				[
					-18,
					-12
				],
				[
					-17,
					-14
				],
				[
					-15,
					-14
				],
				[
					-13,
					-14
				],
				[
					-10,
					-14
				],
				[
					-6,
					-14
				],
				[
					-2,
					-13
				],
				[
					1,
					-11
				],
				[
					3,
					-11
				],
				[
					4,
					-10
				],
				[
					5,
					-9
				],
				[
					5,
					-8
				],
				[
					5,
					-6
				],
				[
					5,
					-3
				],
				[
					5,
					0
				],
				[
					4,
					2
				],
				[
					3,
					2
				],
				[
					3,
					3
				],
				[
					3,
					4
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 58,
			"versionNonce": 388813971,
			"isDeleted": false,
			"id": "UTN6EaNlyap673D6PZrx5",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -366.75,
			"y": 351.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 40,
			"seed": 223235773,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					1,
					2
				],
				[
					1,
					3
				],
				[
					-2,
					3
				],
				[
					-6,
					3
				],
				[
					-10,
					3
				],
				[
					-12,
					2
				],
				[
					-13,
					2
				],
				[
					-14,
					1
				],
				[
					-14,
					0
				],
				[
					-14,
					-1
				],
				[
					-14,
					-2
				],
				[
					-14,
					-3
				],
				[
					-13,
					-4
				],
				[
					-12,
					-5
				],
				[
					-11,
					-5
				],
				[
					-9,
					-5
				],
				[
					-8,
					-5
				],
				[
					-7,
					-5
				],
				[
					-5,
					-5
				],
				[
					-4,
					-5
				],
				[
					-3,
					-4
				],
				[
					-1,
					-3
				],
				[
					0,
					-2
				],
				[
					1,
					-1
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					2,
					-3
				],
				[
					2,
					-9
				],
				[
					1,
					-17
				],
				[
					0,
					-24
				],
				[
					0,
					-31
				],
				[
					0,
					-35
				],
				[
					0,
					-37
				],
				[
					0,
					-37
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 61,
			"versionNonce": 1579594269,
			"isDeleted": false,
			"id": "mhggX3LkMzwNCUz-SEbWz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -353.75,
			"y": 335.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 27,
			"height": 28,
			"seed": 681228499,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					4,
					0
				],
				[
					9,
					0
				],
				[
					13,
					0
				],
				[
					16,
					0
				],
				[
					17,
					-1
				],
				[
					19,
					-2
				],
				[
					20,
					-3
				],
				[
					21,
					-5
				],
				[
					21,
					-7
				],
				[
					21,
					-10
				],
				[
					21,
					-11
				],
				[
					20,
					-11
				],
				[
					20,
					-12
				],
				[
					18,
					-12
				],
				[
					14,
					-12
				],
				[
					10,
					-12
				],
				[
					6,
					-10
				],
				[
					2,
					-7
				],
				[
					0,
					-4
				],
				[
					-1,
					-1
				],
				[
					-3,
					1
				],
				[
					-4,
					4
				],
				[
					-4,
					5
				],
				[
					-4,
					7
				],
				[
					-4,
					8
				],
				[
					-1,
					11
				],
				[
					3,
					13
				],
				[
					7,
					14
				],
				[
					10,
					16
				],
				[
					12,
					16
				],
				[
					15,
					16
				],
				[
					17,
					16
				],
				[
					19,
					15
				],
				[
					21,
					14
				],
				[
					22,
					13
				],
				[
					23,
					13
				],
				[
					23,
					13
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 57,
			"versionNonce": 40553011,
			"isDeleted": false,
			"id": "zNkG5vCDKUJfg9K21eBFk",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -497.75,
			"y": 368.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 191,
			"height": 10,
			"seed": 973582675,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					1,
					1
				],
				[
					3,
					1
				],
				[
					7,
					1
				],
				[
					12,
					1
				],
				[
					21,
					1
				],
				[
					33,
					0
				],
				[
					47,
					-2
				],
				[
					61,
					-4
				],
				[
					73,
					-6
				],
				[
					81,
					-6
				],
				[
					88,
					-7
				],
				[
					94,
					-7
				],
				[
					102,
					-7
				],
				[
					110,
					-8
				],
				[
					118,
					-8
				],
				[
					126,
					-8
				],
				[
					133,
					-8
				],
				[
					139,
					-8
				],
				[
					146,
					-8
				],
				[
					152,
					-8
				],
				[
					159,
					-8
				],
				[
					164,
					-8
				],
				[
					169,
					-8
				],
				[
					172,
					-8
				],
				[
					176,
					-9
				],
				[
					179,
					-9
				],
				[
					183,
					-9
				],
				[
					185,
					-9
				],
				[
					188,
					-9
				],
				[
					189,
					-9
				],
				[
					190,
					-9
				],
				[
					191,
					-9
				],
				[
					191,
					-9
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 213,
			"versionNonce": 1176790653,
			"isDeleted": false,
			"id": "E50t6tWh",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -467.75,
			"y": 384.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 271.1597900390625,
			"height": 250,
			"seed": 1713812115,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Node newNode = new Node()\nif (newNode == null){\nhead = newNode;\n}else{\nNode temp = head;\nwhile(temp.next != null){\ntemp = temp.next;\n}\ntemp.next = newNode;\n}",
			"rawText": "Node newNode = new Node()\nif (newNode == null){\nhead = newNode;\n}else{\nNode temp = head;\nwhile(temp.next != null){\ntemp = temp.next;\n}\ntemp.next = newNode;\n}",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Node newNode = new Node()\nif (newNode == null){\nhead = newNode;\n}else{\nNode temp = head;\nwhile(temp.next != null){\ntemp = temp.next;\n}\ntemp.next = newNode;\n}",
			"lineHeight": 1.25,
			"baseline": 243
		},
		{
			"type": "freedraw",
			"version": 38,
			"versionNonce": 1771637715,
			"isDeleted": false,
			"id": "ASp3vhlhh5dB5WKc5ZhEc",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 105.25,
			"y": 153.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 25,
			"height": 89,
			"seed": 1257587187,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					3,
					5
				],
				[
					5,
					11
				],
				[
					9,
					21
				],
				[
					12,
					32
				],
				[
					15,
					42
				],
				[
					17,
					51
				],
				[
					19,
					60
				],
				[
					20,
					69
				],
				[
					21,
					77
				],
				[
					23,
					82
				],
				[
					24,
					86
				],
				[
					24,
					88
				],
				[
					25,
					89
				],
				[
					25,
					89
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 65,
			"versionNonce": 1630310109,
			"isDeleted": false,
			"id": "ujjF0cLcdUN6Mgz6PNZ7_",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 102.25,
			"y": 150.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 71,
			"height": 75,
			"seed": 295304637,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					4,
					-1
				],
				[
					6,
					-2
				],
				[
					10,
					-3
				],
				[
					15,
					-4
				],
				[
					23,
					-4
				],
				[
					35,
					-4
				],
				[
					48,
					-3
				],
				[
					58,
					0
				],
				[
					63,
					3
				],
				[
					65,
					5
				],
				[
					65,
					8
				],
				[
					65,
					11
				],
				[
					62,
					13
				],
				[
					58,
					15
				],
				[
					53,
					17
				],
				[
					48,
					18
				],
				[
					42,
					20
				],
				[
					38,
					20
				],
				[
					37,
					20
				],
				[
					38,
					20
				],
				[
					40,
					21
				],
				[
					45,
					22
				],
				[
					53,
					25
				],
				[
					60,
					29
				],
				[
					67,
					34
				],
				[
					69,
					38
				],
				[
					71,
					43
				],
				[
					71,
					48
				],
				[
					71,
					54
				],
				[
					71,
					60
				],
				[
					69,
					66
				],
				[
					66,
					69
				],
				[
					62,
					70
				],
				[
					57,
					71
				],
				[
					52,
					71
				],
				[
					44,
					71
				],
				[
					36,
					71
				],
				[
					31,
					70
				],
				[
					28,
					70
				],
				[
					28,
					70
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 32,
			"versionNonce": 13506931,
			"isDeleted": false,
			"id": "e5Gj0cV0CSOahqrXGZl2-",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 192.25,
			"y": 182.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 12,
			"height": 17,
			"seed": 1700508157,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					4,
					3
				],
				[
					7,
					5
				],
				[
					9,
					9
				],
				[
					11,
					13
				],
				[
					12,
					15
				],
				[
					12,
					17
				],
				[
					12,
					17
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 24,
			"versionNonce": 1305520957,
			"isDeleted": false,
			"id": "-3sxn-K-LFNE-quxjAiFE",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 191.25,
			"y": 164.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 88188019,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 48,
			"versionNonce": 894464787,
			"isDeleted": false,
			"id": "ICFwZ2xt-rBhaGqqJv1mt",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 257.25,
			"y": 147.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 40,
			"height": 50,
			"seed": 301219997,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					1
				],
				[
					-9,
					8
				],
				[
					-11,
					10
				],
				[
					-18,
					16
				],
				[
					-23,
					24
				],
				[
					-26,
					33
				],
				[
					-28,
					40
				],
				[
					-28,
					46
				],
				[
					-26,
					49
				],
				[
					-23,
					50
				],
				[
					-21,
					50
				],
				[
					-18,
					50
				],
				[
					-12,
					48
				],
				[
					-6,
					43
				],
				[
					0,
					38
				],
				[
					6,
					35
				],
				[
					9,
					33
				],
				[
					11,
					30
				],
				[
					12,
					29
				],
				[
					12,
					28
				],
				[
					11,
					28
				],
				[
					8,
					28
				],
				[
					5,
					28
				],
				[
					4,
					28
				],
				[
					4,
					28
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 24,
			"versionNonce": 1550990237,
			"isDeleted": false,
			"id": "bwrw_YC7jW9UblWlBmVJB",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 257.25,
			"y": 174.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 800092371,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 60,
			"versionNonce": 127310003,
			"isDeleted": false,
			"id": "Rc7JlVzQeb6_OnzSm9pVH",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 325.25,
			"y": 179.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 81,
			"height": 83,
			"seed": 237549117,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					3
				],
				[
					0,
					4
				],
				[
					-2,
					5
				],
				[
					-7,
					7
				],
				[
					-13,
					7
				],
				[
					-19,
					7
				],
				[
					-27,
					7
				],
				[
					-35,
					5
				],
				[
					-44,
					1
				],
				[
					-51,
					-4
				],
				[
					-57,
					-11
				],
				[
					-62,
					-20
				],
				[
					-65,
					-33
				],
				[
					-67,
					-45
				],
				[
					-66,
					-58
				],
				[
					-61,
					-68
				],
				[
					-53,
					-74
				],
				[
					-43,
					-76
				],
				[
					-31,
					-76
				],
				[
					-20,
					-72
				],
				[
					-8,
					-66
				],
				[
					2,
					-60
				],
				[
					8,
					-54
				],
				[
					11,
					-48
				],
				[
					13,
					-41
				],
				[
					14,
					-35
				],
				[
					14,
					-29
				],
				[
					13,
					-23
				],
				[
					11,
					-18
				],
				[
					7,
					-13
				],
				[
					3,
					-9
				],
				[
					2,
					-8
				],
				[
					0,
					-7
				],
				[
					-1,
					-7
				],
				[
					0,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 38,
			"versionNonce": 1430437885,
			"isDeleted": false,
			"id": "BPkIrWw4l49QqlRkzRdR_",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 70.25,
			"y": 255.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 301,
			"height": 71,
			"seed": 2036254451,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					0
				],
				[
					18,
					-3
				],
				[
					40,
					-8
				],
				[
					74,
					-14
				],
				[
					112,
					-22
				],
				[
					147,
					-30
				],
				[
					184,
					-39
				],
				[
					218,
					-49
				],
				[
					250,
					-57
				],
				[
					273,
					-63
				],
				[
					287,
					-66
				],
				[
					296,
					-69
				],
				[
					300,
					-70
				],
				[
					301,
					-71
				],
				[
					301,
					-71
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 421,
			"versionNonce": 625412691,
			"isDeleted": false,
			"id": "xWUXqUIO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 6.25,
			"y": 277.7578125,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 559.6595458984375,
			"height": 200,
			"seed": 1643923645,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "The Time complexity will be O(n) due to the fact that \n    the time to complete will relate to the length of\nthe Linked list, into infinity.\n\nThe space complexity will be O(1) due to the fact that \nthe nodes will take up the same space for each node \ncreated.\n",
			"rawText": "The Time complexity will be O(n) due to the fact that \n    the time to complete will relate to the length of\nthe Linked list, into infinity.\n\nThe space complexity will be O(1) due to the fact that \nthe nodes will take up the same space for each node \ncreated.\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "The Time complexity will be O(n) due to the fact that \n    the time to complete will relate to the length of\nthe Linked list, into infinity.\n\nThe space complexity will be O(1) due to the fact that \nthe nodes will take up the same space for each node \ncreated.\n",
			"lineHeight": 1.25,
			"baseline": 193
		},
		{
			"type": "ellipse",
			"version": 173,
			"versionNonce": 2118367325,
			"isDeleted": false,
			"id": "RQMZMdiyK4OGm4BTVbOgn",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -536.1702270507812,
			"y": -1710.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 103,
			"height": 63,
			"seed": 1917201427,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "qdNLs9dm"
				},
				{
					"id": "hcqjVM0hQKlaYY-qT7zCr",
					"type": "arrow"
				}
			],
			"updated": 1682458359845,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 152,
			"versionNonce": 1127761907,
			"isDeleted": false,
			"id": "qdNLs9dm",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -487.2962253663611,
			"y": -1691.7582386073761,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 5.4199981689453125,
			"height": 25,
			"seed": 176335315,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "1",
			"rawText": "1",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "RQMZMdiyK4OGm4BTVbOgn",
			"originalText": "1",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "ellipse",
			"version": 274,
			"versionNonce": 1632019645,
			"isDeleted": false,
			"id": "AmBkWNzJAFMDvYz_KFFXd",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -283.17022705078125,
			"y": -1711.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 181,
			"height": 64,
			"seed": 328928957,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "ELs5BNO2"
				},
				{
					"id": "A77RKqMlmn53DPqOnC0KP",
					"type": "arrow"
				},
				{
					"id": "hcqjVM0hQKlaYY-qT7zCr",
					"type": "arrow"
				},
				{
					"id": "Hkh5dXyoVYRka9Ehl3Q94",
					"type": "arrow"
				}
			],
			"updated": 1682458359845,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 224,
			"versionNonce": 930140563,
			"isDeleted": false,
			"id": "ELs5BNO2",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -199.7833858653513,
			"y": -1692.6117919979695,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 14.239990234375,
			"height": 25,
			"seed": 255410685,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2",
			"rawText": "2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "AmBkWNzJAFMDvYz_KFFXd",
			"originalText": "2",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "ellipse",
			"version": 262,
			"versionNonce": 1374487837,
			"isDeleted": false,
			"id": "T5CtXQPq4eMYgagMVkXFn",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 98.82977294921875,
			"y": -1713.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 99,
			"height": 63,
			"seed": 880063539,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "JmHTDAwY"
				},
				{
					"id": "WcGVrNizEhms4XSo5HFRf",
					"type": "arrow"
				},
				{
					"id": "A77RKqMlmn53DPqOnC0KP",
					"type": "arrow"
				}
			],
			"updated": 1682458359845,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 231,
			"versionNonce": 1395074867,
			"isDeleted": false,
			"id": "JmHTDAwY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 141.5179897218909,
			"y": -1694.7582386073761,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 13.6199951171875,
			"height": 25,
			"seed": 1185842483,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "3",
			"rawText": "3",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "T5CtXQPq4eMYgagMVkXFn",
			"originalText": "3",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "ellipse",
			"version": 256,
			"versionNonce": 866670973,
			"isDeleted": false,
			"id": "saXgJ3NCiVw5gNknu_kw-",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 383.82977294921875,
			"y": -1720.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 139,
			"height": 81,
			"seed": 503251581,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "2lel1EqP"
				},
				{
					"id": "WcGVrNizEhms4XSo5HFRf",
					"type": "arrow"
				}
			],
			"updated": 1682458359845,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 228,
			"versionNonce": 2093074643,
			"isDeleted": false,
			"id": "2lel1EqP",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 446.7858577602693,
			"y": -1693.1221996380552,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 12.79998779296875,
			"height": 25,
			"seed": 397660317,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "4",
			"rawText": "4",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "saXgJ3NCiVw5gNknu_kw-",
			"originalText": "4",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 572,
			"versionNonce": 1820860765,
			"isDeleted": false,
			"id": "hcqjVM0hQKlaYY-qT7zCr",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -431.1763361090604,
			"y": -1680.1887242863868,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 141.01115492109312,
			"height": 0.5746288012746845,
			"seed": 506708723,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682458381660,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "RQMZMdiyK4OGm4BTVbOgn",
				"gap": 2.0057147273482983,
				"focus": -0.029279986926655198
			},
			"endBinding": {
				"elementId": "AmBkWNzJAFMDvYz_KFFXd",
				"gap": 6.999348806168356,
				"focus": -0.023985195399719883
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					141.01115492109312,
					0.5746288012746845
				]
			]
		},
		{
			"type": "arrow",
			"version": 711,
			"versionNonce": 955867773,
			"isDeleted": false,
			"id": "A77RKqMlmn53DPqOnC0KP",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -97.17474633904219,
			"y": -1679.0363384515313,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 194.00319379316835,
			"height": 5.906285084849969,
			"seed": 564113587,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": null,
			"updated": 1682458381661,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "AmBkWNzJAFMDvYz_KFFXd",
				"gap": 5.026798008462009,
				"focus": 0.12003485048922753
			},
			"endBinding": {
				"elementId": "T5CtXQPq4eMYgagMVkXFn",
				"gap": 2.139391703779225,
				"focus": 0.1276688597192888
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					194.00319379316835,
					-5.906285084849969
				]
			]
		},
		{
			"type": "arrow",
			"version": 706,
			"versionNonce": 671222493,
			"isDeleted": false,
			"id": "WcGVrNizEhms4XSo5HFRf",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 199.76147894565827,
			"y": -1680.2169883366446,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 174.11068135802134,
			"height": 1.9495137981862172,
			"seed": 1901230397,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": null,
			"updated": 1682458381662,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "T5CtXQPq4eMYgagMVkXFn",
				"gap": 2.0495667267392363,
				"focus": 0.09024845764259272
			},
			"endBinding": {
				"elementId": "saXgJ3NCiVw5gNknu_kw-",
				"gap": 10.001726220683878,
				"focus": 0.06348982224979105
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					174.11068135802134,
					-1.9495137981862172
				]
			]
		},
		{
			"type": "text",
			"version": 219,
			"versionNonce": 1496182803,
			"isDeleted": false,
			"id": "67mQuzfH",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -50.17022705078125,
			"y": -1881.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 116.47991943359375,
			"height": 25,
			"seed": 1616547571,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "INPUT(3,8)",
			"rawText": "INPUT(3,8)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "INPUT(3,8)",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "ellipse",
			"version": 224,
			"versionNonce": 217517725,
			"isDeleted": false,
			"id": "jZCC1d50-yijAZ8sUcz4D",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -36.17022705078125,
			"y": -1848.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 91,
			"height": 79,
			"seed": 937698269,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "MBFClbng"
				},
				{
					"id": "bnvqXv1RpqpPBuNnR-D9w",
					"type": "arrow"
				},
				{
					"id": "Hkh5dXyoVYRka9Ehl3Q94",
					"type": "arrow"
				}
			],
			"updated": 1682458359845,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 174,
			"versionNonce": 750548403,
			"isDeleted": false,
			"id": "MBFClbng",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 1.5064205087464586,
			"y": -1821.9150928568686,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 15.29998779296875,
			"height": 25,
			"seed": 1675995827,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "8",
			"rawText": "8",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "jZCC1d50-yijAZ8sUcz4D",
			"originalText": "8",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 351,
			"versionNonce": 1495162227,
			"isDeleted": false,
			"id": "bnvqXv1RpqpPBuNnR-D9w",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 35.826978473672845,
			"y": -1774.9873225974936,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 73.0027944755459,
			"height": 77.00294759749363,
			"seed": 1305434067,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": null,
			"updated": 1682458381662,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "jZCC1d50-yijAZ8sUcz4D",
				"gap": 2.0467233479171085,
				"focus": 0.10534389660672411
			},
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					73.0027944755459,
					77.00294759749363
				]
			]
		},
		{
			"type": "arrow",
			"version": 527,
			"versionNonce": 586692371,
			"isDeleted": false,
			"id": "Hkh5dXyoVYRka9Ehl3Q94",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -115.5188402296336,
			"y": -1700.674070961681,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 91.02276498897582,
			"height": 81.02026334183552,
			"seed": 612741363,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": null,
			"updated": 1682458381662,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "AmBkWNzJAFMDvYz_KFFXd",
				"gap": 3.9026906455344204,
				"focus": 0.5535827023708164
			},
			"endBinding": {
				"elementId": "jZCC1d50-yijAZ8sUcz4D",
				"gap": 1,
				"focus": 0.04098568021505496
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					91.02276498897582,
					-81.02026334183552
				]
			]
		},
		{
			"type": "freedraw",
			"version": 184,
			"versionNonce": 468699997,
			"isDeleted": false,
			"id": "V8RowK-3Q3FPfiLpgVEF2",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 16.82977294921875,
			"y": -1708.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 34,
			"height": 56,
			"seed": 1448850195,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					-1,
					3
				],
				[
					-5,
					9
				],
				[
					-10,
					18
				],
				[
					-17,
					28
				],
				[
					-23,
					36
				],
				[
					-26,
					42
				],
				[
					-29,
					48
				],
				[
					-32,
					52
				],
				[
					-33,
					55
				],
				[
					-34,
					56
				],
				[
					-34,
					56
				]
			],
			"lastCommittedPoint": [
				-34,
				56
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 191,
			"versionNonce": 877323507,
			"isDeleted": false,
			"id": "4LiJlQkleGfVEjfZh8QnW",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -27.17022705078125,
			"y": -1715.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 67,
			"height": 74,
			"seed": 604665459,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					5,
					3
				],
				[
					9,
					7
				],
				[
					15,
					13
				],
				[
					23,
					20
				],
				[
					28,
					26
				],
				[
					34,
					32
				],
				[
					38,
					38
				],
				[
					43,
					44
				],
				[
					47,
					50
				],
				[
					51,
					56
				],
				[
					55,
					59
				],
				[
					57,
					62
				],
				[
					58,
					64
				],
				[
					60,
					66
				],
				[
					62,
					69
				],
				[
					64,
					73
				],
				[
					67,
					74
				],
				[
					67,
					74
				]
			],
			"lastCommittedPoint": [
				67,
				74
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 184,
			"versionNonce": 905467837,
			"isDeleted": false,
			"id": "D6waXs4I",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -363.17022705078125,
			"y": -1812.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 137.75987243652344,
			"height": 25,
			"seed": 703948285,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Insert Before",
			"rawText": "Insert Before",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Insert Before",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "freedraw",
			"version": 191,
			"versionNonce": 103272083,
			"isDeleted": false,
			"id": "s9pTSr5ow8dOF_Mn09k6b",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -96.17022705078125,
			"y": -1963.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 43,
			"height": 53,
			"seed": 262434739,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					2
				],
				[
					0,
					3
				],
				[
					0,
					10
				],
				[
					2,
					20
				],
				[
					4,
					30
				],
				[
					7,
					40
				],
				[
					11,
					49
				],
				[
					13,
					53
				],
				[
					14,
					53
				],
				[
					19,
					46
				],
				[
					26,
					35
				],
				[
					33,
					25
				],
				[
					38,
					17
				],
				[
					41,
					11
				],
				[
					43,
					7
				],
				[
					43,
					6
				],
				[
					43,
					5
				],
				[
					43,
					5
				]
			],
			"lastCommittedPoint": [
				43,
				5
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 180,
			"versionNonce": 737171485,
			"isDeleted": false,
			"id": "FgBEql8LVK7jUUDzAyL42",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -21.17022705078125,
			"y": -1924.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 2,
			"height": 14,
			"seed": 641478845,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					2
				],
				[
					1,
					5
				],
				[
					1,
					8
				],
				[
					1,
					11
				],
				[
					1,
					13
				],
				[
					2,
					14
				],
				[
					2,
					14
				]
			],
			"lastCommittedPoint": [
				2,
				14
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 173,
			"versionNonce": 200705075,
			"isDeleted": false,
			"id": "cor-a3dECm2MuoLPZODqX",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -23.17022705078125,
			"y": -1958.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 1257577117,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": [
				0.0001,
				0.0001
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 194,
			"versionNonce": 935939197,
			"isDeleted": false,
			"id": "tH17ModYfeYcJ_MWrqn_H",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 21.82977294921875,
			"y": -1960.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 28,
			"height": 46,
			"seed": 606829395,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3,
					1
				],
				[
					-9,
					4
				],
				[
					-15,
					8
				],
				[
					-18,
					11
				],
				[
					-19,
					13
				],
				[
					-19,
					15
				],
				[
					-19,
					17
				],
				[
					-15,
					20
				],
				[
					-10,
					23
				],
				[
					-4,
					26
				],
				[
					1,
					30
				],
				[
					5,
					34
				],
				[
					8,
					37
				],
				[
					9,
					40
				],
				[
					9,
					41
				],
				[
					9,
					42
				],
				[
					6,
					43
				],
				[
					3,
					44
				],
				[
					-1,
					45
				],
				[
					-2,
					46
				],
				[
					-3,
					46
				],
				[
					-3,
					46
				]
			],
			"lastCommittedPoint": [
				-3,
				46
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 190,
			"versionNonce": 2107475411,
			"isDeleted": false,
			"id": "bdTJ3u5xncnzqCKoDfd0V",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 61.82977294921875,
			"y": -1939.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 37,
			"height": 31,
			"seed": 444626643,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					0
				],
				[
					-1,
					1
				],
				[
					-1,
					5
				],
				[
					-1,
					10
				],
				[
					0,
					15
				],
				[
					4,
					20
				],
				[
					8,
					22
				],
				[
					13,
					24
				],
				[
					18,
					25
				],
				[
					22,
					25
				],
				[
					26,
					22
				],
				[
					30,
					18
				],
				[
					33,
					12
				],
				[
					35,
					4
				],
				[
					35,
					-2
				],
				[
					35,
					-5
				],
				[
					36,
					-6
				],
				[
					36,
					-6
				]
			],
			"lastCommittedPoint": [
				36,
				-6
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 205,
			"versionNonce": 1497674973,
			"isDeleted": false,
			"id": "1Gwsed4jzZiLRdjra1TrP",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 134.82977294921875,
			"y": -1933.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 55,
			"height": 21,
			"seed": 2111544083,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					1,
					2
				],
				[
					1,
					4
				],
				[
					-2,
					6
				],
				[
					-4,
					8
				],
				[
					-7,
					9
				],
				[
					-9,
					10
				],
				[
					-11,
					10
				],
				[
					-12,
					10
				],
				[
					-15,
					9
				],
				[
					-18,
					7
				],
				[
					-20,
					4
				],
				[
					-20,
					1
				],
				[
					-19,
					-1
				],
				[
					-15,
					-4
				],
				[
					-8,
					-6
				],
				[
					0,
					-6
				],
				[
					5,
					-5
				],
				[
					8,
					-3
				],
				[
					10,
					-1
				],
				[
					11,
					2
				],
				[
					11,
					5
				],
				[
					11,
					7
				],
				[
					11,
					9
				],
				[
					11,
					11
				],
				[
					11,
					14
				],
				[
					12,
					14
				],
				[
					16,
					15
				],
				[
					21,
					15
				],
				[
					27,
					14
				],
				[
					33,
					12
				],
				[
					35,
					11
				],
				[
					35,
					11
				]
			],
			"lastCommittedPoint": [
				35,
				11
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 182,
			"versionNonce": 1379095411,
			"isDeleted": false,
			"id": "kYmKmTGceSR5FmZhsZssJ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 171.82977294921875,
			"y": -1950.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 3,
			"height": 41,
			"seed": 612695549,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					2
				],
				[
					0,
					8
				],
				[
					0,
					15
				],
				[
					0,
					24
				],
				[
					1,
					32
				],
				[
					2,
					39
				],
				[
					2,
					41
				],
				[
					3,
					41
				],
				[
					3,
					41
				]
			],
			"lastCommittedPoint": [
				3,
				41
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 117,
			"versionNonce": 468980029,
			"isDeleted": false,
			"id": "HhTc3SbARDFnOyORXZPSk",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -478.17022705078125,
			"y": -1505.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 48,
			"height": 82,
			"seed": 855304627,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					-1
				],
				[
					2,
					-4
				],
				[
					4,
					-9
				],
				[
					6,
					-15
				],
				[
					9,
					-23
				],
				[
					12,
					-31
				],
				[
					14,
					-39
				],
				[
					15,
					-45
				],
				[
					17,
					-51
				],
				[
					19,
					-58
				],
				[
					20,
					-66
				],
				[
					21,
					-73
				],
				[
					22,
					-78
				],
				[
					23,
					-81
				],
				[
					23,
					-82
				],
				[
					26,
					-81
				],
				[
					29,
					-75
				],
				[
					31,
					-68
				],
				[
					32,
					-58
				],
				[
					33,
					-48
				],
				[
					35,
					-38
				],
				[
					39,
					-29
				],
				[
					43,
					-21
				],
				[
					44,
					-16
				],
				[
					46,
					-13
				],
				[
					47,
					-11
				],
				[
					48,
					-9
				],
				[
					48,
					-8
				],
				[
					48,
					-8
				]
			],
			"lastCommittedPoint": [
				48,
				-8
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 100,
			"versionNonce": 1509846291,
			"isDeleted": false,
			"id": "JmtNlzpSlGD8b2cCticoZ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -466.17022705078125,
			"y": -1545.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 30,
			"height": 2,
			"seed": 261882013,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					5,
					0
				],
				[
					10,
					0
				],
				[
					15,
					1
				],
				[
					18,
					1
				],
				[
					21,
					1
				],
				[
					22,
					1
				],
				[
					23,
					1
				],
				[
					25,
					2
				],
				[
					28,
					2
				],
				[
					30,
					2
				],
				[
					30,
					2
				]
			],
			"lastCommittedPoint": [
				30,
				2
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 99,
			"versionNonce": 490267037,
			"isDeleted": false,
			"id": "pGwy93i7US3FcIMi0O8bv",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -406.17022705078125,
			"y": -1576.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 7,
			"height": 60,
			"seed": 687686461,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2
				],
				[
					1,
					7
				],
				[
					2,
					14
				],
				[
					2,
					22
				],
				[
					3,
					31
				],
				[
					4,
					39
				],
				[
					4,
					47
				],
				[
					6,
					54
				],
				[
					6,
					59
				],
				[
					7,
					60
				],
				[
					7,
					60
				]
			],
			"lastCommittedPoint": [
				7,
				60
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 129,
			"versionNonce": 410342067,
			"isDeleted": false,
			"id": "TpvbFMJe3tJ_xHIUjuMtz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -337.17022705078125,
			"y": -1569.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 41,
			"height": 53,
			"seed": 947695827,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2,
					-1
				],
				[
					-4,
					-1
				],
				[
					-7,
					-1
				],
				[
					-11,
					-1
				],
				[
					-17,
					0
				],
				[
					-23,
					2
				],
				[
					-28,
					4
				],
				[
					-32,
					8
				],
				[
					-36,
					14
				],
				[
					-39,
					19
				],
				[
					-41,
					25
				],
				[
					-41,
					31
				],
				[
					-41,
					36
				],
				[
					-41,
					41
				],
				[
					-39,
					45
				],
				[
					-37,
					48
				],
				[
					-34,
					50
				],
				[
					-32,
					52
				],
				[
					-29,
					52
				],
				[
					-27,
					52
				],
				[
					-25,
					52
				],
				[
					-21,
					52
				],
				[
					-17,
					50
				],
				[
					-13,
					49
				],
				[
					-11,
					48
				],
				[
					-9,
					45
				],
				[
					-9,
					43
				],
				[
					-9,
					40
				],
				[
					-9,
					36
				],
				[
					-9,
					34
				],
				[
					-10,
					32
				],
				[
					-11,
					30
				],
				[
					-12,
					29
				],
				[
					-13,
					29
				],
				[
					-14,
					29
				],
				[
					-16,
					29
				],
				[
					-19,
					29
				],
				[
					-22,
					29
				],
				[
					-25,
					29
				],
				[
					-27,
					29
				],
				[
					-27,
					29
				]
			],
			"lastCommittedPoint": [
				-27,
				29
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 122,
			"versionNonce": 1380230653,
			"isDeleted": false,
			"id": "wkvkrwfCfTNcpjtuTe1t0",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -287.17022705078125,
			"y": -1525.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 39,
			"height": 38,
			"seed": 281761213,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					-1,
					3
				],
				[
					-3,
					5
				],
				[
					-7,
					6
				],
				[
					-11,
					7
				],
				[
					-15,
					7
				],
				[
					-19,
					7
				],
				[
					-22,
					5
				],
				[
					-27,
					2
				],
				[
					-31,
					-2
				],
				[
					-33,
					-5
				],
				[
					-35,
					-9
				],
				[
					-35,
					-15
				],
				[
					-35,
					-18
				],
				[
					-35,
					-21
				],
				[
					-32,
					-24
				],
				[
					-29,
					-26
				],
				[
					-24,
					-27
				],
				[
					-19,
					-27
				],
				[
					-15,
					-27
				],
				[
					-10,
					-26
				],
				[
					-4,
					-23
				],
				[
					0,
					-20
				],
				[
					2,
					-18
				],
				[
					3,
					-16
				],
				[
					4,
					-14
				],
				[
					4,
					-10
				],
				[
					4,
					-6
				],
				[
					2,
					-2
				],
				[
					0,
					3
				],
				[
					-3,
					7
				],
				[
					-4,
					10
				],
				[
					-5,
					11
				],
				[
					-5,
					11
				]
			],
			"lastCommittedPoint": [
				-5,
				11
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 128,
			"versionNonce": 1581155411,
			"isDeleted": false,
			"id": "3_FMQCpXtaTQU9-JsP5gc",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -526.1702270507812,
			"y": -1495.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 302,
			"height": 4,
			"seed": 1859235965,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2,
					0
				],
				[
					8,
					0
				],
				[
					16,
					0
				],
				[
					28,
					0
				],
				[
					45,
					0
				],
				[
					63,
					1
				],
				[
					80,
					2
				],
				[
					97,
					4
				],
				[
					111,
					4
				],
				[
					122,
					4
				],
				[
					136,
					4
				],
				[
					144,
					4
				],
				[
					154,
					4
				],
				[
					164,
					4
				],
				[
					174,
					4
				],
				[
					185,
					4
				],
				[
					196,
					4
				],
				[
					206,
					4
				],
				[
					218,
					4
				],
				[
					230,
					3
				],
				[
					243,
					3
				],
				[
					254,
					2
				],
				[
					264,
					1
				],
				[
					270,
					1
				],
				[
					275,
					1
				],
				[
					279,
					1
				],
				[
					282,
					1
				],
				[
					284,
					1
				],
				[
					285,
					0
				],
				[
					286,
					0
				],
				[
					287,
					0
				],
				[
					288,
					0
				],
				[
					290,
					0
				],
				[
					292,
					0
				],
				[
					294,
					0
				],
				[
					297,
					0
				],
				[
					299,
					0
				],
				[
					301,
					0
				],
				[
					302,
					0
				],
				[
					302,
					0
				]
			],
			"lastCommittedPoint": [
				302,
				0
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 112,
			"versionNonce": 236510813,
			"isDeleted": false,
			"id": "5VSemB2zLCiiXuwPar0OO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -378.17022705078125,
			"y": -1786.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 168,
			"height": 9,
			"seed": 202976019,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					6,
					0
				],
				[
					17,
					1
				],
				[
					25,
					2
				],
				[
					39,
					3
				],
				[
					54,
					3
				],
				[
					71,
					3
				],
				[
					86,
					3
				],
				[
					97,
					3
				],
				[
					107,
					3
				],
				[
					115,
					4
				],
				[
					123,
					5
				],
				[
					128,
					7
				],
				[
					135,
					7
				],
				[
					141,
					8
				],
				[
					148,
					9
				],
				[
					155,
					9
				],
				[
					160,
					9
				],
				[
					164,
					9
				],
				[
					165,
					9
				],
				[
					166,
					9
				],
				[
					167,
					9
				],
				[
					168,
					9
				],
				[
					168,
					9
				]
			],
			"lastCommittedPoint": [
				168,
				9
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 572,
			"versionNonce": 590381555,
			"isDeleted": false,
			"id": "xYwU66HG",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -513.1702270507812,
			"y": -1468.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 590.719482421875,
			"height": 200,
			"seed": 1050950131,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "1. Check to see if Linked list is null\n2. check to see if the first value of the input is null \n3. create temp node & create prevTemp node\n5. assign temp node to list.head\n6. use while loop to loop through linked list \n7. set truthy statement for while top to temp != null\n8. the temp needs to be one ahead then the previous temp\n9. when temp hits the value after ",
			"rawText": "1. Check to see if Linked list is null\n2. check to see if the first value of the input is null \n3. create temp node & create prevTemp node\n5. assign temp node to list.head\n6. use while loop to loop through linked list \n7. set truthy statement for while top to temp != null\n8. the temp needs to be one ahead then the previous temp\n9. when temp hits the value after ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "1. Check to see if Linked list is null\n2. check to see if the first value of the input is null \n3. create temp node & create prevTemp node\n5. assign temp node to list.head\n6. use while loop to loop through linked list \n7. set truthy statement for while top to temp != null\n8. the temp needs to be one ahead then the previous temp\n9. when temp hits the value after ",
			"lineHeight": 1.25,
			"baseline": 193
		},
		{
			"type": "freedraw",
			"version": 98,
			"versionNonce": 1200032445,
			"isDeleted": false,
			"id": "hNlpn7p2BlPaxvXdtgqPP",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 115.82977294921875,
			"y": -1642.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 3,
			"height": 30,
			"seed": 1907107475,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2
				],
				[
					0,
					5
				],
				[
					-1,
					9
				],
				[
					-1,
					13
				],
				[
					-2,
					18
				],
				[
					-3,
					23
				],
				[
					-3,
					26
				],
				[
					-3,
					27
				],
				[
					-3,
					29
				],
				[
					-3,
					30
				],
				[
					-3,
					30
				]
			],
			"lastCommittedPoint": [
				-3,
				30
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 100,
			"versionNonce": 542231443,
			"isDeleted": false,
			"id": "0-XbQ4iFeKV1vdO2jSPh3",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 99.82977294921875,
			"y": -1641.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 33,
			"height": 2,
			"seed": 463996509,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					3,
					0
				],
				[
					7,
					0
				],
				[
					13,
					0
				],
				[
					19,
					-1
				],
				[
					23,
					-1
				],
				[
					26,
					-2
				],
				[
					27,
					-2
				],
				[
					28,
					-2
				],
				[
					31,
					-2
				],
				[
					32,
					-2
				],
				[
					33,
					-2
				],
				[
					33,
					-2
				]
			],
			"lastCommittedPoint": [
				33,
				-2
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 130,
			"versionNonce": 523283229,
			"isDeleted": false,
			"id": "I_WGOkwc-SG-Hkm0jqDnf",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 130.82977294921875,
			"y": -1631.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 26,
			"height": 23,
			"seed": 177281363,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					3,
					0
				],
				[
					6,
					-1
				],
				[
					10,
					-1
				],
				[
					14,
					-2
				],
				[
					17,
					-3
				],
				[
					19,
					-4
				],
				[
					20,
					-5
				],
				[
					21,
					-7
				],
				[
					21,
					-9
				],
				[
					21,
					-10
				],
				[
					20,
					-10
				],
				[
					18,
					-7
				],
				[
					17,
					-6
				],
				[
					15,
					-5
				],
				[
					15,
					-4
				],
				[
					14,
					-4
				],
				[
					14,
					-3
				],
				[
					13,
					-3
				],
				[
					12,
					-3
				],
				[
					11,
					-3
				],
				[
					10,
					-3
				],
				[
					9,
					-3
				],
				[
					8,
					-3
				],
				[
					8,
					-2
				],
				[
					7,
					-1
				],
				[
					6,
					1
				],
				[
					6,
					2
				],
				[
					6,
					5
				],
				[
					7,
					6
				],
				[
					8,
					7
				],
				[
					9,
					9
				],
				[
					11,
					10
				],
				[
					13,
					11
				],
				[
					15,
					12
				],
				[
					17,
					12
				],
				[
					18,
					13
				],
				[
					21,
					13
				],
				[
					22,
					13
				],
				[
					24,
					13
				],
				[
					25,
					13
				],
				[
					26,
					12
				],
				[
					26,
					12
				]
			],
			"lastCommittedPoint": [
				26,
				12
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 122,
			"versionNonce": 702079283,
			"isDeleted": false,
			"id": "u_E2Ze-GZtrywCnhNQz_Z",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 163.82977294921875,
			"y": -1633.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 18,
			"height": 22,
			"seed": 2092651933,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					5
				],
				[
					0,
					8
				],
				[
					0,
					12
				],
				[
					0,
					14
				],
				[
					0,
					15
				],
				[
					0,
					12
				],
				[
					0,
					6
				],
				[
					0,
					1
				],
				[
					2,
					-3
				],
				[
					4,
					-4
				],
				[
					6,
					-6
				],
				[
					7,
					-6
				],
				[
					9,
					-4
				],
				[
					10,
					-1
				],
				[
					11,
					1
				],
				[
					11,
					4
				],
				[
					11,
					7
				],
				[
					11,
					9
				],
				[
					11,
					10
				],
				[
					11,
					9
				],
				[
					11,
					6
				],
				[
					12,
					3
				],
				[
					14,
					1
				],
				[
					15,
					0
				],
				[
					16,
					0
				],
				[
					17,
					0
				],
				[
					17,
					1
				],
				[
					18,
					3
				],
				[
					18,
					6
				],
				[
					18,
					9
				],
				[
					18,
					12
				],
				[
					18,
					14
				],
				[
					18,
					16
				],
				[
					18,
					16
				]
			],
			"lastCommittedPoint": [
				18,
				16
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 94,
			"versionNonce": 629620605,
			"isDeleted": false,
			"id": "CRW1ac5tEoU99sExcyGwX",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 192.82977294921875,
			"y": -1637.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 2,
			"height": 21,
			"seed": 1781041139,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					4
				],
				[
					0,
					8
				],
				[
					-1,
					13
				],
				[
					-2,
					16
				],
				[
					-2,
					19
				],
				[
					-2,
					21
				],
				[
					-2,
					21
				]
			],
			"lastCommittedPoint": [
				-2,
				21
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 108,
			"versionNonce": 1227637459,
			"isDeleted": false,
			"id": "we8gw-q00Dam-TbjTDQDv",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 189.82977294921875,
			"y": -1639.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 14,
			"height": 12,
			"seed": 579313213,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1
				],
				[
					2,
					-1
				],
				[
					3,
					-1
				],
				[
					4,
					-1
				],
				[
					6,
					-1
				],
				[
					7,
					-1
				],
				[
					8,
					-1
				],
				[
					11,
					0
				],
				[
					12,
					2
				],
				[
					13,
					3
				],
				[
					14,
					5
				],
				[
					14,
					7
				],
				[
					13,
					8
				],
				[
					10,
					9
				],
				[
					8,
					9
				],
				[
					6,
					10
				],
				[
					5,
					11
				],
				[
					4,
					11
				],
				[
					3,
					11
				],
				[
					2,
					11
				],
				[
					2,
					11
				]
			],
			"lastCommittedPoint": [
				2,
				11
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 95,
			"versionNonce": 1624000477,
			"isDeleted": false,
			"id": "WWSlbTCFIuOrx1ZpbMgNv",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -270.17022705078125,
			"y": -1642.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 8,
			"height": 22,
			"seed": 1101054451,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					4,
					2
				],
				[
					6,
					6
				],
				[
					7,
					10
				],
				[
					8,
					15
				],
				[
					8,
					19
				],
				[
					8,
					22
				],
				[
					8,
					22
				]
			],
			"lastCommittedPoint": [
				8,
				22
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 103,
			"versionNonce": 383938675,
			"isDeleted": false,
			"id": "Uij-gpLXgrhr2DumDf43c",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -264.17022705078125,
			"y": -1652.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 19,
			"height": 11,
			"seed": 621423123,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					5,
					0
				],
				[
					10,
					0
				],
				[
					13,
					1
				],
				[
					15,
					2
				],
				[
					17,
					3
				],
				[
					18,
					4
				],
				[
					19,
					5
				],
				[
					19,
					6
				],
				[
					19,
					7
				],
				[
					18,
					8
				],
				[
					15,
					10
				],
				[
					12,
					10
				],
				[
					10,
					11
				],
				[
					8,
					11
				],
				[
					8,
					11
				]
			],
			"lastCommittedPoint": [
				8,
				11
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 102,
			"versionNonce": 319898685,
			"isDeleted": false,
			"id": "sEIv4cxNVAh30jb0Sx1-m",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -241.17022705078125,
			"y": -1620.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 9,
			"height": 23,
			"seed": 1621118131,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					1,
					2
				],
				[
					1,
					1
				],
				[
					1,
					-2
				],
				[
					1,
					-9
				],
				[
					1,
					-15
				],
				[
					1,
					-19
				],
				[
					2,
					-21
				],
				[
					3,
					-21
				],
				[
					4,
					-21
				],
				[
					5,
					-21
				],
				[
					6,
					-21
				],
				[
					7,
					-21
				],
				[
					9,
					-21
				],
				[
					9,
					-21
				]
			],
			"lastCommittedPoint": [
				9,
				-21
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 114,
			"versionNonce": 1421994515,
			"isDeleted": false,
			"id": "q4rIitQ4LAA7VMY2Nr7wC",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -230.17022705078125,
			"y": -1635.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 8,
			"height": 23,
			"seed": 50642685,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2,
					1
				],
				[
					4,
					1
				],
				[
					5,
					1
				],
				[
					6,
					1
				],
				[
					7,
					1
				],
				[
					7,
					0
				],
				[
					7,
					-1
				],
				[
					6,
					-3
				],
				[
					6,
					-4
				],
				[
					5,
					-4
				],
				[
					4,
					-4
				],
				[
					3,
					-3
				],
				[
					2,
					-2
				],
				[
					1,
					1
				],
				[
					1,
					5
				],
				[
					1,
					9
				],
				[
					1,
					12
				],
				[
					1,
					15
				],
				[
					1,
					16
				],
				[
					1,
					18
				],
				[
					2,
					19
				],
				[
					3,
					19
				],
				[
					4,
					19
				],
				[
					5,
					19
				],
				[
					7,
					19
				],
				[
					8,
					19
				],
				[
					8,
					19
				]
			],
			"lastCommittedPoint": [
				8,
				19
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 108,
			"versionNonce": 1077392541,
			"isDeleted": false,
			"id": "tTcA01A2j3C1WIa_NwpR3",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -214.17022705078125,
			"y": -1631.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 25,
			"height": 26,
			"seed": 647372307,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					1,
					1
				],
				[
					2,
					4
				],
				[
					3,
					8
				],
				[
					6,
					12
				],
				[
					12,
					17
				],
				[
					18,
					20
				],
				[
					22,
					23
				],
				[
					23,
					24
				],
				[
					24,
					24
				],
				[
					24,
					22
				],
				[
					24,
					19
				],
				[
					25,
					15
				],
				[
					25,
					12
				],
				[
					25,
					9
				],
				[
					25,
					6
				],
				[
					25,
					4
				],
				[
					25,
					2
				],
				[
					25,
					-1
				],
				[
					24,
					-2
				],
				[
					24,
					-2
				]
			],
			"lastCommittedPoint": [
				24,
				-2
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 95,
			"versionNonce": 1203842995,
			"isDeleted": false,
			"id": "02VXiZuceyclLG57WvK_e",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -155.17022705078125,
			"y": -1640.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 3,
			"height": 26,
			"seed": 137624765,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					-1,
					4
				],
				[
					-2,
					9
				],
				[
					-2,
					14
				],
				[
					-3,
					19
				],
				[
					-3,
					24
				],
				[
					-3,
					26
				],
				[
					-3,
					26
				]
			],
			"lastCommittedPoint": [
				-3,
				26
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 96,
			"versionNonce": 1945180413,
			"isDeleted": false,
			"id": "VC4EFywIjvUdpE1yBOVZG",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -172.17022705078125,
			"y": -1637.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 38,
			"height": 0,
			"seed": 2089641629,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					6,
					0
				],
				[
					12,
					0
				],
				[
					21,
					0
				],
				[
					29,
					0
				],
				[
					35,
					0
				],
				[
					37,
					0
				],
				[
					38,
					0
				],
				[
					38,
					0
				]
			],
			"lastCommittedPoint": [
				38,
				0
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 118,
			"versionNonce": 1376174419,
			"isDeleted": false,
			"id": "l8dmL9t31q1cVBN8WGB4d",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -134.17022705078125,
			"y": -1625.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 13,
			"height": 25,
			"seed": 222277075,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3,
					0
				],
				[
					4,
					0
				],
				[
					5,
					0
				],
				[
					6,
					-1
				],
				[
					6,
					-3
				],
				[
					6,
					-5
				],
				[
					6,
					-7
				],
				[
					5,
					-9
				],
				[
					4,
					-10
				],
				[
					3,
					-10
				],
				[
					2,
					-10
				],
				[
					1,
					-9
				],
				[
					0,
					-7
				],
				[
					-2,
					-4
				],
				[
					-3,
					-1
				],
				[
					-5,
					2
				],
				[
					-5,
					4
				],
				[
					-7,
					7
				],
				[
					-7,
					8
				],
				[
					-7,
					10
				],
				[
					-7,
					11
				],
				[
					-6,
					12
				],
				[
					-5,
					13
				],
				[
					-3,
					14
				],
				[
					-1,
					15
				],
				[
					0,
					15
				],
				[
					2,
					15
				],
				[
					3,
					15
				],
				[
					4,
					15
				],
				[
					4,
					14
				],
				[
					4,
					14
				]
			],
			"lastCommittedPoint": [
				4,
				14
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 122,
			"versionNonce": 1203695965,
			"isDeleted": false,
			"id": "isjo3dAH8l0Wnvpu-GuHU",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -122.17022705078125,
			"y": -1624.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 17,
			"height": 21,
			"seed": 982856413,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					1,
					1
				],
				[
					1,
					3
				],
				[
					1,
					7
				],
				[
					1,
					10
				],
				[
					1,
					12
				],
				[
					1,
					13
				],
				[
					1,
					12
				],
				[
					1,
					10
				],
				[
					3,
					6
				],
				[
					4,
					1
				],
				[
					6,
					-2
				],
				[
					7,
					-4
				],
				[
					8,
					-4
				],
				[
					8,
					-2
				],
				[
					9,
					2
				],
				[
					9,
					5
				],
				[
					9,
					7
				],
				[
					9,
					8
				],
				[
					9,
					7
				],
				[
					9,
					6
				],
				[
					9,
					0
				],
				[
					11,
					-4
				],
				[
					13,
					-6
				],
				[
					15,
					-8
				],
				[
					16,
					-8
				],
				[
					16,
					-6
				],
				[
					17,
					-4
				],
				[
					17,
					-1
				],
				[
					17,
					1
				],
				[
					17,
					3
				],
				[
					17,
					6
				],
				[
					17,
					8
				],
				[
					17,
					9
				],
				[
					17,
					9
				]
			],
			"lastCommittedPoint": [
				17,
				9
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 95,
			"versionNonce": 1290346227,
			"isDeleted": false,
			"id": "ia9mwuKI3XCs2KXI9P0Bc",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -92.17022705078125,
			"y": -1635.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 5,
			"height": 21,
			"seed": 1080684211,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2
				],
				[
					2,
					6
				],
				[
					3,
					10
				],
				[
					4,
					14
				],
				[
					4,
					18
				],
				[
					5,
					20
				],
				[
					5,
					21
				],
				[
					5,
					21
				]
			],
			"lastCommittedPoint": [
				5,
				21
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 106,
			"versionNonce": 686996925,
			"isDeleted": false,
			"id": "Pf8qu0lhHZxnq6eGUGE5M",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -88.17022705078125,
			"y": -1640.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 12,
			"seed": 1488936659,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					6,
					0
				],
				[
					10,
					0
				],
				[
					12,
					0
				],
				[
					14,
					1
				],
				[
					15,
					1
				],
				[
					16,
					2
				],
				[
					16,
					4
				],
				[
					16,
					6
				],
				[
					16,
					9
				],
				[
					14,
					10
				],
				[
					12,
					11
				],
				[
					11,
					12
				],
				[
					9,
					12
				],
				[
					6,
					12
				],
				[
					4,
					12
				],
				[
					3,
					12
				],
				[
					3,
					12
				]
			],
			"lastCommittedPoint": [
				3,
				12
			],
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 691,
			"versionNonce": 586074259,
			"isDeleted": false,
			"id": "GFr8aOXv",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -508.17022705078125,
			"y": -1216.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 612.259521484375,
			"height": 650,
			"seed": 1267583709,
			"groupIds": [],
			"roundness": null,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "public void insertBefore(int value, int newValue)\nthrow IllegalArgumentException{   \n if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n}\nNode temp = head;\nNode prevNode = null;\nNode newNode = new Node(newValue)\n\nif (temp.value == value){\n    newNode.next = temp;\n    head = newNode;\n    return;\n}\n\nwhile(temp.next != null){\nprevTemp = temp;\ntemp = temp.next;\nif(temp.value == value){\nnewNode.next = temp;\nprevTemp.next = newNode;\nreturn;\n}\n}\n\n}",
			"rawText": "public void insertBefore(int value, int newValue)\nthrow IllegalArgumentException{   \n if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n}\nNode temp = head;\nNode prevNode = null;\nNode newNode = new Node(newValue)\n\nif (temp.value == value){\n    newNode.next = temp;\n    head = newNode;\n    return;\n}\n\nwhile(temp.next != null){\nprevTemp = temp;\ntemp = temp.next;\nif(temp.value == value){\nnewNode.next = temp;\nprevTemp.next = newNode;\nreturn;\n}\n}\n\n}",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "public void insertBefore(int value, int newValue)\nthrow IllegalArgumentException{   \n if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n}\nNode temp = head;\nNode prevNode = null;\nNode newNode = new Node(newValue)\n\nif (temp.value == value){\n    newNode.next = temp;\n    head = newNode;\n    return;\n}\n\nwhile(temp.next != null){\nprevTemp = temp;\ntemp = temp.next;\nif(temp.value == value){\nnewNode.next = temp;\nprevTemp.next = newNode;\nreturn;\n}\n}\n\n}",
			"lineHeight": 1.25,
			"baseline": 643
		},
		{
			"type": "arrow",
			"version": 72,
			"versionNonce": 1588461085,
			"isDeleted": false,
			"id": "E-EyUxqDrm0T_ln0urJpk",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -262.17022705078125,
			"y": -930.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 131,
			"height": 37,
			"seed": 506307581,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "RTbc1zm9",
				"focus": 0.5506648896505036,
				"gap": 11
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					131,
					-37
				]
			]
		},
		{
			"id": "RTbc1zm9",
			"type": "text",
			"x": -188.17022705078125,
			"y": -1003.984375,
			"width": 732.5194091796875,
			"height": 25,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 918644531,
			"version": 248,
			"versionNonce": 701382195,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "E-EyUxqDrm0T_ln0urJpk",
					"type": "arrow"
				}
			],
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"text": "This is an edge case incase the value is the first node in the LinkedList.",
			"rawText": "This is an edge case incase the value is the first node in the LinkedList.",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "This is an edge case incase the value is the first node in the LinkedList.",
			"lineHeight": 1.25
		},
		{
			"id": "32yGixx14jsvkgXP2_ZtW",
			"type": "freedraw",
			"x": -212.17022705078125,
			"y": -3227.984375,
			"width": 35,
			"height": 49,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1291376787,
			"version": 25,
			"versionNonce": 1340224125,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					4,
					2
				],
				[
					7,
					7
				],
				[
					11,
					14
				],
				[
					13,
					24
				],
				[
					16,
					32
				],
				[
					17,
					39
				],
				[
					17,
					44
				],
				[
					19,
					47
				],
				[
					19,
					48
				],
				[
					20,
					48
				],
				[
					21,
					48
				],
				[
					23,
					44
				],
				[
					25,
					37
				],
				[
					28,
					28
				],
				[
					29,
					20
				],
				[
					31,
					11
				],
				[
					33,
					5
				],
				[
					34,
					1
				],
				[
					35,
					-1
				],
				[
					35,
					-1
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				35,
				-1
			]
		},
		{
			"id": "EkNPmFg4rLIO0kam5TYVC",
			"type": "freedraw",
			"x": -167.17022705078125,
			"y": -3194.984375,
			"width": 3,
			"height": 11,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 922196541,
			"version": 11,
			"versionNonce": 1013841875,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359845,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					2
				],
				[
					2,
					4
				],
				[
					3,
					6
				],
				[
					3,
					9
				],
				[
					3,
					10
				],
				[
					3,
					11
				],
				[
					3,
					11
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				3,
				11
			]
		},
		{
			"id": "myrTVuK_1aIrIvWukjxB6",
			"type": "freedraw",
			"x": -169.17022705078125,
			"y": -3216.984375,
			"width": 0.0001,
			"height": 0.0001,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 560714387,
			"version": 5,
			"versionNonce": 156293853,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				0.0001,
				0.0001
			]
		},
		{
			"id": "Oc_T_EkF6YmkMYFkBc0oL",
			"type": "freedraw",
			"x": -129.17022705078125,
			"y": -3220.984375,
			"width": 21,
			"height": 37,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 76548221,
			"version": 47,
			"versionNonce": 350522739,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					0
				],
				[
					-2,
					0
				],
				[
					-3,
					0
				],
				[
					-7,
					0
				],
				[
					-12,
					0
				],
				[
					-16,
					0
				],
				[
					-19,
					1
				],
				[
					-21,
					1
				],
				[
					-21,
					2
				],
				[
					-21,
					4
				],
				[
					-21,
					5
				],
				[
					-20,
					6
				],
				[
					-20,
					7
				],
				[
					-19,
					8
				],
				[
					-18,
					9
				],
				[
					-18,
					10
				],
				[
					-18,
					13
				],
				[
					-18,
					15
				],
				[
					-18,
					16
				],
				[
					-18,
					17
				],
				[
					-17,
					17
				],
				[
					-16,
					18
				],
				[
					-15,
					19
				],
				[
					-13,
					20
				],
				[
					-11,
					21
				],
				[
					-9,
					21
				],
				[
					-6,
					22
				],
				[
					-4,
					23
				],
				[
					-3,
					25
				],
				[
					-2,
					25
				],
				[
					-1,
					26
				],
				[
					-1,
					27
				],
				[
					-1,
					29
				],
				[
					-2,
					31
				],
				[
					-3,
					33
				],
				[
					-6,
					35
				],
				[
					-7,
					37
				],
				[
					-8,
					37
				],
				[
					-9,
					37
				],
				[
					-10,
					37
				],
				[
					-11,
					37
				],
				[
					-12,
					37
				],
				[
					-12,
					37
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-12,
				37
			]
		},
		{
			"id": "tVUZReUZRTJIQ7_tuxNUf",
			"type": "freedraw",
			"x": -106.17022705078125,
			"y": -3213.984375,
			"width": 22,
			"height": 24,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 2088159635,
			"version": 24,
			"versionNonce": 59471677,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					2
				],
				[
					0,
					6
				],
				[
					-1,
					10
				],
				[
					-1,
					16
				],
				[
					-1,
					20
				],
				[
					1,
					23
				],
				[
					3,
					24
				],
				[
					6,
					24
				],
				[
					9,
					24
				],
				[
					12,
					24
				],
				[
					15,
					24
				],
				[
					17,
					21
				],
				[
					19,
					17
				],
				[
					21,
					13
				],
				[
					21,
					8
				],
				[
					21,
					3
				],
				[
					21,
					1
				],
				[
					21,
					0
				],
				[
					21,
					0
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				21,
				0
			]
		},
		{
			"id": "QrhcbXLE6Bn1GAkpjPPRK",
			"type": "freedraw",
			"x": -51.17022705078125,
			"y": -3203.984375,
			"width": 42,
			"height": 22,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 367283059,
			"version": 36,
			"versionNonce": 1719166739,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					2
				],
				[
					0,
					3
				],
				[
					-2,
					5
				],
				[
					-5,
					6
				],
				[
					-8,
					8
				],
				[
					-12,
					8
				],
				[
					-14,
					9
				],
				[
					-16,
					9
				],
				[
					-18,
					9
				],
				[
					-19,
					5
				],
				[
					-19,
					1
				],
				[
					-19,
					-2
				],
				[
					-15,
					-6
				],
				[
					-11,
					-10
				],
				[
					-6,
					-12
				],
				[
					-4,
					-13
				],
				[
					-3,
					-13
				],
				[
					-2,
					-13
				],
				[
					0,
					-10
				],
				[
					1,
					-7
				],
				[
					2,
					-3
				],
				[
					2,
					1
				],
				[
					2,
					3
				],
				[
					3,
					5
				],
				[
					4,
					6
				],
				[
					5,
					6
				],
				[
					9,
					6
				],
				[
					14,
					6
				],
				[
					19,
					5
				],
				[
					23,
					4
				],
				[
					23,
					4
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				23,
				4
			]
		},
		{
			"id": "lOssmeDAZ_S04RaPiiOtK",
			"type": "freedraw",
			"x": -20.17022705078125,
			"y": -3228.984375,
			"width": 3,
			"height": 31,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 442130195,
			"version": 14,
			"versionNonce": 687048605,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					-1,
					2
				],
				[
					-1,
					7
				],
				[
					-2,
					14
				],
				[
					-3,
					22
				],
				[
					-3,
					27
				],
				[
					-3,
					30
				],
				[
					-3,
					31
				],
				[
					-2,
					31
				],
				[
					-2,
					31
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-2,
				31
			]
		},
		{
			"id": "Gb5VNOhR3DbLNs1SGZIw0",
			"type": "ellipse",
			"x": -407.17022705078125,
			"y": -3136.984375,
			"width": 89,
			"height": 67,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 1147843795,
			"version": 22,
			"versionNonce": 933235891,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "Y1df-0SkczbCWnadP7I8j",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "S0hMYnUg"
				}
			],
			"updated": 1682458359846,
			"link": null,
			"locked": false
		},
		{
			"id": "S0hMYnUg",
			"type": "text",
			"x": -365.3464778980553,
			"y": -3116.1724521697492,
			"width": 5.4199981689453125,
			"height": 25,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 559384595,
			"version": 5,
			"versionNonce": 465210365,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"text": "1",
			"rawText": "1",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "Gb5VNOhR3DbLNs1SGZIw0",
			"originalText": "1",
			"lineHeight": 1.25
		},
		{
			"id": "t7TJGdAo-l2dPN5XWZOet",
			"type": "ellipse",
			"x": -270.17022705078125,
			"y": -3131.984375,
			"width": 69,
			"height": 72,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 1708951773,
			"version": 45,
			"versionNonce": 2080505427,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "Y1df-0SkczbCWnadP7I8j",
					"type": "arrow"
				},
				{
					"id": "1hmz-YoG55m4fjpZkGcMU",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "kmG4Hbh1"
				}
			],
			"updated": 1682458359846,
			"link": null,
			"locked": false
		},
		{
			"id": "kmG4Hbh1",
			"type": "text",
			"x": -242.68540611890464,
			"y": -3108.440219122716,
			"width": 14.239990234375,
			"height": 25,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1704476701,
			"version": 5,
			"versionNonce": 1004667997,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"text": "2",
			"rawText": "2",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "t7TJGdAo-l2dPN5XWZOet",
			"originalText": "2",
			"lineHeight": 1.25
		},
		{
			"id": "wBWUPa15bJZTozUUK_ggT",
			"type": "ellipse",
			"x": -134.17022705078125,
			"y": -3129.984375,
			"width": 86,
			"height": 72,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 841892317,
			"version": 20,
			"versionNonce": 1853144051,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "1hmz-YoG55m4fjpZkGcMU",
					"type": "arrow"
				},
				{
					"id": "eHUs-Yqi4Pa-AfnRvpYuQ",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "7UaSmko6"
				},
				{
					"id": "fWZ3kM0OTqwYiTYHVyK9G",
					"type": "arrow"
				}
			],
			"updated": 1682458359846,
			"link": null,
			"locked": false
		},
		{
			"id": "7UaSmko6",
			"type": "text",
			"x": -97.88581620039655,
			"y": -3106.440219122716,
			"width": 13.6199951171875,
			"height": 25,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 466230355,
			"version": 5,
			"versionNonce": 1832612029,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"text": "3",
			"rawText": "3",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "wBWUPa15bJZTozUUK_ggT",
			"originalText": "3",
			"lineHeight": 1.25
		},
		{
			"id": "91srR5S_i6aUWMrfu2_iS",
			"type": "ellipse",
			"x": 152.82977294921875,
			"y": -3129.984375,
			"width": 94,
			"height": 76,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 471952509,
			"version": 64,
			"versionNonce": 721339795,
			"isDeleted": false,
			"boundElements": [
				{
					"id": "eHUs-Yqi4Pa-AfnRvpYuQ",
					"type": "arrow"
				},
				{
					"type": "text",
					"id": "iJ5qusjB"
				},
				{
					"id": "21uNE0M4GY_aRhDGJtb8J",
					"type": "arrow"
				}
			],
			"updated": 1682458359846,
			"link": null,
			"locked": false
		},
		{
			"id": "iJ5qusjB",
			"type": "text",
			"x": 193.19576033696663,
			"y": -3104.354432685089,
			"width": 12.79998779296875,
			"height": 25,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1383738429,
			"version": 35,
			"versionNonce": 493375773,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"text": "4",
			"rawText": "4",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "91srR5S_i6aUWMrfu2_iS",
			"originalText": "4",
			"lineHeight": 1.25
		},
		{
			"id": "Y1df-0SkczbCWnadP7I8j",
			"type": "arrow",
			"x": -316.172028414342,
			"y": -3098.984453320155,
			"width": 45.01590520493602,
			"height": 1.9572132697794586,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 458728979,
			"version": 41,
			"versionNonce": 1456328275,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458381663,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					45.01590520493602,
					1.9572132697794586
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "Gb5VNOhR3DbLNs1SGZIw0",
				"gap": 2.36849854167113,
				"focus": 0.07385486359001378
			},
			"endBinding": {
				"elementId": "t7TJGdAo-l2dPN5XWZOet",
				"gap": 1,
				"focus": -0.013876848237393777
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "1hmz-YoG55m4fjpZkGcMU",
			"type": "arrow",
			"x": -200.17022964135896,
			"y": -3097.9843751195654,
			"width": 65.00001612484283,
			"height": 3.0000007442235983,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 1566234419,
			"version": 36,
			"versionNonce": 18257299,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458381664,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					65.00001612484283,
					3.0000007442235983
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "t7TJGdAo-l2dPN5XWZOet",
				"gap": 1.0518283863858429,
				"focus": -0.10096965777929334
			},
			"endBinding": {
				"elementId": "wBWUPa15bJZTozUUK_ggT",
				"gap": 1.016051424829378,
				"focus": -0.028589068798272665
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "eHUs-Yqi4Pa-AfnRvpYuQ",
			"type": "arrow",
			"x": -44.0798425824032,
			"y": -3092.308616365731,
			"width": 193.98093256011788,
			"height": 2.730375953386101,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 1680826685,
			"version": 92,
			"versionNonce": 446921331,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458381665,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					193.98093256011788,
					2.730375953386101
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "wBWUPa15bJZTozUUK_ggT",
				"gap": 4.131492146287194,
				"focus": 0.028133206858789075
			},
			"endBinding": {
				"elementId": "91srR5S_i6aUWMrfu2_iS",
				"gap": 3.0148222138030647,
				"focus": -0.08180089645052044
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "czYakp4V",
			"type": "text",
			"x": 69.82977294921875,
			"y": -3194.984375,
			"width": 131.7598876953125,
			"height": 25,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1015837011,
			"version": 27,
			"versionNonce": 1171418589,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"text": "Insert after!",
			"rawText": "Insert after!",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "Insert after!",
			"lineHeight": 1.25
		},
		{
			"id": "z88CJX1apqOOuYfGj1T4c",
			"type": "freedraw",
			"x": 62.82977294921875,
			"y": -3171.984375,
			"width": 145,
			"height": 6,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1940781629,
			"version": 33,
			"versionNonce": 154774131,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2,
					0
				],
				[
					3,
					0
				],
				[
					9,
					0
				],
				[
					19,
					0
				],
				[
					31,
					2
				],
				[
					43,
					3
				],
				[
					56,
					3
				],
				[
					67,
					4
				],
				[
					76,
					5
				],
				[
					84,
					5
				],
				[
					92,
					5
				],
				[
					97,
					6
				],
				[
					104,
					6
				],
				[
					108,
					6
				],
				[
					112,
					6
				],
				[
					116,
					6
				],
				[
					120,
					5
				],
				[
					124,
					4
				],
				[
					127,
					3
				],
				[
					128,
					3
				],
				[
					130,
					3
				],
				[
					132,
					3
				],
				[
					134,
					2
				],
				[
					137,
					2
				],
				[
					140,
					2
				],
				[
					142,
					2
				],
				[
					143,
					2
				],
				[
					144,
					2
				],
				[
					145,
					2
				],
				[
					145,
					2
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				145,
				2
			]
		},
		{
			"id": "rm4S8H8IVfkMx_SLBRfz8",
			"type": "freedraw",
			"x": -216.17022705078125,
			"y": -3168.984375,
			"width": 231,
			"height": 28,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 903045181,
			"version": 32,
			"versionNonce": 6466109,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					7,
					0
				],
				[
					17,
					-1
				],
				[
					31,
					-2
				],
				[
					48,
					-3
				],
				[
					62,
					-4
				],
				[
					75,
					-6
				],
				[
					88,
					-7
				],
				[
					100,
					-9
				],
				[
					111,
					-10
				],
				[
					123,
					-13
				],
				[
					134,
					-14
				],
				[
					144,
					-16
				],
				[
					153,
					-18
				],
				[
					163,
					-19
				],
				[
					174,
					-21
				],
				[
					182,
					-22
				],
				[
					189,
					-24
				],
				[
					196,
					-24
				],
				[
					202,
					-25
				],
				[
					206,
					-25
				],
				[
					211,
					-25
				],
				[
					216,
					-26
				],
				[
					221,
					-27
				],
				[
					227,
					-28
				],
				[
					229,
					-28
				],
				[
					230,
					-28
				],
				[
					231,
					-28
				],
				[
					231,
					-28
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				231,
				-28
			]
		},
		{
			"id": "sjIQa0GIzei97ccXL8vfX",
			"type": "ellipse",
			"x": -3.17022705078125,
			"y": -3034.984375,
			"width": 97,
			"height": 78,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 413640125,
			"version": 134,
			"versionNonce": 740418579,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "v0rjeYWP"
				},
				{
					"id": "fWZ3kM0OTqwYiTYHVyK9G",
					"type": "arrow"
				},
				{
					"id": "21uNE0M4GY_aRhDGJtb8J",
					"type": "arrow"
				}
			],
			"updated": 1682458359846,
			"link": null,
			"locked": false
		},
		{
			"id": "v0rjeYWP",
			"type": "text",
			"x": 39.355101385889945,
			"y": -3008.5615394662755,
			"width": 12.3599853515625,
			"height": 25,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1222897907,
			"version": 107,
			"versionNonce": 174873245,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"text": "5",
			"rawText": "5",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "sjIQa0GIzei97ccXL8vfX",
			"originalText": "5",
			"lineHeight": 1.25
		},
		{
			"id": "6GHh6vRF",
			"type": "text",
			"x": 280.82977294921875,
			"y": -3178.984375,
			"width": 92.41990661621094,
			"height": 25,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 754651891,
			"version": 16,
			"versionNonce": 1695672755,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"text": "input(3,5)",
			"rawText": "input(3,5)",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "input(3,5)",
			"lineHeight": 1.25
		},
		{
			"id": "fWZ3kM0OTqwYiTYHVyK9G",
			"type": "arrow",
			"x": -53.17455302811668,
			"y": -3073.988261047437,
			"width": 59.011014421099894,
			"height": 53.00989431047947,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 2026115411,
			"version": 42,
			"versionNonce": 1648867763,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458381666,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					59.011014421099894,
					53.00989431047947
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "wBWUPa15bJZTozUUK_ggT",
				"gap": 1.7817302745750965,
				"focus": -0.2677092796715283
			},
			"endBinding": {
				"elementId": "sjIQa0GIzei97ccXL8vfX",
				"gap": 1.608814255693595,
				"focus": -0.17927859132065752
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "21uNE0M4GY_aRhDGJtb8J",
			"type": "arrow",
			"x": 89.82068750357685,
			"y": -3015.9792644368267,
			"width": 80.01609177307317,
			"height": 45.00905162235358,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"seed": 267824893,
			"version": 50,
			"versionNonce": 791415635,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458381666,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					80.01609177307317,
					-45.00905162235358
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "sjIQa0GIzei97ccXL8vfX",
				"gap": 2.334321338797089,
				"focus": 0.10571003990014341
			},
			"endBinding": {
				"elementId": "91srR5S_i6aUWMrfu2_iS",
				"gap": 1.461798310098402,
				"focus": -0.30512887533034433
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "fHzsalqlZkgSjp_Boa-f1",
			"type": "freedraw",
			"x": 76.82977294921875,
			"y": -3115.984375,
			"width": 47,
			"height": 47,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 857801267,
			"version": 15,
			"versionNonce": 1568806749,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					3
				],
				[
					-3,
					6
				],
				[
					-8,
					11
				],
				[
					-14,
					17
				],
				[
					-21,
					24
				],
				[
					-29,
					31
				],
				[
					-37,
					37
				],
				[
					-41,
					42
				],
				[
					-44,
					45
				],
				[
					-46,
					46
				],
				[
					-47,
					47
				],
				[
					-47,
					47
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-47,
				47
			]
		},
		{
			"id": "sNvQRu-fyqBx3dAQRorXC",
			"type": "freedraw",
			"x": 30.82977294921875,
			"y": -3126.984375,
			"width": 49,
			"height": 64,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 903219603,
			"version": 16,
			"versionNonce": 1154701555,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					2,
					3
				],
				[
					6,
					9
				],
				[
					12,
					17
				],
				[
					18,
					24
				],
				[
					24,
					32
				],
				[
					29,
					40
				],
				[
					33,
					46
				],
				[
					38,
					52
				],
				[
					43,
					57
				],
				[
					46,
					61
				],
				[
					49,
					64
				],
				[
					49,
					64
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				49,
				64
			]
		},
		{
			"id": "lNU2VErlGPWinAFTtsLAg",
			"type": "freedraw",
			"x": 171.82977294921875,
			"y": -3147.984375,
			"width": 0,
			"height": 12,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 562274237,
			"version": 10,
			"versionNonce": 660677565,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					4
				],
				[
					0,
					7
				],
				[
					0,
					10
				],
				[
					0,
					11
				],
				[
					0,
					12
				],
				[
					0,
					12
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				0,
				12
			]
		},
		{
			"id": "aoi7uuHgC4Sn5_qNa2cmz",
			"type": "freedraw",
			"x": 157.82977294921875,
			"y": -3152.984375,
			"width": 29,
			"height": 2,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 961520915,
			"version": 19,
			"versionNonce": 1434567315,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					3,
					0
				],
				[
					6,
					0
				],
				[
					9,
					0
				],
				[
					11,
					0
				],
				[
					13,
					0
				],
				[
					15,
					0
				],
				[
					17,
					0
				],
				[
					20,
					0
				],
				[
					22,
					0
				],
				[
					24,
					-1
				],
				[
					26,
					-1
				],
				[
					27,
					-2
				],
				[
					28,
					-2
				],
				[
					29,
					-2
				],
				[
					29,
					-2
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				29,
				-2
			]
		},
		{
			"id": "Ex8BEUDTZjyqtRzV4iym4",
			"type": "freedraw",
			"x": 190.82977294921875,
			"y": -3143.984375,
			"width": 20,
			"height": 13,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1618175923,
			"version": 39,
			"versionNonce": 241148957,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					5,
					0
				],
				[
					10,
					0
				],
				[
					12,
					-1
				],
				[
					14,
					-2
				],
				[
					15,
					-3
				],
				[
					16,
					-4
				],
				[
					16,
					-5
				],
				[
					15,
					-6
				],
				[
					14,
					-7
				],
				[
					13,
					-7
				],
				[
					12,
					-7
				],
				[
					11,
					-7
				],
				[
					9,
					-7
				],
				[
					8,
					-7
				],
				[
					6,
					-6
				],
				[
					4,
					-5
				],
				[
					3,
					-4
				],
				[
					3,
					-2
				],
				[
					1,
					-1
				],
				[
					1,
					0
				],
				[
					0,
					2
				],
				[
					0,
					3
				],
				[
					-1,
					3
				],
				[
					-1,
					4
				],
				[
					-1,
					5
				],
				[
					-1,
					6
				],
				[
					0,
					6
				],
				[
					2,
					6
				],
				[
					5,
					6
				],
				[
					9,
					6
				],
				[
					12,
					6
				],
				[
					15,
					6
				],
				[
					18,
					6
				],
				[
					19,
					6
				],
				[
					19,
					6
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				19,
				6
			]
		},
		{
			"id": "D7XTpl8ETvvotpNN4Ez6p",
			"type": "freedraw",
			"x": 221.82977294921875,
			"y": -3148.984375,
			"width": 20,
			"height": 21,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1448016531,
			"version": 40,
			"versionNonce": 1139931187,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					3
				],
				[
					0,
					6
				],
				[
					0,
					9
				],
				[
					0,
					12
				],
				[
					0,
					13
				],
				[
					0,
					12
				],
				[
					0,
					9
				],
				[
					1,
					3
				],
				[
					1,
					2
				],
				[
					3,
					0
				],
				[
					4,
					0
				],
				[
					5,
					0
				],
				[
					6,
					0
				],
				[
					8,
					0
				],
				[
					10,
					3
				],
				[
					11,
					5
				],
				[
					11,
					8
				],
				[
					12,
					10
				],
				[
					12,
					11
				],
				[
					12,
					12
				],
				[
					12,
					11
				],
				[
					12,
					8
				],
				[
					12,
					4
				],
				[
					14,
					1
				],
				[
					15,
					1
				],
				[
					16,
					1
				],
				[
					17,
					1
				],
				[
					18,
					1
				],
				[
					19,
					2
				],
				[
					20,
					4
				],
				[
					20,
					7
				],
				[
					20,
					10
				],
				[
					20,
					13
				],
				[
					19,
					16
				],
				[
					19,
					18
				],
				[
					19,
					21
				],
				[
					19,
					21
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				19,
				21
			]
		},
		{
			"id": "mD1WvX-urozcKNKSsu9j4",
			"type": "freedraw",
			"x": 252.82977294921875,
			"y": -3144.984375,
			"width": 0,
			"height": 16,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 336431933,
			"version": 12,
			"versionNonce": 644814973,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					2
				],
				[
					0,
					4
				],
				[
					0,
					7
				],
				[
					0,
					11
				],
				[
					0,
					13
				],
				[
					0,
					15
				],
				[
					0,
					16
				],
				[
					0,
					16
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				0,
				16
			]
		},
		{
			"id": "Ha3CILiBy1QDAgjJibXRX",
			"type": "freedraw",
			"x": 252.82977294921875,
			"y": -3149.984375,
			"width": 9,
			"height": 10,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 787760947,
			"version": 21,
			"versionNonce": 235567571,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					4,
					0
				],
				[
					6,
					1
				],
				[
					7,
					2
				],
				[
					8,
					2
				],
				[
					8,
					4
				],
				[
					8,
					6
				],
				[
					8,
					8
				],
				[
					8,
					9
				],
				[
					7,
					9
				],
				[
					5,
					10
				],
				[
					4,
					10
				],
				[
					1,
					10
				],
				[
					0,
					10
				],
				[
					-1,
					10
				],
				[
					-1,
					9
				],
				[
					-1,
					9
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-1,
				9
			]
		},
		{
			"id": "MdCVTN6HLWKMhB5u39ODu",
			"type": "freedraw",
			"x": -127.17022705078125,
			"y": -3150.984375,
			"width": 0,
			"height": 21,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 102265715,
			"version": 12,
			"versionNonce": 156303581,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					0,
					2
				],
				[
					0,
					6
				],
				[
					0,
					10
				],
				[
					0,
					15
				],
				[
					0,
					18
				],
				[
					0,
					20
				],
				[
					0,
					21
				],
				[
					0,
					21
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				0,
				21
			]
		},
		{
			"id": "KShb-8DHa7UHU9Z-rFzoh",
			"type": "freedraw",
			"x": -141.17022705078125,
			"y": -3150.984375,
			"width": 26,
			"height": 4,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 362908445,
			"version": 12,
			"versionNonce": 820103027,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					-1
				],
				[
					6,
					-1
				],
				[
					11,
					-2
				],
				[
					17,
					-3
				],
				[
					22,
					-3
				],
				[
					24,
					-4
				],
				[
					26,
					-4
				],
				[
					26,
					-4
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				26,
				-4
			]
		},
		{
			"id": "4m7hjGNLAMy91lS53VxH-",
			"type": "freedraw",
			"x": -116.17022705078125,
			"y": -3140.984375,
			"width": 14,
			"height": 18,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 593486163,
			"version": 34,
			"versionNonce": 479649085,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					3,
					0
				],
				[
					6,
					0
				],
				[
					9,
					-1
				],
				[
					10,
					-1
				],
				[
					11,
					-3
				],
				[
					12,
					-4
				],
				[
					13,
					-5
				],
				[
					13,
					-7
				],
				[
					12,
					-8
				],
				[
					11,
					-9
				],
				[
					10,
					-9
				],
				[
					9,
					-9
				],
				[
					8,
					-9
				],
				[
					6,
					-9
				],
				[
					4,
					-7
				],
				[
					2,
					-5
				],
				[
					0,
					-4
				],
				[
					-1,
					-2
				],
				[
					-1,
					0
				],
				[
					-1,
					2
				],
				[
					-1,
					4
				],
				[
					0,
					6
				],
				[
					2,
					8
				],
				[
					4,
					9
				],
				[
					5,
					9
				],
				[
					6,
					9
				],
				[
					8,
					9
				],
				[
					10,
					8
				],
				[
					12,
					5
				],
				[
					12,
					5
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				12,
				5
			]
		},
		{
			"id": "ez7MIstHCNlkwUwHllkvu",
			"type": "freedraw",
			"x": -100.17022705078125,
			"y": -3141.984375,
			"width": 27,
			"height": 20,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 604698461,
			"version": 38,
			"versionNonce": 1119772947,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					1,
					1
				],
				[
					1,
					2
				],
				[
					1,
					4
				],
				[
					1,
					5
				],
				[
					1,
					7
				],
				[
					1,
					8
				],
				[
					1,
					6
				],
				[
					1,
					1
				],
				[
					2,
					-3
				],
				[
					3,
					-6
				],
				[
					5,
					-7
				],
				[
					6,
					-8
				],
				[
					7,
					-8
				],
				[
					9,
					-7
				],
				[
					10,
					-5
				],
				[
					11,
					-3
				],
				[
					11,
					0
				],
				[
					11,
					1
				],
				[
					11,
					0
				],
				[
					11,
					-3
				],
				[
					11,
					-7
				],
				[
					13,
					-10
				],
				[
					15,
					-12
				],
				[
					17,
					-12
				],
				[
					20,
					-12
				],
				[
					23,
					-12
				],
				[
					25,
					-12
				],
				[
					26,
					-10
				],
				[
					27,
					-8
				],
				[
					27,
					-5
				],
				[
					27,
					-4
				],
				[
					27,
					-3
				],
				[
					27,
					-2
				],
				[
					27,
					-2
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				27,
				-2
			]
		},
		{
			"id": "eI-uwZkU5R8nr4xr0vU_D",
			"type": "freedraw",
			"x": -64.17022705078125,
			"y": -3157.984375,
			"width": 2,
			"height": 21,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 2085540403,
			"version": 11,
			"versionNonce": 396504477,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					1,
					5
				],
				[
					2,
					9
				],
				[
					2,
					15
				],
				[
					2,
					18
				],
				[
					2,
					20
				],
				[
					2,
					21
				],
				[
					2,
					21
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				2,
				21
			]
		},
		{
			"id": "IPhyXSmLjStlSOECH1gNe",
			"type": "freedraw",
			"x": -61.17022705078125,
			"y": -3161.984375,
			"width": 13,
			"height": 13,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1202066003,
			"version": 19,
			"versionNonce": 1293338291,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					3,
					0
				],
				[
					5,
					0
				],
				[
					8,
					1
				],
				[
					9,
					1
				],
				[
					10,
					3
				],
				[
					12,
					5
				],
				[
					13,
					8
				],
				[
					13,
					10
				],
				[
					13,
					12
				],
				[
					11,
					13
				],
				[
					9,
					13
				],
				[
					7,
					13
				],
				[
					4,
					13
				],
				[
					3,
					13
				],
				[
					3,
					13
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				3,
				13
			]
		},
		{
			"id": "lh8fGLcYX6U_faohtNisW",
			"type": "freedraw",
			"x": -40.17022705078125,
			"y": -3148.984375,
			"width": 15,
			"height": 32,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 553708787,
			"version": 41,
			"versionNonce": 1235513853,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					1,
					3
				],
				[
					2,
					6
				],
				[
					3,
					8
				],
				[
					3,
					10
				],
				[
					3,
					11
				],
				[
					3,
					10
				],
				[
					3,
					9
				],
				[
					2,
					5
				],
				[
					1,
					1
				],
				[
					0,
					-3
				],
				[
					0,
					-7
				],
				[
					0,
					-9
				],
				[
					1,
					-12
				],
				[
					1,
					-14
				],
				[
					2,
					-16
				],
				[
					3,
					-19
				],
				[
					4,
					-20
				],
				[
					4,
					-21
				],
				[
					5,
					-21
				],
				[
					7,
					-21
				],
				[
					9,
					-19
				],
				[
					11,
					-17
				],
				[
					12,
					-14
				],
				[
					13,
					-12
				],
				[
					14,
					-9
				],
				[
					15,
					-8
				],
				[
					15,
					-6
				],
				[
					15,
					-5
				],
				[
					13,
					-5
				],
				[
					12,
					-5
				],
				[
					9,
					-4
				],
				[
					6,
					-4
				],
				[
					4,
					-4
				],
				[
					3,
					-4
				],
				[
					2,
					-4
				],
				[
					0,
					0
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				2,
				-4
			]
		},
		{
			"id": "ZjRrw6nnUhJlAzAK7vdil",
			"type": "freedraw",
			"x": -16.17022705078125,
			"y": -3144.984375,
			"width": 6,
			"height": 20,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1766233459,
			"version": 17,
			"versionNonce": 1720809555,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					2
				],
				[
					2,
					4
				],
				[
					3,
					5
				],
				[
					3,
					4
				],
				[
					2,
					0
				],
				[
					-1,
					-7
				],
				[
					-2,
					-11
				],
				[
					-2,
					-14
				],
				[
					-2,
					-15
				],
				[
					-1,
					-15
				],
				[
					1,
					-15
				],
				[
					2,
					-15
				],
				[
					4,
					-15
				],
				[
					4,
					-15
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				4,
				-15
			]
		},
		{
			"id": "g-jXaiuz4cf3Mi8wZSCN5",
			"type": "freedraw",
			"x": -4.17022705078125,
			"y": -3153.984375,
			"width": 8,
			"height": 19,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1427354227,
			"version": 29,
			"versionNonce": 530524765,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2,
					0
				],
				[
					3,
					0
				],
				[
					4,
					0
				],
				[
					4,
					-2
				],
				[
					3,
					-5
				],
				[
					3,
					-6
				],
				[
					2,
					-6
				],
				[
					1,
					-6
				],
				[
					-1,
					-4
				],
				[
					-2,
					-4
				],
				[
					-3,
					-2
				],
				[
					-3,
					0
				],
				[
					-3,
					1
				],
				[
					-4,
					4
				],
				[
					-4,
					5
				],
				[
					-4,
					8
				],
				[
					-4,
					10
				],
				[
					-3,
					12
				],
				[
					-3,
					13
				],
				[
					-2,
					13
				],
				[
					-1,
					13
				],
				[
					0,
					13
				],
				[
					1,
					13
				],
				[
					2,
					12
				],
				[
					3,
					12
				],
				[
					3,
					12
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				3,
				12
			]
		},
		{
			"id": "Huudc5as1u6NRZeZsOrvI",
			"type": "freedraw",
			"x": 4.82977294921875,
			"y": -3156.984375,
			"width": 16,
			"height": 14,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 1347181875,
			"version": 24,
			"versionNonce": 218428915,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2
				],
				[
					0,
					5
				],
				[
					1,
					7
				],
				[
					1,
					10
				],
				[
					2,
					11
				],
				[
					3,
					12
				],
				[
					4,
					12
				],
				[
					5,
					12
				],
				[
					6,
					12
				],
				[
					8,
					12
				],
				[
					9,
					12
				],
				[
					11,
					12
				],
				[
					12,
					12
				],
				[
					13,
					12
				],
				[
					14,
					9
				],
				[
					15,
					7
				],
				[
					15,
					4
				],
				[
					15,
					2
				],
				[
					16,
					0
				],
				[
					16,
					-2
				],
				[
					16,
					-2
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				16,
				-2
			]
		},
		{
			"id": "ywCeGsYbdtEA9fWeLkMRO",
			"type": "freedraw",
			"x": 157.82977294921875,
			"y": 399.015625,
			"width": 0.0001,
			"height": 0.0001,
			"angle": 0,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"roundness": null,
			"seed": 318262173,
			"version": 4,
			"versionNonce": 1784927933,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				0.0001,
				0.0001
			]
		},
		{
			"type": "freedraw",
			"version": 87,
			"versionNonce": 1064812435,
			"isDeleted": false,
			"id": "YKBlQqc4kNTd-rSq2-c7F",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 228,
			"y": -1576.484375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 25,
			"height": 89,
			"seed": 1257587187,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					3,
					5
				],
				[
					5,
					11
				],
				[
					9,
					21
				],
				[
					12,
					32
				],
				[
					15,
					42
				],
				[
					17,
					51
				],
				[
					19,
					60
				],
				[
					20,
					69
				],
				[
					21,
					77
				],
				[
					23,
					82
				],
				[
					24,
					86
				],
				[
					24,
					88
				],
				[
					25,
					89
				],
				[
					25,
					89
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 114,
			"versionNonce": 1687418653,
			"isDeleted": false,
			"id": "RU_G0ZcheRlxx3dEfEQ0a",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 225,
			"y": -1579.484375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 71,
			"height": 75,
			"seed": 295304637,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					4,
					-1
				],
				[
					6,
					-2
				],
				[
					10,
					-3
				],
				[
					15,
					-4
				],
				[
					23,
					-4
				],
				[
					35,
					-4
				],
				[
					48,
					-3
				],
				[
					58,
					0
				],
				[
					63,
					3
				],
				[
					65,
					5
				],
				[
					65,
					8
				],
				[
					65,
					11
				],
				[
					62,
					13
				],
				[
					58,
					15
				],
				[
					53,
					17
				],
				[
					48,
					18
				],
				[
					42,
					20
				],
				[
					38,
					20
				],
				[
					37,
					20
				],
				[
					38,
					20
				],
				[
					40,
					21
				],
				[
					45,
					22
				],
				[
					53,
					25
				],
				[
					60,
					29
				],
				[
					67,
					34
				],
				[
					69,
					38
				],
				[
					71,
					43
				],
				[
					71,
					48
				],
				[
					71,
					54
				],
				[
					71,
					60
				],
				[
					69,
					66
				],
				[
					66,
					69
				],
				[
					62,
					70
				],
				[
					57,
					71
				],
				[
					52,
					71
				],
				[
					44,
					71
				],
				[
					36,
					71
				],
				[
					31,
					70
				],
				[
					28,
					70
				],
				[
					28,
					70
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 81,
			"versionNonce": 1478513971,
			"isDeleted": false,
			"id": "eyZXo0dUTHC5f37D9MYuW",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 315,
			"y": -1547.484375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 12,
			"height": 17,
			"seed": 1700508157,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					4,
					3
				],
				[
					7,
					5
				],
				[
					9,
					9
				],
				[
					11,
					13
				],
				[
					12,
					15
				],
				[
					12,
					17
				],
				[
					12,
					17
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 73,
			"versionNonce": 2023820157,
			"isDeleted": false,
			"id": "gi3kWoEEDiBQ1JpDyAwS5",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 314,
			"y": -1565.484375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 88188019,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 97,
			"versionNonce": 644167379,
			"isDeleted": false,
			"id": "-mTMYw35L9v51Vmni-_ta",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 380,
			"y": -1582.484375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 40,
			"height": 50,
			"seed": 301219997,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					1
				],
				[
					-9,
					8
				],
				[
					-11,
					10
				],
				[
					-18,
					16
				],
				[
					-23,
					24
				],
				[
					-26,
					33
				],
				[
					-28,
					40
				],
				[
					-28,
					46
				],
				[
					-26,
					49
				],
				[
					-23,
					50
				],
				[
					-21,
					50
				],
				[
					-18,
					50
				],
				[
					-12,
					48
				],
				[
					-6,
					43
				],
				[
					0,
					38
				],
				[
					6,
					35
				],
				[
					9,
					33
				],
				[
					11,
					30
				],
				[
					12,
					29
				],
				[
					12,
					28
				],
				[
					11,
					28
				],
				[
					8,
					28
				],
				[
					5,
					28
				],
				[
					4,
					28
				],
				[
					4,
					28
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 73,
			"versionNonce": 1187812317,
			"isDeleted": false,
			"id": "hHLjW4DytjAL_7co-r1Dq",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 380,
			"y": -1555.484375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 800092371,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 87,
			"versionNonce": 1222435955,
			"isDeleted": false,
			"id": "NNn5c11uf43grwGWJFIZ-",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 193,
			"y": -1474.484375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 301,
			"height": 71,
			"seed": 2036254451,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					0
				],
				[
					18,
					-3
				],
				[
					40,
					-8
				],
				[
					74,
					-14
				],
				[
					112,
					-22
				],
				[
					147,
					-30
				],
				[
					184,
					-39
				],
				[
					218,
					-49
				],
				[
					250,
					-57
				],
				[
					273,
					-63
				],
				[
					287,
					-66
				],
				[
					296,
					-69
				],
				[
					300,
					-70
				],
				[
					301,
					-71
				],
				[
					301,
					-71
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 470,
			"versionNonce": 1797787709,
			"isDeleted": false,
			"id": "lJKuSIw4",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 129,
			"y": -1452.484375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 559.6595458984375,
			"height": 200,
			"seed": 1643923645,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "The Time complexity will be O(n) due to the fact that \n    the time to complete will relate to the length of\nthe Linked list, into infinity.\n\nThe space complexity will be O(1) due to the fact that \nthe nodes will take up the same space for each node \ncreated.\n",
			"rawText": "The Time complexity will be O(n) due to the fact that \n    the time to complete will relate to the length of\nthe Linked list, into infinity.\n\nThe space complexity will be O(1) due to the fact that \nthe nodes will take up the same space for each node \ncreated.\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "The Time complexity will be O(n) due to the fact that \n    the time to complete will relate to the length of\nthe Linked list, into infinity.\n\nThe space complexity will be O(1) due to the fact that \nthe nodes will take up the same space for each node \ncreated.\n",
			"lineHeight": 1.25,
			"baseline": 193
		},
		{
			"type": "freedraw",
			"version": 53,
			"versionNonce": 1196285459,
			"isDeleted": false,
			"id": "GUcouD-XYDM9r6szShYKB",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 280.57977294921875,
			"y": -1331.2265625,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 318262173,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 1034,
			"versionNonce": 439682579,
			"isDeleted": false,
			"id": "PVbPGUa4",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -596.9740611881381,
			"y": -2798.1183331805855,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 612.259521484375,
			"height": 650,
			"seed": 1267583709,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682459095827,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "public void insertBefore(int value, int newValue)\nthrow IllegalArgumentException{   \n if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n}\nNode temp = head;\nNode prevNode = null;\nNode newNode = new Node(newValue)\n\nif (temp.value == value){\n    newNode.next = temp;\n    head = newNode;\n    return;\n}\n\nwhile(temp.next != null){\nprevTemp = temp;\ntemp = temp.next;\nif(prevTemp.value == value){\nnewNode.next = temp;\nprevTemp.next = newNode;\nreturn;\n}\n}\n\n}",
			"rawText": "public void insertBefore(int value, int newValue)\nthrow IllegalArgumentException{   \n if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n}\nNode temp = head;\nNode prevNode = null;\nNode newNode = new Node(newValue)\n\nif (temp.value == value){\n    newNode.next = temp;\n    head = newNode;\n    return;\n}\n\nwhile(temp.next != null){\nprevTemp = temp;\ntemp = temp.next;\nif(prevTemp.value == value){\nnewNode.next = temp;\nprevTemp.next = newNode;\nreturn;\n}\n}\n\n}",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "public void insertBefore(int value, int newValue)\nthrow IllegalArgumentException{   \n if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n}\nNode temp = head;\nNode prevNode = null;\nNode newNode = new Node(newValue)\n\nif (temp.value == value){\n    newNode.next = temp;\n    head = newNode;\n    return;\n}\n\nwhile(temp.next != null){\nprevTemp = temp;\ntemp = temp.next;\nif(prevTemp.value == value){\nnewNode.next = temp;\nprevTemp.next = newNode;\nreturn;\n}\n}\n\n}",
			"lineHeight": 1.25,
			"baseline": 643
		},
		{
			"type": "arrow",
			"version": 228,
			"versionNonce": 1823384499,
			"isDeleted": false,
			"id": "oqgGuAbYEE2WsZ-moT9jJ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -310.49806612052566,
			"y": -2500.63801874188,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 131,
			"height": 37,
			"seed": 506307581,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": {
				"elementId": "p3JxAlkY",
				"focus": 0.5506648896505036,
				"gap": 11
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					131,
					-37
				]
			]
		},
		{
			"type": "text",
			"version": 326,
			"versionNonce": 1975837949,
			"isDeleted": false,
			"id": "p3JxAlkY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -236.49806612052566,
			"y": -2573.63801874188,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 732.5194091796875,
			"height": 25,
			"seed": 918644531,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "oqgGuAbYEE2WsZ-moT9jJ",
					"type": "arrow"
				}
			],
			"updated": 1682458359846,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "This is an edge case incase the value is the first node in the LinkedList.",
			"rawText": "This is an edge case incase the value is the first node in the LinkedList.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "This is an edge case incase the value is the first node in the LinkedList.",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "freedraw",
			"version": 118,
			"versionNonce": 1634928093,
			"isDeleted": false,
			"id": "ANibH4BplmtejI3XBxt3i",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -519.3922076845283,
			"y": -2850.714941818803,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 48,
			"height": 82,
			"seed": 855304627,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458367670,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					-1
				],
				[
					2,
					-4
				],
				[
					4,
					-9
				],
				[
					6,
					-15
				],
				[
					9,
					-23
				],
				[
					12,
					-31
				],
				[
					14,
					-39
				],
				[
					15,
					-45
				],
				[
					17,
					-51
				],
				[
					19,
					-58
				],
				[
					20,
					-66
				],
				[
					21,
					-73
				],
				[
					22,
					-78
				],
				[
					23,
					-81
				],
				[
					23,
					-82
				],
				[
					26,
					-81
				],
				[
					29,
					-75
				],
				[
					31,
					-68
				],
				[
					32,
					-58
				],
				[
					33,
					-48
				],
				[
					35,
					-38
				],
				[
					39,
					-29
				],
				[
					43,
					-21
				],
				[
					44,
					-16
				],
				[
					46,
					-13
				],
				[
					47,
					-11
				],
				[
					48,
					-9
				],
				[
					48,
					-8
				],
				[
					48,
					-8
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 101,
			"versionNonce": 1737396851,
			"isDeleted": false,
			"id": "yD_zHcDOFh2OrpNuylP_b",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -507.39220768452833,
			"y": -2890.714941818803,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 30,
			"height": 2,
			"seed": 261882013,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458367670,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					5,
					0
				],
				[
					10,
					0
				],
				[
					15,
					1
				],
				[
					18,
					1
				],
				[
					21,
					1
				],
				[
					22,
					1
				],
				[
					23,
					1
				],
				[
					25,
					2
				],
				[
					28,
					2
				],
				[
					30,
					2
				],
				[
					30,
					2
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 100,
			"versionNonce": 204489277,
			"isDeleted": false,
			"id": "9SDGu4YDW4yg2JdT6KUMs",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -447.3922076845282,
			"y": -2921.714941818803,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 7,
			"height": 60,
			"seed": 687686461,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458367670,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					2
				],
				[
					1,
					7
				],
				[
					2,
					14
				],
				[
					2,
					22
				],
				[
					3,
					31
				],
				[
					4,
					39
				],
				[
					4,
					47
				],
				[
					6,
					54
				],
				[
					6,
					59
				],
				[
					7,
					60
				],
				[
					7,
					60
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 130,
			"versionNonce": 1067043859,
			"isDeleted": false,
			"id": "jfOK4vkqGWU1L3Y6ybRXl",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -378.3922076845282,
			"y": -2914.714941818803,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 41,
			"height": 53,
			"seed": 947695827,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458367670,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2,
					-1
				],
				[
					-4,
					-1
				],
				[
					-7,
					-1
				],
				[
					-11,
					-1
				],
				[
					-17,
					0
				],
				[
					-23,
					2
				],
				[
					-28,
					4
				],
				[
					-32,
					8
				],
				[
					-36,
					14
				],
				[
					-39,
					19
				],
				[
					-41,
					25
				],
				[
					-41,
					31
				],
				[
					-41,
					36
				],
				[
					-41,
					41
				],
				[
					-39,
					45
				],
				[
					-37,
					48
				],
				[
					-34,
					50
				],
				[
					-32,
					52
				],
				[
					-29,
					52
				],
				[
					-27,
					52
				],
				[
					-25,
					52
				],
				[
					-21,
					52
				],
				[
					-17,
					50
				],
				[
					-13,
					49
				],
				[
					-11,
					48
				],
				[
					-9,
					45
				],
				[
					-9,
					43
				],
				[
					-9,
					40
				],
				[
					-9,
					36
				],
				[
					-9,
					34
				],
				[
					-10,
					32
				],
				[
					-11,
					30
				],
				[
					-12,
					29
				],
				[
					-13,
					29
				],
				[
					-14,
					29
				],
				[
					-16,
					29
				],
				[
					-19,
					29
				],
				[
					-22,
					29
				],
				[
					-25,
					29
				],
				[
					-27,
					29
				],
				[
					-27,
					29
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 123,
			"versionNonce": 2026304157,
			"isDeleted": false,
			"id": "FAEcjfs_3cIlsNkHRQsOn",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -328.3922076845282,
			"y": -2870.714941818803,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 39,
			"height": 38,
			"seed": 281761213,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458367670,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					-1,
					3
				],
				[
					-3,
					5
				],
				[
					-7,
					6
				],
				[
					-11,
					7
				],
				[
					-15,
					7
				],
				[
					-19,
					7
				],
				[
					-22,
					5
				],
				[
					-27,
					2
				],
				[
					-31,
					-2
				],
				[
					-33,
					-5
				],
				[
					-35,
					-9
				],
				[
					-35,
					-15
				],
				[
					-35,
					-18
				],
				[
					-35,
					-21
				],
				[
					-32,
					-24
				],
				[
					-29,
					-26
				],
				[
					-24,
					-27
				],
				[
					-19,
					-27
				],
				[
					-15,
					-27
				],
				[
					-10,
					-26
				],
				[
					-4,
					-23
				],
				[
					0,
					-20
				],
				[
					2,
					-18
				],
				[
					3,
					-16
				],
				[
					4,
					-14
				],
				[
					4,
					-10
				],
				[
					4,
					-6
				],
				[
					2,
					-2
				],
				[
					0,
					3
				],
				[
					-3,
					7
				],
				[
					-4,
					10
				],
				[
					-5,
					11
				],
				[
					-5,
					11
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 129,
			"versionNonce": 290247091,
			"isDeleted": false,
			"id": "8s1Kx3gCxFaYVU2GdR5e1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -567.3922076845283,
			"y": -2840.714941818803,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 302,
			"height": 4,
			"seed": 1859235965,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458367670,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2,
					0
				],
				[
					8,
					0
				],
				[
					16,
					0
				],
				[
					28,
					0
				],
				[
					45,
					0
				],
				[
					63,
					1
				],
				[
					80,
					2
				],
				[
					97,
					4
				],
				[
					111,
					4
				],
				[
					122,
					4
				],
				[
					136,
					4
				],
				[
					144,
					4
				],
				[
					154,
					4
				],
				[
					164,
					4
				],
				[
					174,
					4
				],
				[
					185,
					4
				],
				[
					196,
					4
				],
				[
					206,
					4
				],
				[
					218,
					4
				],
				[
					230,
					3
				],
				[
					243,
					3
				],
				[
					254,
					2
				],
				[
					264,
					1
				],
				[
					270,
					1
				],
				[
					275,
					1
				],
				[
					279,
					1
				],
				[
					282,
					1
				],
				[
					284,
					1
				],
				[
					285,
					0
				],
				[
					286,
					0
				],
				[
					287,
					0
				],
				[
					288,
					0
				],
				[
					290,
					0
				],
				[
					292,
					0
				],
				[
					294,
					0
				],
				[
					297,
					0
				],
				[
					299,
					0
				],
				[
					301,
					0
				],
				[
					302,
					0
				],
				[
					302,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 154,
			"versionNonce": 365639997,
			"isDeleted": false,
			"id": "09BGpSVRrczw_BKKqdcOV",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 225.85494244317647,
			"y": -2953.9841725880333,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 25,
			"height": 89,
			"seed": 1257587187,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458383755,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1
				],
				[
					3,
					5
				],
				[
					5,
					11
				],
				[
					9,
					21
				],
				[
					12,
					32
				],
				[
					15,
					42
				],
				[
					17,
					51
				],
				[
					19,
					60
				],
				[
					20,
					69
				],
				[
					21,
					77
				],
				[
					23,
					82
				],
				[
					24,
					86
				],
				[
					24,
					88
				],
				[
					25,
					89
				],
				[
					25,
					89
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 181,
			"versionNonce": 1787675923,
			"isDeleted": false,
			"id": "deDaRlZPECCR7PilHYGwe",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 222.85494244317647,
			"y": -2956.9841725880333,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 71,
			"height": 75,
			"seed": 295304637,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458383755,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					4,
					-1
				],
				[
					6,
					-2
				],
				[
					10,
					-3
				],
				[
					15,
					-4
				],
				[
					23,
					-4
				],
				[
					35,
					-4
				],
				[
					48,
					-3
				],
				[
					58,
					0
				],
				[
					63,
					3
				],
				[
					65,
					5
				],
				[
					65,
					8
				],
				[
					65,
					11
				],
				[
					62,
					13
				],
				[
					58,
					15
				],
				[
					53,
					17
				],
				[
					48,
					18
				],
				[
					42,
					20
				],
				[
					38,
					20
				],
				[
					37,
					20
				],
				[
					38,
					20
				],
				[
					40,
					21
				],
				[
					45,
					22
				],
				[
					53,
					25
				],
				[
					60,
					29
				],
				[
					67,
					34
				],
				[
					69,
					38
				],
				[
					71,
					43
				],
				[
					71,
					48
				],
				[
					71,
					54
				],
				[
					71,
					60
				],
				[
					69,
					66
				],
				[
					66,
					69
				],
				[
					62,
					70
				],
				[
					57,
					71
				],
				[
					52,
					71
				],
				[
					44,
					71
				],
				[
					36,
					71
				],
				[
					31,
					70
				],
				[
					28,
					70
				],
				[
					28,
					70
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 148,
			"versionNonce": 569051549,
			"isDeleted": false,
			"id": "Sp830c_yR_y9w2IEaoyvA",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 312.85494244317647,
			"y": -2924.9841725880333,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 12,
			"height": 17,
			"seed": 1700508157,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458383755,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1,
					0
				],
				[
					2,
					0
				],
				[
					4,
					3
				],
				[
					7,
					5
				],
				[
					9,
					9
				],
				[
					11,
					13
				],
				[
					12,
					15
				],
				[
					12,
					17
				],
				[
					12,
					17
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 140,
			"versionNonce": 223980211,
			"isDeleted": false,
			"id": "fCcWJ4MJchK9PHlzAcGjY",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 311.85494244317647,
			"y": -2942.9841725880333,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 88188019,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458383755,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 164,
			"versionNonce": 1316081149,
			"isDeleted": false,
			"id": "zdZKW1V7ebIIbyh6ttbVp",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 377.85494244317647,
			"y": -2959.9841725880333,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 40,
			"height": 50,
			"seed": 301219997,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458383755,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1,
					1
				],
				[
					-9,
					8
				],
				[
					-11,
					10
				],
				[
					-18,
					16
				],
				[
					-23,
					24
				],
				[
					-26,
					33
				],
				[
					-28,
					40
				],
				[
					-28,
					46
				],
				[
					-26,
					49
				],
				[
					-23,
					50
				],
				[
					-21,
					50
				],
				[
					-18,
					50
				],
				[
					-12,
					48
				],
				[
					-6,
					43
				],
				[
					0,
					38
				],
				[
					6,
					35
				],
				[
					9,
					33
				],
				[
					11,
					30
				],
				[
					12,
					29
				],
				[
					12,
					28
				],
				[
					11,
					28
				],
				[
					8,
					28
				],
				[
					5,
					28
				],
				[
					4,
					28
				],
				[
					4,
					28
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 140,
			"versionNonce": 1691868243,
			"isDeleted": false,
			"id": "tCLKIWqJHjSQYr9cjBZgD",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 377.85494244317647,
			"y": -2932.9841725880333,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 800092371,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458383755,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 154,
			"versionNonce": 1516308061,
			"isDeleted": false,
			"id": "XBmYeWpkHp1VVN6nhaeEZ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 190.85494244317647,
			"y": -2851.9841725880333,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 301,
			"height": 71,
			"seed": 2036254451,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458383755,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5,
					0
				],
				[
					18,
					-3
				],
				[
					40,
					-8
				],
				[
					74,
					-14
				],
				[
					112,
					-22
				],
				[
					147,
					-30
				],
				[
					184,
					-39
				],
				[
					218,
					-49
				],
				[
					250,
					-57
				],
				[
					273,
					-63
				],
				[
					287,
					-66
				],
				[
					296,
					-69
				],
				[
					300,
					-70
				],
				[
					301,
					-71
				],
				[
					301,
					-71
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 537,
			"versionNonce": 1021237747,
			"isDeleted": false,
			"id": "k8gUkxQJ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 126.85494244317647,
			"y": -2829.9841725880333,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 559.6595458984375,
			"height": 200,
			"seed": 1643923645,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458383755,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "The Time complexity will be O(n) due to the fact that \n    the time to complete will relate to the length of\nthe Linked list, into infinity.\n\nThe space complexity will be O(1) due to the fact that \nthe nodes will take up the same space for each node \ncreated.\n",
			"rawText": "The Time complexity will be O(n) due to the fact that \n    the time to complete will relate to the length of\nthe Linked list, into infinity.\n\nThe space complexity will be O(1) due to the fact that \nthe nodes will take up the same space for each node \ncreated.\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "The Time complexity will be O(n) due to the fact that \n    the time to complete will relate to the length of\nthe Linked list, into infinity.\n\nThe space complexity will be O(1) due to the fact that \nthe nodes will take up the same space for each node \ncreated.\n",
			"lineHeight": 1.25,
			"baseline": 193
		},
		{
			"type": "freedraw",
			"version": 120,
			"versionNonce": 680145597,
			"isDeleted": false,
			"id": "FR9rZKzMvC18GmMsLUWIf",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 278.4347153923952,
			"y": -2708.7263600880333,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 318262173,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682458383755,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.0001,
					0.0001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		}
	],
	"appState": {
		"theme": "light",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#000000",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "hachure",
		"currentItemStrokeWidth": 1,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 1012.4030791291539,
		"scrollY": 2941.365220126771,
		"zoom": {
			"value": 0.8316456618509293
		},
		"currentItemRoundness": "round",
		"gridSize": null,
		"colorPalette": {},
		"currentStrokeOptions": null,
		"previousGridSize": null
	},
	"files": {}
}
```
%%