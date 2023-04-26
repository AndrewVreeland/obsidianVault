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

public void insertAfter(int value, int newValue)
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

  public void appendNode(int value){
    Node newNode = new Node(value);
    if(head == null){
      head = newNode;
    }else{
      Node temp = head;
      while(temp.next != null){
        temp = temp.next
      }
      temp.next = newNode;
    }
  } ^N82BXQII

1 ^t9NlJVvX

2 ^2UfKC8Fu

3 ^rgVv98Uj

4 ^rxI39dtR

5 ^zcd6N6cC

Kth from end ^8arB6hgX

input(2) ^tWjEIG6O

Check to see if link is null;
check to see if input value is longer than the length of the link;
create temp node and equate it to the head;
create a prev temp node and equate it to head;
create a for loop and do temp.next to equate the value of the index, have this in an if else to make sure you don't step into null;
now create a while loop and do a temp.next and a prevTemp.next until the while loop breaks and then return the value of prevTemp

 ^hmy1bQnB

What if the input value does not exsist;
what if the linklist does not exsist;
what if k is not the last node;
any more edge cases? ^Hc1EREYv

NOT SURE WHAT BIG O IS HERE ^wJnO8ZeL

public void kthFromEnd(int k)throw IllegalArgumentException{
     if(head == null){
        throw new IllegalArgumentException("value not in list")
      }
Node temp = head;
Node prevTemp = head;
int i = 0;

while (temp.next != null && i < k) { 
    for (int j = 0; j < k; j++) { 
        if (temp.next == null) break; 
        temp = temp.next; 
    }
    i += k; // Update 'i' by adding 'k' after each iteration of the inner loop
}

while(temp != null){
prevTemp = prevTemp.next;
temp = temp.next;
}
return preTemp.value;
} ^uqpYut4e

not sure how to handle edge cases ^wVikPDML

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
			"version": 277,
			"versionNonce": 1324932541,
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
			"updated": 1682485574242,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 241,
			"versionNonce": 1608165523,
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
			"updated": 1682485574242,
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
			"version": 530,
			"versionNonce": 1558813853,
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
			"updated": 1682485582289,
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
			"version": 333,
			"versionNonce": 507387443,
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
			"updated": 1682485574242,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 241,
			"versionNonce": 48255613,
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
			"updated": 1682485574242,
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
			"version": 715,
			"versionNonce": 1915093245,
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
			"updated": 1682485582289,
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
			"version": 318,
			"versionNonce": 2005596893,
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
			"updated": 1682485574242,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 241,
			"versionNonce": 1457286515,
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
			"updated": 1682485574242,
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
			"version": 505,
			"versionNonce": 2098046397,
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
			"updated": 1682485582290,
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
			"version": 279,
			"versionNonce": 1584678675,
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
			"updated": 1682485574242,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 241,
			"versionNonce": 656779165,
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
			"updated": 1682485574242,
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
			"version": 266,
			"versionNonce": 85978291,
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
			"updated": 1682485574242,
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
			"version": 247,
			"versionNonce": 1319676925,
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
			"updated": 1682485574242,
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
			"version": 247,
			"versionNonce": 1317396051,
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
			"updated": 1682485574242,
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
			"version": 257,
			"versionNonce": 738993245,
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
			"updated": 1682485574242,
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
			"version": 248,
			"versionNonce": 92052467,
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
			"updated": 1682485574243,
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
			"version": 256,
			"versionNonce": 320966845,
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
			"updated": 1682485574243,
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
			"version": 267,
			"versionNonce": 1443538323,
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
			"updated": 1682485574243,
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
			"version": 260,
			"versionNonce": 1636462877,
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
			"updated": 1682485574243,
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
			"version": 270,
			"versionNonce": 661027635,
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
			"updated": 1682485574243,
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
			"version": 315,
			"versionNonce": 1152927101,
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
			"updated": 1682485574243,
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
			"version": 512,
			"versionNonce": 905354451,
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
			"updated": 1682485574243,
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
			"version": 251,
			"versionNonce": 1072467421,
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
			"updated": 1682485574243,
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
			"version": 277,
			"versionNonce": 1834060403,
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
			"updated": 1682485574243,
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
			"version": 249,
			"versionNonce": 1916324413,
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
			"updated": 1682485574243,
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
			"version": 247,
			"versionNonce": 37602323,
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
			"updated": 1682485574243,
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
			"version": 249,
			"versionNonce": 478050973,
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
			"updated": 1682485574243,
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
			"version": 246,
			"versionNonce": 1286719923,
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
			"updated": 1682485574243,
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
			"version": 274,
			"versionNonce": 1735335677,
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
			"updated": 1682485574243,
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
			"version": 274,
			"versionNonce": 1641290579,
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
			"updated": 1682485574243,
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
			"version": 277,
			"versionNonce": 1770796893,
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
			"updated": 1682485574243,
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
			"version": 260,
			"versionNonce": 1845180659,
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
			"updated": 1682485574243,
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
			"version": 264,
			"versionNonce": 1831289789,
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
			"updated": 1682485574243,
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
			"version": 274,
			"versionNonce": 1320002195,
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
			"updated": 1682485574243,
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
			"version": 274,
			"versionNonce": 1986118685,
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
			"updated": 1682485574243,
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
			"version": 270,
			"versionNonce": 1822545971,
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
			"updated": 1682485574243,
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
			"version": 251,
			"versionNonce": 153958525,
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
			"updated": 1682485574243,
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
			"version": 285,
			"versionNonce": 1438538195,
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
			"updated": 1682485574243,
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
			"version": 248,
			"versionNonce": 793452765,
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
			"updated": 1682485574243,
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
			"version": 267,
			"versionNonce": 387557235,
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
			"updated": 1682485574243,
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
			"version": 248,
			"versionNonce": 1045232957,
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
			"updated": 1682485574243,
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
			"version": 410,
			"versionNonce": 1459241235,
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
			"updated": 1682485574243,
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
			"version": 262,
			"versionNonce": 1570000285,
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
			"updated": 1682485574243,
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
			"version": 278,
			"versionNonce": 785819315,
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
			"updated": 1682485574243,
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
			"version": 247,
			"versionNonce": 1280479741,
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
			"updated": 1682485574243,
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
			"version": 225,
			"versionNonce": 1163221075,
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
			"updated": 1682485574243,
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
			"version": 249,
			"versionNonce": 1737050717,
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
			"updated": 1682485574243,
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
			"version": 266,
			"versionNonce": 676124147,
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
			"updated": 1682485574243,
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
			"version": 249,
			"versionNonce": 1879701181,
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
			"updated": 1682485574243,
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
			"version": 218,
			"versionNonce": 1724096403,
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
			"updated": 1682485574243,
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
			"version": 259,
			"versionNonce": 276174621,
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
			"updated": 1682485574243,
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
			"version": 260,
			"versionNonce": 1794127155,
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
			"updated": 1682485574243,
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
			"version": 245,
			"versionNonce": 591342461,
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
			"updated": 1682485574243,
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
			"version": 247,
			"versionNonce": 339285715,
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
			"updated": 1682485574243,
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
			"version": 245,
			"versionNonce": 950449117,
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
			"updated": 1682485574243,
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
			"version": 281,
			"versionNonce": 288670835,
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
			"updated": 1682485574243,
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
			"version": 351,
			"versionNonce": 1555968061,
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
			"updated": 1682485574243,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 330,
			"versionNonce": 2041167379,
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
			"updated": 1682485574243,
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
			"version": 155,
			"versionNonce": 493297821,
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
			"updated": 1682485574243,
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
			"version": 66,
			"versionNonce": 680428467,
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
			"updated": 1682485574243,
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
			"version": 47,
			"versionNonce": 1616273555,
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
			"updated": 1682485582290,
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
			"version": 48,
			"versionNonce": 1443468627,
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
			"updated": 1682485574243,
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
			"version": 35,
			"versionNonce": 419650909,
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
			"updated": 1682485574243,
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
			"version": 38,
			"versionNonce": 1903260403,
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
			"updated": 1682485574243,
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
			"version": 58,
			"versionNonce": 784968125,
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
			"updated": 1682485574243,
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
			"version": 34,
			"versionNonce": 994876563,
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
			"updated": 1682485574243,
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
			"version": 61,
			"versionNonce": 1657235997,
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
			"updated": 1682485574243,
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
			"version": 52,
			"versionNonce": 525439539,
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
			"updated": 1682485574243,
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
			"version": 64,
			"versionNonce": 1710104189,
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
			"updated": 1682485574243,
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
			"version": 61,
			"versionNonce": 1315361747,
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
			"updated": 1682485574244,
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
			"version": 64,
			"versionNonce": 1325352669,
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
			"updated": 1682485574244,
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
			"version": 60,
			"versionNonce": 413327731,
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
			"updated": 1682485574244,
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
			"version": 266,
			"versionNonce": 1619813181,
			"isDeleted": false,
			"id": "E50t6tWh",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -867.75,
			"y": -51.9088541666668,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 271.1597900390625,
			"height": 250,
			"seed": 1713812115,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 112,
			"versionNonce": 122436371,
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
			"updated": 1682485574244,
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
			"version": 139,
			"versionNonce": 251065245,
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
			"updated": 1682485574244,
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
			"version": 106,
			"versionNonce": 920215731,
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
			"updated": 1682485574244,
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
			"version": 98,
			"versionNonce": 1181775869,
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
			"updated": 1682485574244,
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
			"version": 122,
			"versionNonce": 1894830675,
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
			"updated": 1682485574244,
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
			"version": 98,
			"versionNonce": 1895460957,
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
			"updated": 1682485574244,
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
			"version": 63,
			"versionNonce": 107548659,
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
			"updated": 1682485574244,
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
			"version": 112,
			"versionNonce": 1013341373,
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
			"updated": 1682485574244,
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
			"version": 495,
			"versionNonce": 1766365587,
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
			"updated": 1682485574244,
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
			"version": 176,
			"versionNonce": 542489885,
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
			"updated": 1682485574244,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 155,
			"versionNonce": 113635123,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 277,
			"versionNonce": 607785341,
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
			"updated": 1682485574244,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 227,
			"versionNonce": 1632080083,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 265,
			"versionNonce": 1700059613,
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
			"updated": 1682485574244,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 234,
			"versionNonce": 1784938099,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 259,
			"versionNonce": 1555535421,
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
			"updated": 1682485574244,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 231,
			"versionNonce": 484554771,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 587,
			"versionNonce": 257107315,
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
			"updated": 1682485582291,
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
			"version": 726,
			"versionNonce": 1557632595,
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
			"boundElements": [],
			"updated": 1682485582292,
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
			"version": 721,
			"versionNonce": 1356289011,
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
			"boundElements": [],
			"updated": 1682485582292,
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
			"version": 222,
			"versionNonce": 1930104659,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 227,
			"versionNonce": 1651409757,
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
			"updated": 1682485574244,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 177,
			"versionNonce": 607366387,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 357,
			"versionNonce": 1240357053,
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
			"boundElements": [],
			"updated": 1682485582293,
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
			"version": 542,
			"versionNonce": 863910173,
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
			"boundElements": [],
			"updated": 1682485582293,
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
			"version": 187,
			"versionNonce": 2082541597,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 194,
			"versionNonce": 508382259,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 187,
			"versionNonce": 824378493,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 194,
			"versionNonce": 702238163,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 183,
			"versionNonce": 1856466141,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 176,
			"versionNonce": 1131944819,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 197,
			"versionNonce": 1681901885,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 193,
			"versionNonce": 1466578195,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 208,
			"versionNonce": 1397594525,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 185,
			"versionNonce": 86514355,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 120,
			"versionNonce": 1426218493,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 103,
			"versionNonce": 962088019,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 102,
			"versionNonce": 1616877149,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 132,
			"versionNonce": 131156467,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 125,
			"versionNonce": 272024253,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 131,
			"versionNonce": 1167692691,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 115,
			"versionNonce": 690578205,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 575,
			"versionNonce": 1659349299,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 101,
			"versionNonce": 1604908925,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 103,
			"versionNonce": 86117075,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 133,
			"versionNonce": 1576468445,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 125,
			"versionNonce": 1625241715,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 97,
			"versionNonce": 170196029,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 111,
			"versionNonce": 1407562259,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 98,
			"versionNonce": 202665117,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 106,
			"versionNonce": 1059846067,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 105,
			"versionNonce": 326553853,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 117,
			"versionNonce": 551061843,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 111,
			"versionNonce": 1573759325,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 98,
			"versionNonce": 1849812723,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 99,
			"versionNonce": 2087351741,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 121,
			"versionNonce": 770609299,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 125,
			"versionNonce": 1517205021,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 98,
			"versionNonce": 1368720947,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 109,
			"versionNonce": 46918269,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 694,
			"versionNonce": 1343997907,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"version": 75,
			"versionNonce": 641962717,
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
			"boundElements": [],
			"updated": 1682485574244,
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
			"type": "text",
			"version": 251,
			"versionNonce": 2140755315,
			"isDeleted": false,
			"id": "RTbc1zm9",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -188.17022705078125,
			"y": -1003.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 732.5194091796875,
			"height": 25,
			"seed": 918644531,
			"groupIds": [],
			"roundness": null,
			"boundElements": [
				{
					"id": "E-EyUxqDrm0T_ln0urJpk",
					"type": "arrow"
				}
			],
			"updated": 1682485574244,
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
			"version": 28,
			"versionNonce": 1634152253,
			"isDeleted": false,
			"id": "32yGixx14jsvkgXP2_ZtW",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -212.17022705078125,
			"y": -3227.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 35,
			"height": 49,
			"seed": 1291376787,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 14,
			"versionNonce": 794046227,
			"isDeleted": false,
			"id": "EkNPmFg4rLIO0kam5TYVC",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -167.17022705078125,
			"y": -3194.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 3,
			"height": 11,
			"seed": 922196541,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574244,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 8,
			"versionNonce": 1117274013,
			"isDeleted": false,
			"id": "myrTVuK_1aIrIvWukjxB6",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -169.17022705078125,
			"y": -3216.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 560714387,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"version": 50,
			"versionNonce": 29545651,
			"isDeleted": false,
			"id": "Oc_T_EkF6YmkMYFkBc0oL",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -129.17022705078125,
			"y": -3220.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 21,
			"height": 37,
			"seed": 76548221,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 27,
			"versionNonce": 268977149,
			"isDeleted": false,
			"id": "tVUZReUZRTJIQ7_tuxNUf",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -106.17022705078125,
			"y": -3213.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 22,
			"height": 24,
			"seed": 2088159635,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 39,
			"versionNonce": 109823571,
			"isDeleted": false,
			"id": "QrhcbXLE6Bn1GAkpjPPRK",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -51.17022705078125,
			"y": -3203.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 42,
			"height": 22,
			"seed": 367283059,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 17,
			"versionNonce": 1303952477,
			"isDeleted": false,
			"id": "lOssmeDAZ_S04RaPiiOtK",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -20.17022705078125,
			"y": -3228.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 3,
			"height": 31,
			"seed": 442130195,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "ellipse",
			"version": 25,
			"versionNonce": 344294387,
			"isDeleted": false,
			"id": "Gb5VNOhR3DbLNs1SGZIw0",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -407.17022705078125,
			"y": -3136.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 89,
			"height": 67,
			"seed": 1147843795,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
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
			"updated": 1682485574245,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 8,
			"versionNonce": 58403005,
			"isDeleted": false,
			"id": "S0hMYnUg",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -365.3464778980553,
			"y": -3116.1724521697492,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 5.4199981689453125,
			"height": 25,
			"seed": 559384595,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "1",
			"rawText": "1",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "Gb5VNOhR3DbLNs1SGZIw0",
			"originalText": "1",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "ellipse",
			"version": 48,
			"versionNonce": 1672908179,
			"isDeleted": false,
			"id": "t7TJGdAo-l2dPN5XWZOet",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -270.17022705078125,
			"y": -3131.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 69,
			"height": 72,
			"seed": 1708951773,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
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
			"updated": 1682485574245,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 8,
			"versionNonce": 1123092765,
			"isDeleted": false,
			"id": "kmG4Hbh1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -242.68540611890464,
			"y": -3108.440219122716,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 14.239990234375,
			"height": 25,
			"seed": 1704476701,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2",
			"rawText": "2",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "t7TJGdAo-l2dPN5XWZOet",
			"originalText": "2",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "ellipse",
			"version": 23,
			"versionNonce": 1733649203,
			"isDeleted": false,
			"id": "wBWUPa15bJZTozUUK_ggT",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -134.17022705078125,
			"y": -3129.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 86,
			"height": 72,
			"seed": 841892317,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
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
			"updated": 1682485574245,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 8,
			"versionNonce": 1837882749,
			"isDeleted": false,
			"id": "7UaSmko6",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -97.88581620039655,
			"y": -3106.440219122716,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 13.6199951171875,
			"height": 25,
			"seed": 466230355,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "3",
			"rawText": "3",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "wBWUPa15bJZTozUUK_ggT",
			"originalText": "3",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "ellipse",
			"version": 67,
			"versionNonce": 1741194451,
			"isDeleted": false,
			"id": "91srR5S_i6aUWMrfu2_iS",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 152.82977294921875,
			"y": -3129.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 94,
			"height": 76,
			"seed": 471952509,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
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
			"updated": 1682485574245,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 38,
			"versionNonce": 982328797,
			"isDeleted": false,
			"id": "iJ5qusjB",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 193.19576033696663,
			"y": -3104.354432685089,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 12.79998779296875,
			"height": 25,
			"seed": 1383738429,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "4",
			"rawText": "4",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "91srR5S_i6aUWMrfu2_iS",
			"originalText": "4",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 56,
			"versionNonce": 1838044637,
			"isDeleted": false,
			"id": "Y1df-0SkczbCWnadP7I8j",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -316.172028414342,
			"y": -3098.984453320155,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 45.01590520493602,
			"height": 1.9572132697794586,
			"seed": 458728979,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682485582294,
			"link": null,
			"locked": false,
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
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					45.01590520493602,
					1.9572132697794586
				]
			]
		},
		{
			"type": "arrow",
			"version": 51,
			"versionNonce": 307118749,
			"isDeleted": false,
			"id": "1hmz-YoG55m4fjpZkGcMU",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -200.17022964135896,
			"y": -3097.9843751195654,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 65.00001612484283,
			"height": 3.0000007442235983,
			"seed": 1566234419,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682485582294,
			"link": null,
			"locked": false,
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
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					65.00001612484283,
					3.0000007442235983
				]
			]
		},
		{
			"type": "arrow",
			"version": 107,
			"versionNonce": 1957432253,
			"isDeleted": false,
			"id": "eHUs-Yqi4Pa-AfnRvpYuQ",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -44.079842582370844,
			"y": -3092.30861636639,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 193.98093256007584,
			"height": 2.730375953910425,
			"seed": 1680826685,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682485582295,
			"link": null,
			"locked": false,
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
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					193.98093256007584,
					2.730375953910425
				]
			]
		},
		{
			"type": "text",
			"version": 30,
			"versionNonce": 702091933,
			"isDeleted": false,
			"id": "czYakp4V",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 69.82977294921875,
			"y": -3194.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 131.7598876953125,
			"height": 25,
			"seed": 1015837011,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Insert after!",
			"rawText": "Insert after!",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Insert after!",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "freedraw",
			"version": 36,
			"versionNonce": 1240248755,
			"isDeleted": false,
			"id": "z88CJX1apqOOuYfGj1T4c",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 62.82977294921875,
			"y": -3171.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 145,
			"height": 6,
			"seed": 1940781629,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 35,
			"versionNonce": 498513661,
			"isDeleted": false,
			"id": "rm4S8H8IVfkMx_SLBRfz8",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -216.17022705078125,
			"y": -3168.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 231,
			"height": 28,
			"seed": 903045181,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "ellipse",
			"version": 137,
			"versionNonce": 1198654291,
			"isDeleted": false,
			"id": "sjIQa0GIzei97ccXL8vfX",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -3.17022705078125,
			"y": -3034.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 97,
			"height": 78,
			"seed": 413640125,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
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
			"updated": 1682485574245,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 110,
			"versionNonce": 589352797,
			"isDeleted": false,
			"id": "v0rjeYWP",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 39.355101385889945,
			"y": -3008.5615394662755,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 12.3599853515625,
			"height": 25,
			"seed": 1222897907,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "5",
			"rawText": "5",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "sjIQa0GIzei97ccXL8vfX",
			"originalText": "5",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "text",
			"version": 19,
			"versionNonce": 932978931,
			"isDeleted": false,
			"id": "6GHh6vRF",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 280.82977294921875,
			"y": -3178.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 92.41990661621094,
			"height": 25,
			"seed": 754651891,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "input(3,5)",
			"rawText": "input(3,5)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "input(3,5)",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "arrow",
			"version": 57,
			"versionNonce": 2082472061,
			"isDeleted": false,
			"id": "fWZ3kM0OTqwYiTYHVyK9G",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -53.17455302811668,
			"y": -3073.988261047437,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 59.011014421099894,
			"height": 53.00989431047947,
			"seed": 2026115411,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682485582296,
			"link": null,
			"locked": false,
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
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					59.011014421099894,
					53.00989431047947
				]
			]
		},
		{
			"type": "arrow",
			"version": 65,
			"versionNonce": 1218767069,
			"isDeleted": false,
			"id": "21uNE0M4GY_aRhDGJtb8J",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 89.82068750357685,
			"y": -3015.9792644368267,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 80.01609177307317,
			"height": 45.00905162235358,
			"seed": 267824893,
			"groupIds": [],
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1682485582296,
			"link": null,
			"locked": false,
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
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					80.01609177307317,
					-45.00905162235358
				]
			]
		},
		{
			"type": "freedraw",
			"version": 18,
			"versionNonce": 363879453,
			"isDeleted": false,
			"id": "fHzsalqlZkgSjp_Boa-f1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 76.82977294921875,
			"y": -3115.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 47,
			"height": 47,
			"seed": 857801267,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 19,
			"versionNonce": 556318771,
			"isDeleted": false,
			"id": "sNvQRu-fyqBx3dAQRorXC",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 30.82977294921875,
			"y": -3126.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 49,
			"height": 64,
			"seed": 903219603,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 13,
			"versionNonce": 1927860349,
			"isDeleted": false,
			"id": "lNU2VErlGPWinAFTtsLAg",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 171.82977294921875,
			"y": -3147.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 12,
			"seed": 562274237,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 22,
			"versionNonce": 690504147,
			"isDeleted": false,
			"id": "aoi7uuHgC4Sn5_qNa2cmz",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 157.82977294921875,
			"y": -3152.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 29,
			"height": 2,
			"seed": 961520915,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 42,
			"versionNonce": 231979229,
			"isDeleted": false,
			"id": "Ex8BEUDTZjyqtRzV4iym4",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 190.82977294921875,
			"y": -3143.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 20,
			"height": 13,
			"seed": 1618175923,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 43,
			"versionNonce": 889622387,
			"isDeleted": false,
			"id": "D7XTpl8ETvvotpNN4Ez6p",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 221.82977294921875,
			"y": -3148.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 20,
			"height": 21,
			"seed": 1448016531,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 15,
			"versionNonce": 1879217469,
			"isDeleted": false,
			"id": "mD1WvX-urozcKNKSsu9j4",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 252.82977294921875,
			"y": -3144.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 16,
			"seed": 336431933,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 24,
			"versionNonce": 1997154579,
			"isDeleted": false,
			"id": "Ha3CILiBy1QDAgjJibXRX",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 252.82977294921875,
			"y": -3149.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 9,
			"height": 10,
			"seed": 787760947,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 15,
			"versionNonce": 1960240541,
			"isDeleted": false,
			"id": "MdCVTN6HLWKMhB5u39ODu",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -127.17022705078125,
			"y": -3150.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 21,
			"seed": 102265715,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 15,
			"versionNonce": 346656435,
			"isDeleted": false,
			"id": "KShb-8DHa7UHU9Z-rFzoh",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -141.17022705078125,
			"y": -3150.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 26,
			"height": 4,
			"seed": 362908445,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 37,
			"versionNonce": 260188669,
			"isDeleted": false,
			"id": "4m7hjGNLAMy91lS53VxH-",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -116.17022705078125,
			"y": -3140.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 14,
			"height": 18,
			"seed": 593486163,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 41,
			"versionNonce": 1082867795,
			"isDeleted": false,
			"id": "ez7MIstHCNlkwUwHllkvu",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -100.17022705078125,
			"y": -3141.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 27,
			"height": 20,
			"seed": 604698461,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 14,
			"versionNonce": 1359340125,
			"isDeleted": false,
			"id": "eI-uwZkU5R8nr4xr0vU_D",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -64.17022705078125,
			"y": -3157.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 2,
			"height": 21,
			"seed": 2085540403,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 22,
			"versionNonce": 344309235,
			"isDeleted": false,
			"id": "IPhyXSmLjStlSOECH1gNe",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -61.17022705078125,
			"y": -3161.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 13,
			"height": 13,
			"seed": 1202066003,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 44,
			"versionNonce": 775130813,
			"isDeleted": false,
			"id": "lh8fGLcYX6U_faohtNisW",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -40.17022705078125,
			"y": -3148.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 15,
			"height": 32,
			"seed": 553708787,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 20,
			"versionNonce": 731875219,
			"isDeleted": false,
			"id": "ZjRrw6nnUhJlAzAK7vdil",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -16.17022705078125,
			"y": -3144.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 6,
			"height": 20,
			"seed": 1766233459,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 32,
			"versionNonce": 95203101,
			"isDeleted": false,
			"id": "g-jXaiuz4cf3Mi8wZSCN5",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -4.17022705078125,
			"y": -3153.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 8,
			"height": 19,
			"seed": 1427354227,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 27,
			"versionNonce": 2081365299,
			"isDeleted": false,
			"id": "Huudc5as1u6NRZeZsOrvI",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4.82977294921875,
			"y": -3156.984375,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 16,
			"height": 14,
			"seed": 1347181875,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 78,
			"versionNonce": 1709359997,
			"isDeleted": false,
			"id": "ywCeGsYbdtEA9fWeLkMRO",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 157.82977294921875,
			"y": 399.015625,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 318262173,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
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
			"version": 90,
			"versionNonce": 1899691731,
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
			"updated": 1682485574245,
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
			"version": 117,
			"versionNonce": 320293853,
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
			"updated": 1682485574245,
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
			"version": 84,
			"versionNonce": 1169796211,
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
			"updated": 1682485574245,
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
			"version": 76,
			"versionNonce": 1297860669,
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
			"updated": 1682485574245,
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
			"version": 100,
			"versionNonce": 491890195,
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
			"updated": 1682485574245,
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
			"version": 76,
			"versionNonce": 1452390557,
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
			"updated": 1682485574245,
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
			"version": 90,
			"versionNonce": 1593404339,
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
			"updated": 1682485574245,
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
			"version": 473,
			"versionNonce": 946511101,
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
			"updated": 1682485574245,
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
			"version": 56,
			"versionNonce": 1322745171,
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
			"updated": 1682485574245,
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
			"version": 1095,
			"versionNonce": 1248327005,
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
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "public void insertAfter(int value, int newValue)\nthrow IllegalArgumentException{   \n if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n}\nNode temp = head;\nNode prevNode = null;\nNode newNode = new Node(newValue)\n\nif (temp.value == value){\n    newNode.next = temp;\n    head = newNode;\n    return;\n}\n\nwhile(temp.next != null){\nprevTemp = temp;\ntemp = temp.next;\nif(prevTemp.value == value){\nnewNode.next = temp;\nprevTemp.next = newNode;\nreturn;\n}\n}\n\n}",
			"rawText": "public void insertAfter(int value, int newValue)\nthrow IllegalArgumentException{   \n if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n}\nNode temp = head;\nNode prevNode = null;\nNode newNode = new Node(newValue)\n\nif (temp.value == value){\n    newNode.next = temp;\n    head = newNode;\n    return;\n}\n\nwhile(temp.next != null){\nprevTemp = temp;\ntemp = temp.next;\nif(prevTemp.value == value){\nnewNode.next = temp;\nprevTemp.next = newNode;\nreturn;\n}\n}\n\n}",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "public void insertAfter(int value, int newValue)\nthrow IllegalArgumentException{   \n if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n}\nNode temp = head;\nNode prevNode = null;\nNode newNode = new Node(newValue)\n\nif (temp.value == value){\n    newNode.next = temp;\n    head = newNode;\n    return;\n}\n\nwhile(temp.next != null){\nprevTemp = temp;\ntemp = temp.next;\nif(prevTemp.value == value){\nnewNode.next = temp;\nprevTemp.next = newNode;\nreturn;\n}\n}\n\n}",
			"lineHeight": 1.25,
			"baseline": 643
		},
		{
			"type": "arrow",
			"version": 231,
			"versionNonce": 1749179123,
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
			"updated": 1682485574245,
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
			"version": 329,
			"versionNonce": 2010857917,
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
			"updated": 1682485574245,
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
			"version": 121,
			"versionNonce": 2009105555,
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
			"updated": 1682485574245,
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
			"version": 104,
			"versionNonce": 1172701725,
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
			"updated": 1682485574245,
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
			"version": 103,
			"versionNonce": 1963489843,
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
			"updated": 1682485574245,
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
			"version": 133,
			"versionNonce": 427406973,
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
			"updated": 1682485574245,
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
			"version": 126,
			"versionNonce": 486587347,
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
			"updated": 1682485574245,
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
			"version": 132,
			"versionNonce": 1029168861,
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
			"updated": 1682485574245,
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
			"version": 157,
			"versionNonce": 1270860147,
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
			"updated": 1682485574245,
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
			"version": 184,
			"versionNonce": 672267069,
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
			"updated": 1682485574245,
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
			"version": 151,
			"versionNonce": 378282771,
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
			"updated": 1682485574245,
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
			"version": 143,
			"versionNonce": 34179997,
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
			"updated": 1682485574245,
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
			"version": 167,
			"versionNonce": 635193523,
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
			"updated": 1682485574245,
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
			"version": 143,
			"versionNonce": 1802506237,
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
			"updated": 1682485574245,
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
			"version": 157,
			"versionNonce": 1331083859,
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
			"updated": 1682485574245,
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
			"version": 540,
			"versionNonce": 38209629,
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
			"updated": 1682485574245,
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
			"version": 123,
			"versionNonce": 1876031475,
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
			"updated": 1682485574245,
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
			"version": 109,
			"versionNonce": 677377213,
			"isDeleted": false,
			"id": "N82BXQII",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -568.1568968944899,
			"y": 397.2717408459607,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 367.67974853515625,
			"height": 300,
			"seed": 1220589789,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "  public void appendNode(int value){\n    Node newNode = new Node(value);\n    if(head == null){\n      head = newNode;\n    }else{\n      Node temp = head;\n      while(temp.next != null){\n        temp = temp.next\n      }\n      temp.next = newNode;\n    }\n  }",
			"rawText": "  public void appendNode(int value){\n    Node newNode = new Node(value);\n    if(head == null){\n      head = newNode;\n    }else{\n      Node temp = head;\n      while(temp.next != null){\n        temp = temp.next\n      }\n      temp.next = newNode;\n    }\n  }",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "  public void appendNode(int value){\n    Node newNode = new Node(value);\n    if(head == null){\n      head = newNode;\n    }else{\n      Node temp = head;\n      while(temp.next != null){\n        temp = temp.next\n      }\n      temp.next = newNode;\n    }\n  }",
			"lineHeight": 1.25,
			"baseline": 293
		},
		{
			"id": "kLogV9NeOkkhuzjPRh2Kc",
			"type": "freedraw",
			"x": -534.9618937174481,
			"y": 911.2660787563137,
			"width": 50,
			"height": 106,
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
			"seed": 70169341,
			"version": 29,
			"versionNonce": 89424275,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
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
					4
				],
				[
					0,
					16
				],
				[
					2,
					28
				],
				[
					6,
					42
				],
				[
					10,
					54
				],
				[
					12,
					68
				],
				[
					14,
					76
				],
				[
					16,
					86
				],
				[
					18,
					94
				],
				[
					20,
					100
				],
				[
					20,
					102
				],
				[
					22,
					102
				],
				[
					24,
					100
				],
				[
					24,
					92
				],
				[
					28,
					80
				],
				[
					32,
					66
				],
				[
					34,
					54
				],
				[
					40,
					40
				],
				[
					42,
					28
				],
				[
					46,
					14
				],
				[
					48,
					4
				],
				[
					50,
					-2
				],
				[
					50,
					-4
				],
				[
					50,
					-4
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				50,
				-4
			]
		},
		{
			"id": "s9WfZBHMjcmOEqcEIieeJ",
			"type": "freedraw",
			"x": -462.9618937174481,
			"y": 973.2660787563137,
			"width": 2,
			"height": 30,
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
			"seed": 1664151667,
			"version": 12,
			"versionNonce": 157046045,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
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
					4
				],
				[
					0,
					12
				],
				[
					2,
					16
				],
				[
					2,
					24
				],
				[
					2,
					28
				],
				[
					2,
					30
				],
				[
					2,
					30
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				2,
				30
			]
		},
		{
			"id": "rCGypcOcuszYHCPb3pPL7",
			"type": "freedraw",
			"x": -462.9618937174481,
			"y": 945.2660787563137,
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
			"seed": 1848461459,
			"version": 5,
			"versionNonce": 152360755,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
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
			"id": "t8z4fmzAdcy87qTQAP5s8",
			"type": "freedraw",
			"x": -402.9618937174481,
			"y": 951.2660787563137,
			"width": 32,
			"height": 44,
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
			"seed": 1151054461,
			"version": 43,
			"versionNonce": 1621993853,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-2
				],
				[
					-2,
					-2
				],
				[
					-4,
					-2
				],
				[
					-6,
					-2
				],
				[
					-8,
					-2
				],
				[
					-10,
					-2
				],
				[
					-12,
					-2
				],
				[
					-14,
					-2
				],
				[
					-14,
					2
				],
				[
					-14,
					4
				],
				[
					-14,
					6
				],
				[
					-14,
					10
				],
				[
					-14,
					12
				],
				[
					-14,
					14
				],
				[
					-12,
					16
				],
				[
					-10,
					16
				],
				[
					-8,
					18
				],
				[
					-6,
					18
				],
				[
					-2,
					20
				],
				[
					0,
					20
				],
				[
					2,
					20
				],
				[
					2,
					22
				],
				[
					4,
					22
				],
				[
					6,
					22
				],
				[
					6,
					24
				],
				[
					6,
					26
				],
				[
					6,
					28
				],
				[
					6,
					30
				],
				[
					4,
					34
				],
				[
					2,
					38
				],
				[
					-2,
					40
				],
				[
					-4,
					42
				],
				[
					-6,
					42
				],
				[
					-8,
					42
				],
				[
					-14,
					42
				],
				[
					-20,
					42
				],
				[
					-24,
					42
				],
				[
					-26,
					42
				],
				[
					-26,
					42
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-26,
				42
			]
		},
		{
			"id": "qEAGdH6tZQsDmcLa1by2p",
			"type": "freedraw",
			"x": -364.9618937174481,
			"y": 947.2660787563137,
			"width": 22,
			"height": 42,
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
			"seed": 66058323,
			"version": 26,
			"versionNonce": 158955731,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2,
					0
				],
				[
					-2,
					2
				],
				[
					-4,
					8
				],
				[
					-4,
					14
				],
				[
					-4,
					20
				],
				[
					-4,
					26
				],
				[
					-2,
					34
				],
				[
					2,
					40
				],
				[
					4,
					42
				],
				[
					8,
					42
				],
				[
					10,
					42
				],
				[
					12,
					42
				],
				[
					14,
					42
				],
				[
					14,
					40
				],
				[
					16,
					32
				],
				[
					16,
					26
				],
				[
					16,
					18
				],
				[
					16,
					10
				],
				[
					18,
					4
				],
				[
					18,
					2
				],
				[
					18,
					0
				],
				[
					18,
					0
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				18,
				0
			]
		},
		{
			"id": "J6Z4m5O_NQ5pujRITSxNL",
			"type": "freedraw",
			"x": -304.961893717448,
			"y": 973.2660787563137,
			"width": 60.000000000000114,
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
			"seed": 772895699,
			"version": 45,
			"versionNonce": 2140500445,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
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
					4,
					0
				],
				[
					6,
					2
				],
				[
					6,
					4
				],
				[
					6,
					6
				],
				[
					6,
					10
				],
				[
					4,
					12
				],
				[
					2,
					14
				],
				[
					-2,
					16
				],
				[
					-4,
					16
				],
				[
					-6,
					16
				],
				[
					-12,
					14
				],
				[
					-14,
					10
				],
				[
					-16.000000000000114,
					4
				],
				[
					-16.000000000000114,
					-2
				],
				[
					-16.000000000000114,
					-6
				],
				[
					-16.000000000000114,
					-10
				],
				[
					-14,
					-12
				],
				[
					-10,
					-14
				],
				[
					-2,
					-16
				],
				[
					6,
					-16
				],
				[
					12,
					-16
				],
				[
					16,
					-16
				],
				[
					18,
					-16
				],
				[
					18,
					-14
				],
				[
					20,
					-12
				],
				[
					20,
					-8
				],
				[
					20,
					-2
				],
				[
					20,
					4
				],
				[
					18,
					8
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
					20,
					14
				],
				[
					22,
					14
				],
				[
					26,
					14
				],
				[
					34,
					14
				],
				[
					38,
					10
				],
				[
					42,
					8
				],
				[
					42,
					6
				],
				[
					44,
					4
				],
				[
					44,
					4
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				44,
				4
			]
		},
		{
			"id": "UO7pGjADz1TdJKvROqVv0",
			"type": "freedraw",
			"x": -248.961893717448,
			"y": 925.2660787563137,
			"width": 4,
			"height": 54,
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
			"seed": 1571431101,
			"version": 14,
			"versionNonce": 68740723,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2,
					2
				],
				[
					2,
					6
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
					2,
					30
				],
				[
					0,
					38
				],
				[
					-2,
					46
				],
				[
					-2,
					52
				],
				[
					-2,
					54
				],
				[
					-2,
					54
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-2,
				54
			]
		},
		{
			"id": "xWi11ZndMCfLa0AjubbLW",
			"type": "freedraw",
			"x": -600.9618937174481,
			"y": 1031.2660787563136,
			"width": 432.0000000000001,
			"height": 41.999999999999886,
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
			"seed": 1256337661,
			"version": 28,
			"versionNonce": 321203773,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					4,
					0
				],
				[
					22,
					-4
				],
				[
					50,
					-9.999999999999886
				],
				[
					90,
					-15.999999999999886
				],
				[
					140,
					-21.999999999999886
				],
				[
					192,
					-27.999999999999886
				],
				[
					236,
					-31.999999999999886
				],
				[
					270,
					-35.999999999999886
				],
				[
					300.0000000000001,
					-39.999999999999886
				],
				[
					320.0000000000001,
					-39.999999999999886
				],
				[
					340.0000000000001,
					-39.999999999999886
				],
				[
					354.0000000000001,
					-39.999999999999886
				],
				[
					366.0000000000001,
					-39.999999999999886
				],
				[
					376.0000000000001,
					-39.999999999999886
				],
				[
					386.0000000000001,
					-39.999999999999886
				],
				[
					400.0000000000001,
					-39.999999999999886
				],
				[
					410.0000000000001,
					-39.999999999999886
				],
				[
					420.0000000000001,
					-39.999999999999886
				],
				[
					424.0000000000001,
					-39.999999999999886
				],
				[
					428.0000000000001,
					-39.999999999999886
				],
				[
					430.0000000000001,
					-39.999999999999886
				],
				[
					432.0000000000001,
					-39.999999999999886
				],
				[
					432.0000000000001,
					-41.999999999999886
				],
				[
					432.0000000000001,
					-41.999999999999886
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				432.0000000000001,
				-41.999999999999886
			]
		},
		{
			"id": "jGyZnsBtsNzWdZyMA8HiV",
			"type": "ellipse",
			"x": -902.9618937174481,
			"y": 1087.2660787563138,
			"width": 132,
			"height": 134,
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
			"seed": 897353181,
			"version": 85,
			"versionNonce": 2142871571,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "t9NlJVvX"
				},
				{
					"id": "XEGvZa-FUwOyQYCsqlScY",
					"type": "arrow"
				}
			],
			"updated": 1682485574245,
			"link": null,
			"locked": false
		},
		{
			"id": "t9NlJVvX",
			"type": "text",
			"x": -839.8409403602329,
			"y": 1141.8899244168151,
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
			"seed": 346877437,
			"version": 38,
			"versionNonce": 708730525,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"text": "1",
			"rawText": "1",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "jGyZnsBtsNzWdZyMA8HiV",
			"originalText": "1",
			"lineHeight": 1.25
		},
		{
			"id": "uIbCI-bPeNrKxbXRC5Hlg",
			"type": "ellipse",
			"x": -610.9618937174481,
			"y": 1083.2660787563138,
			"width": 152,
			"height": 140,
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
			"seed": 521061139,
			"version": 78,
			"versionNonce": 1716659635,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "2UfKC8Fu"
				},
				{
					"id": "XEGvZa-FUwOyQYCsqlScY",
					"type": "arrow"
				},
				{
					"id": "HO18kUoAszJURlaAw_E6A",
					"type": "arrow"
				}
			],
			"updated": 1682485574245,
			"link": null,
			"locked": false
		},
		{
			"id": "2UfKC8Fu",
			"type": "text",
			"x": -542.3220042048132,
			"y": 1140.7686040732556,
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
			"seed": 1799625011,
			"version": 34,
			"versionNonce": 2073199357,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"text": "2",
			"rawText": "2",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "uIbCI-bPeNrKxbXRC5Hlg",
			"originalText": "2",
			"lineHeight": 1.25
		},
		{
			"id": "kRtWFw-uLlfX0DVsDxTiF",
			"type": "ellipse",
			"x": -306.961893717448,
			"y": 1083.2660787563138,
			"width": 178,
			"height": 138,
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
			"seed": 356876211,
			"version": 51,
			"versionNonce": 1805851485,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "rgVv98Uj"
				},
				{
					"id": "HO18kUoAszJURlaAw_E6A",
					"type": "arrow"
				},
				{
					"id": "wMEG2ZaF7rbadbP0PPbfJ",
					"type": "arrow"
				}
			],
			"updated": 1682485574245,
			"link": null,
			"locked": false
		},
		{
			"id": "rgVv98Uj",
			"type": "text",
			"x": -224.70439480164447,
			"y": 1139.975710854442,
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
			"seed": 1037068211,
			"version": 6,
			"versionNonce": 1748276467,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574245,
			"link": null,
			"locked": false,
			"text": "3",
			"rawText": "3",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "kRtWFw-uLlfX0DVsDxTiF",
			"originalText": "3",
			"lineHeight": 1.25
		},
		{
			"id": "ocDdSJ0tEVFaNZhrZS66_",
			"type": "ellipse",
			"x": 19.038106282552008,
			"y": 1079.2660787563138,
			"width": 228,
			"height": 158,
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
			"seed": 1234230685,
			"version": 47,
			"versionNonce": 1388423101,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "rxI39dtR"
				},
				{
					"id": "wMEG2ZaF7rbadbP0PPbfJ",
					"type": "arrow"
				},
				{
					"id": "IKCtRP_Td0_tbOVFHPzKL",
					"type": "arrow"
				}
			],
			"updated": 1682485574245,
			"link": null,
			"locked": false
		},
		{
			"id": "rxI39dtR",
			"type": "text",
			"x": 126.52793933080122,
			"y": 1145.9046430425765,
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
			"seed": 1809008157,
			"version": 24,
			"versionNonce": 1901821587,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"text": "4",
			"rawText": "4",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "ocDdSJ0tEVFaNZhrZS66_",
			"originalText": "4",
			"lineHeight": 1.25
		},
		{
			"id": "kX4WUsuFyPthWcxD3z-ZA",
			"type": "ellipse",
			"x": 415.038106282552,
			"y": 1085.2660787563138,
			"width": 270,
			"height": 192,
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
			"seed": 771621427,
			"version": 65,
			"versionNonce": 51357725,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "zcd6N6cC"
				},
				{
					"id": "IKCtRP_Td0_tbOVFHPzKL",
					"type": "arrow"
				}
			],
			"updated": 1682485574246,
			"link": null,
			"locked": false
		},
		{
			"id": "zcd6N6cC",
			"type": "text",
			"x": 543.8986981465869,
			"y": 1168.8838277624052,
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
			"seed": 1482071827,
			"version": 29,
			"versionNonce": 892613683,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"text": "5",
			"rawText": "5",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "center",
			"verticalAlign": "middle",
			"baseline": 18,
			"containerId": "kX4WUsuFyPthWcxD3z-ZA",
			"originalText": "5",
			"lineHeight": 1.25
		},
		{
			"id": "XEGvZa-FUwOyQYCsqlScY",
			"type": "arrow",
			"x": -764.9618966630629,
			"y": 1159.2660789134134,
			"width": 150.00001312489587,
			"height": 8.000000699994416,
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
			"seed": 354282739,
			"version": 37,
			"versionNonce": 823924125,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485582297,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					150.00001312489587,
					-8.000000699994416
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "jGyZnsBtsNzWdZyMA8HiV",
				"gap": 6.168697471497623,
				"focus": 0.13175858580855065
			},
			"endBinding": {
				"elementId": "uIbCI-bPeNrKxbXRC5Hlg",
				"gap": 4.029201185968773,
				"focus": 0.08937410095294246
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "HO18kUoAszJURlaAw_E6A",
			"type": "arrow",
			"x": -452.9620229311858,
			"y": 1147.2660787563138,
			"width": 145.23001464665174,
			"height": 0,
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
			"seed": 1527828627,
			"version": 27,
			"versionNonce": 1103041117,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485582298,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					145.23001464665174,
					0
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "uIbCI-bPeNrKxbXRC5Hlg",
				"gap": 6.254889816138288,
				"focus": -0.08571428571428572
			},
			"endBinding": {
				"elementId": "kRtWFw-uLlfX0DVsDxTiF",
				"gap": 1,
				"focus": 0.07246376811594202
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "wMEG2ZaF7rbadbP0PPbfJ",
			"type": "arrow",
			"x": -126.96204339525258,
			"y": 1149.2660787563138,
			"width": 145.7302013372632,
			"height": 0,
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
			"seed": 180363837,
			"version": 36,
			"versionNonce": 500817693,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485582298,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					145.7302013372632,
					0
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "kRtWFw-uLlfX0DVsDxTiF",
				"gap": 2.0810074597838337,
				"focus": -0.043478260869565216
			},
			"endBinding": {
				"elementId": "ocDdSJ0tEVFaNZhrZS66_",
				"gap": 1,
				"focus": 0.11392405063291139
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "IKCtRP_Td0_tbOVFHPzKL",
			"type": "arrow",
			"x": 251.0376216165696,
			"y": 1161.2660728457531,
			"width": 164.0064707936242,
			"height": 2.00007891211726,
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
			"seed": 1335199805,
			"version": 24,
			"versionNonce": 95976413,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485582299,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					164.0064707936242,
					2.00007891211726
				]
			],
			"lastCommittedPoint": null,
			"startBinding": {
				"elementId": "ocDdSJ0tEVFaNZhrZS66_",
				"gap": 4.076527503147986,
				"focus": 0.019756126028635995
			},
			"endBinding": {
				"elementId": "kX4WUsuFyPthWcxD3z-ZA",
				"gap": 2.315017366064012,
				"focus": 0.17032556508798932
			},
			"startArrowhead": null,
			"endArrowhead": "arrow"
		},
		{
			"id": "8arB6hgX",
			"type": "text",
			"x": -816.961893717448,
			"y": 953.2660787563133,
			"width": 127.15989685058594,
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
			"seed": 885586515,
			"version": 141,
			"versionNonce": 563437885,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"text": "Kth from end",
			"rawText": "Kth from end",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "Kth from end",
			"lineHeight": 1.25
		},
		{
			"id": "iKRRjBn4TOSCTDcN0bXjm",
			"type": "freedraw",
			"x": -842.6761794317335,
			"y": 978.8511603413945,
			"width": 188,
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
			"seed": 769637619,
			"version": 23,
			"versionNonce": 1977228563,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.3333333333332575,
					0
				],
				[
					4,
					0
				],
				[
					13.333333333333258,
					0
				],
				[
					26.66666666666663,
					0
				],
				[
					44,
					1.333333333333485
				],
				[
					62.66666666666663,
					1.333333333333485
				],
				[
					81.33333333333326,
					2.6666666666667425
				],
				[
					100,
					4
				],
				[
					116,
					4
				],
				[
					133.33333333333326,
					4
				],
				[
					146.66666666666663,
					4
				],
				[
					160,
					4
				],
				[
					169.33333333333326,
					4
				],
				[
					177.33333333333326,
					4
				],
				[
					182.66666666666663,
					4
				],
				[
					184,
					4
				],
				[
					186.66666666666663,
					4
				],
				[
					188,
					4
				],
				[
					188,
					4
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				188,
				4
			]
		},
		{
			"id": "vImOmcWfmbJO3dq3oQr1p",
			"type": "freedraw",
			"x": -809.9640582196126,
			"y": 1287.1986461888805,
			"width": 10.909090909090878,
			"height": 65.4545454545455,
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
			"seed": 212055645,
			"version": 13,
			"versionNonce": 492503731,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181818699,
					0
				],
				[
					-1.8181818181818699,
					5.454545454545496
				],
				[
					-3.636363636363626,
					14.545454545454504
				],
				[
					-5.454545454545382,
					25.454545454545496
				],
				[
					-7.272727272727252,
					34.545454545454504
				],
				[
					-9.090909090909122,
					45.454545454545496
				],
				[
					-10.909090909090878,
					56.36363636363649
				],
				[
					-10.909090909090878,
					61.81818181818198
				],
				[
					-10.909090909090878,
					65.4545454545455
				],
				[
					-10.909090909090878,
					65.4545454545455
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-10.909090909090878,
				65.4545454545455
			]
		},
		{
			"id": "tzXZJylLOE5ToNCEOvZKc",
			"type": "freedraw",
			"x": -866.327694583249,
			"y": 1289.0168280070625,
			"width": 130.909090909091,
			"height": 3.6363636363635123,
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
			"seed": 2126548125,
			"version": 17,
			"versionNonce": 1003615741,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1.8181818181819835
				],
				[
					1.8181818181817562,
					-1.8181818181819835
				],
				[
					5.454545454545496,
					-1.8181818181819835
				],
				[
					10.909090909090992,
					-1.8181818181819835
				],
				[
					18.181818181818244,
					-3.6363636363635123
				],
				[
					30.90909090909099,
					-3.6363636363635123
				],
				[
					47.27272727272725,
					-3.6363636363635123
				],
				[
					67.27272727272725,
					-3.6363636363635123
				],
				[
					87.27272727272725,
					-3.6363636363635123
				],
				[
					105.4545454545455,
					-3.6363636363635123
				],
				[
					118.18181818181824,
					-3.6363636363635123
				],
				[
					127.27272727272725,
					-3.6363636363635123
				],
				[
					130.909090909091,
					-3.6363636363635123
				],
				[
					130.909090909091,
					-3.6363636363635123
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				130.909090909091,
				-3.6363636363635123
			]
		},
		{
			"id": "2he15HYYKXAz7Ev98rzUn",
			"type": "freedraw",
			"x": -713.6004218559763,
			"y": 1349.0168280070625,
			"width": 61.81818181818187,
			"height": 52.727272727272975,
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
			"seed": 790912925,
			"version": 33,
			"versionNonce": 451818579,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181817562,
					0
				],
				[
					-3.636363636363626,
					0
				],
				[
					-5.454545454545496,
					0
				],
				[
					-7.272727272727252,
					0
				],
				[
					-10.909090909090878,
					0
				],
				[
					-14.545454545454504,
					-1.8181818181819835
				],
				[
					-25.454545454545496,
					-7.272727272727479
				],
				[
					-30.909090909090878,
					-10.909090909090992
				],
				[
					-38.181818181818244,
					-16.363636363636488
				],
				[
					-43.636363636363626,
					-20
				],
				[
					-45.454545454545496,
					-27.27272727272748
				],
				[
					-45.454545454545496,
					-34.545454545454504
				],
				[
					-41.818181818181756,
					-41.81818181818198
				],
				[
					-32.72727272727275,
					-49.09090909090901
				],
				[
					-20,
					-50.90909090909099
				],
				[
					-7.272727272727252,
					-52.727272727272975
				],
				[
					1.8181818181817562,
					-52.727272727272975
				],
				[
					7.272727272727252,
					-49.09090909090901
				],
				[
					10.909090909090992,
					-45.454545454545496
				],
				[
					14.545454545454504,
					-41.81818181818198
				],
				[
					16.363636363636374,
					-36.36363636363649
				],
				[
					16.363636363636374,
					-32.727272727272975
				],
				[
					16.363636363636374,
					-27.27272727272748
				],
				[
					16.363636363636374,
					-21.818181818181984
				],
				[
					12.727272727272748,
					-14.545454545454504
				],
				[
					9.090909090909122,
					-10.909090909090992
				],
				[
					5.454545454545496,
					-7.272727272727479
				],
				[
					3.636363636363626,
					-3.6363636363635123
				],
				[
					0,
					0
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				3.636363636363626,
				-3.6363636363635123
			]
		},
		{
			"id": "Stbw0BbilhIfu2O5wLuoZ",
			"type": "freedraw",
			"x": -655.418603674158,
			"y": 1279.9259189161535,
			"width": 5.454545454545496,
			"height": 65.4545454545455,
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
			"seed": 891487645,
			"version": 12,
			"versionNonce": 2038181469,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					7.272727272727025
				],
				[
					0,
					14.545454545454504
				],
				[
					0,
					29.09090909090901
				],
				[
					1.8181818181817562,
					41.81818181818153
				],
				[
					3.6363636363635123,
					54.545454545454504
				],
				[
					3.6363636363635123,
					60
				],
				[
					3.6363636363635123,
					63.63636363636351
				],
				[
					5.454545454545496,
					65.4545454545455
				],
				[
					5.454545454545496,
					65.4545454545455
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				5.454545454545496,
				65.4545454545455
			]
		},
		{
			"id": "QM2D2MfED4WncppJwyJKP",
			"type": "freedraw",
			"x": -657.2367854923399,
			"y": 1279.9259189161535,
			"width": 67.27272727272725,
			"height": 67.27272727272702,
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
			"seed": 1670700755,
			"version": 22,
			"versionNonce": 241840627,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.454545454545382,
					0
				],
				[
					20,
					5.454545454545496
				],
				[
					36.363636363636374,
					12.72727272727252
				],
				[
					50.90909090909088,
					18.181818181818016
				],
				[
					60,
					23.636363636363512
				],
				[
					65.4545454545455,
					29.09090909090901
				],
				[
					67.27272727272725,
					36.36363636363603
				],
				[
					67.27272727272725,
					41.81818181818153
				],
				[
					67.27272727272725,
					49.09090909090901
				],
				[
					61.81818181818187,
					54.545454545454504
				],
				[
					54.545454545454504,
					58.18181818181802
				],
				[
					43.636363636363626,
					63.63636363636351
				],
				[
					32.72727272727275,
					65.4545454545455
				],
				[
					23.636363636363626,
					65.4545454545455
				],
				[
					16.363636363636374,
					67.27272727272702
				],
				[
					9.090909090909122,
					67.27272727272702
				],
				[
					7.272727272727366,
					67.27272727272702
				],
				[
					5.454545454545382,
					67.27272727272702
				],
				[
					5.454545454545382,
					67.27272727272702
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				5.454545454545382,
				67.27272727272702
			]
		},
		{
			"id": "8jOatx5fIYsKMhhvp9g9b",
			"type": "freedraw",
			"x": -526.327694583249,
			"y": 1345.380464370699,
			"width": 45.45454545454538,
			"height": 41.81818181818198,
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
			"seed": 370518941,
			"version": 26,
			"versionNonce": 167795389,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-7.272727272727252,
					1.8181818181815288
				],
				[
					-16.36363636363626,
					3.6363636363635123
				],
				[
					-23.636363636363626,
					5.454545454545496
				],
				[
					-30.909090909090878,
					5.454545454545496
				],
				[
					-36.36363636363626,
					5.454545454545496
				],
				[
					-40,
					0
				],
				[
					-43.636363636363626,
					-7.272727272727479
				],
				[
					-45.45454545454538,
					-16.363636363636488
				],
				[
					-45.45454545454538,
					-23.636363636363967
				],
				[
					-40,
					-30.90909090909099
				],
				[
					-30.909090909090878,
					-34.545454545454504
				],
				[
					-21.818181818181756,
					-36.36363636363649
				],
				[
					-16.36363636363626,
					-36.36363636363649
				],
				[
					-10.909090909090878,
					-34.545454545454504
				],
				[
					-7.272727272727252,
					-27.27272727272748
				],
				[
					-5.454545454545382,
					-21.818181818181984
				],
				[
					-3.636363636363626,
					-14.545454545454504
				],
				[
					-1.8181818181817562,
					-5.454545454545496
				],
				[
					-1.8181818181817562,
					0
				],
				[
					-1.8181818181817562,
					3.6363636363635123
				],
				[
					-3.636363636363626,
					3.6363636363635123
				],
				[
					0,
					0
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-3.636363636363626,
				3.6363636363635123
			]
		},
		{
			"id": "rtDJXUDxba-Glwe2WG9pV",
			"type": "freedraw",
			"x": -891.7822400377945,
			"y": 1374.471373461608,
			"width": 421.81818181818187,
			"height": 12.72727272727252,
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
			"seed": 1906971699,
			"version": 18,
			"versionNonce": 1490385811,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.8181818181818699,
					1.8181818181815288
				],
				[
					3.6363636363637397,
					1.8181818181815288
				],
				[
					9.090909090909122,
					3.6363636363635123
				],
				[
					21.81818181818187,
					3.6363636363635123
				],
				[
					45.454545454545496,
					3.6363636363635123
				],
				[
					85.4545454545455,
					3.6363636363635123
				],
				[
					140,
					1.8181818181815288
				],
				[
					200,
					-1.8181818181819835
				],
				[
					263.63636363636374,
					-3.6363636363635123
				],
				[
					323.63636363636374,
					-5.454545454545496
				],
				[
					369.09090909090924,
					-7.272727272727479
				],
				[
					400.0000000000001,
					-9.090909090909008
				],
				[
					414.5454545454546,
					-9.090909090909008
				],
				[
					421.81818181818187,
					-9.090909090909008
				],
				[
					421.81818181818187,
					-9.090909090909008
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				421.81818181818187,
				-9.090909090909008
			]
		},
		{
			"id": "tWjEIG6O",
			"type": "text",
			"x": -797.2367854923398,
			"y": 1010.8350098252441,
			"width": 75.5399169921875,
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
			"seed": 1512353661,
			"version": 59,
			"versionNonce": 1711274781,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"text": "input(2)",
			"rawText": "input(2)",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "input(2)",
			"lineHeight": 1.25
		},
		{
			"id": "OXt0tXHHIhrVheiNkb3zj",
			"type": "freedraw",
			"x": -117.23678549233978,
			"y": 1283.562282552517,
			"width": 260.0000000000001,
			"height": 240.00000000000023,
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
			"seed": 1133334419,
			"version": 75,
			"versionNonce": 1986433331,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181817562,
					0
				],
				[
					-3.6363636363637397,
					0
				],
				[
					-7.272727272727252,
					1.8181818181819835
				],
				[
					-12.727272727272748,
					1.8181818181819835
				],
				[
					-18.181818181818244,
					1.8181818181819835
				],
				[
					-27.272727272727366,
					1.8181818181819835
				],
				[
					-38.181818181818244,
					1.8181818181819835
				],
				[
					-50.90909090909099,
					1.8181818181819835
				],
				[
					-67.27272727272737,
					0
				],
				[
					-83.63636363636374,
					-3.6363636363635123
				],
				[
					-100,
					-5.454545454545496
				],
				[
					-114.54545454545462,
					-10.909090909090992
				],
				[
					-129.09090909090912,
					-16.363636363636488
				],
				[
					-143.63636363636374,
					-21.818181818181984
				],
				[
					-156.36363636363637,
					-27.272727272727252
				],
				[
					-167.27272727272737,
					-34.545454545454504
				],
				[
					-176.36363636363637,
					-41.81818181818198
				],
				[
					-185.4545454545455,
					-50.90909090909099
				],
				[
					-192.72727272727275,
					-61.81818181818198
				],
				[
					-200.0000000000001,
					-72.72727272727275
				],
				[
					-205.4545454545455,
					-85.4545454545455
				],
				[
					-209.09090909090912,
					-96.36363636363649
				],
				[
					-210.909090909091,
					-110.90909090909099
				],
				[
					-212.72727272727275,
					-123.63636363636351
				],
				[
					-214.54545454545462,
					-132.72727272727275
				],
				[
					-214.54545454545462,
					-143.6363636363635
				],
				[
					-214.54545454545462,
					-154.5454545454545
				],
				[
					-212.72727272727275,
					-163.6363636363635
				],
				[
					-207.27272727272737,
					-174.5454545454545
				],
				[
					-201.81818181818187,
					-185.4545454545455
				],
				[
					-196.36363636363637,
					-194.5454545454545
				],
				[
					-190.909090909091,
					-203.6363636363635
				],
				[
					-183.63636363636374,
					-210.909090909091
				],
				[
					-176.36363636363637,
					-216.3636363636365
				],
				[
					-169.09090909090912,
					-223.6363636363635
				],
				[
					-161.81818181818187,
					-229.090909090909
				],
				[
					-152.72727272727275,
					-232.72727272727275
				],
				[
					-145.4545454545455,
					-236.3636363636365
				],
				[
					-138.18181818181824,
					-238.18181818181824
				],
				[
					-129.09090909090912,
					-238.18181818181824
				],
				[
					-120,
					-238.18181818181824
				],
				[
					-107.27272727272737,
					-238.18181818181824
				],
				[
					-92.72727272727275,
					-234.5454545454545
				],
				[
					-76.36363636363637,
					-230.909090909091
				],
				[
					-60,
					-223.6363636363635
				],
				[
					-41.81818181818187,
					-218.18181818181824
				],
				[
					-25.454545454545496,
					-210.909090909091
				],
				[
					-12.727272727272748,
					-203.6363636363635
				],
				[
					0,
					-194.5454545454545
				],
				[
					10.909090909090764,
					-185.4545454545455
				],
				[
					21.818181818181756,
					-170.909090909091
				],
				[
					30.909090909090764,
					-156.3636363636365
				],
				[
					38.181818181818244,
					-141.81818181818198
				],
				[
					41.818181818181756,
					-127.27272727272725
				],
				[
					45.454545454545496,
					-112.72727272727275
				],
				[
					45.454545454545496,
					-96.36363636363649
				],
				[
					45.454545454545496,
					-83.63636363636351
				],
				[
					41.818181818181756,
					-72.72727272727275
				],
				[
					36.36363636363626,
					-63.63636363636351
				],
				[
					29.09090909090901,
					-56.36363636363649
				],
				[
					25.454545454545496,
					-49.09090909090901
				],
				[
					18.181818181818244,
					-41.81818181818198
				],
				[
					12.727272727272748,
					-36.36363636363649
				],
				[
					9.090909090909008,
					-30.90909090909099
				],
				[
					3.6363636363635123,
					-27.272727272727252
				],
				[
					-1.8181818181817562,
					-21.818181818181984
				],
				[
					-5.454545454545496,
					-18.181818181818244
				],
				[
					-9.090909090909122,
					-12.727272727272748
				],
				[
					-12.727272727272748,
					-9.090909090909008
				],
				[
					-14.545454545454618,
					-5.454545454545496
				],
				[
					-16.363636363636374,
					-3.6363636363635123
				],
				[
					-16.363636363636374,
					-3.6363636363635123
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-16.363636363636374,
				-3.6363636363635123
			]
		},
		{
			"id": "o6d1kICwwMmIptLjGp-KY",
			"type": "freedraw",
			"x": -313.60042185597615,
			"y": 1063.562282552517,
			"width": 378.18181818181836,
			"height": 34.545454545454504,
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
			"seed": 757573555,
			"version": 78,
			"versionNonce": 1978437501,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181818699,
					0
				],
				[
					-5.454545454545496,
					0
				],
				[
					-12.727272727272748,
					0
				],
				[
					-21.81818181818187,
					0
				],
				[
					-34.54545454545462,
					0
				],
				[
					-43.63636363636374,
					0
				],
				[
					-56.363636363636374,
					0
				],
				[
					-67.27272727272737,
					0
				],
				[
					-80.00000000000011,
					0
				],
				[
					-92.72727272727275,
					1.8181818181817562
				],
				[
					-103.63636363636374,
					3.6363636363635123
				],
				[
					-116.36363636363649,
					3.6363636363635123
				],
				[
					-125.4545454545455,
					3.6363636363635123
				],
				[
					-134.54545454545462,
					3.6363636363635123
				],
				[
					-145.4545454545455,
					3.6363636363635123
				],
				[
					-154.54545454545462,
					3.6363636363635123
				],
				[
					-161.81818181818187,
					3.6363636363635123
				],
				[
					-169.09090909090912,
					3.6363636363635123
				],
				[
					-178.18181818181824,
					3.6363636363635123
				],
				[
					-185.4545454545455,
					3.6363636363635123
				],
				[
					-194.54545454545462,
					3.6363636363635123
				],
				[
					-201.81818181818187,
					3.6363636363635123
				],
				[
					-212.72727272727286,
					1.8181818181817562
				],
				[
					-220.0000000000001,
					1.8181818181817562
				],
				[
					-229.09090909090912,
					0
				],
				[
					-236.3636363636365,
					0
				],
				[
					-247.27272727272737,
					-1.8181818181819835
				],
				[
					-252.72727272727286,
					-1.8181818181819835
				],
				[
					-260.0000000000001,
					-3.6363636363635123
				],
				[
					-267.27272727272737,
					-3.6363636363635123
				],
				[
					-274.5454545454546,
					-3.6363636363635123
				],
				[
					-281.81818181818187,
					-5.454545454545496
				],
				[
					-287.27272727272737,
					-7.272727272727479
				],
				[
					-292.72727272727286,
					-7.272727272727479
				],
				[
					-296.3636363636365,
					-7.272727272727479
				],
				[
					-300.0000000000001,
					-7.272727272727479
				],
				[
					-303.63636363636374,
					-9.090909090909008
				],
				[
					-307.27272727272737,
					-9.090909090909008
				],
				[
					-310.909090909091,
					-9.090909090909008
				],
				[
					-312.72727272727286,
					-9.090909090909008
				],
				[
					-314.5454545454546,
					-10.909090909090992
				],
				[
					-318.18181818181824,
					-10.909090909090992
				],
				[
					-320.0000000000001,
					-10.909090909090992
				],
				[
					-321.81818181818187,
					-10.909090909090992
				],
				[
					-325.4545454545456,
					-10.909090909090992
				],
				[
					-329.0909090909091,
					-12.727272727272748
				],
				[
					-332.72727272727286,
					-12.727272727272748
				],
				[
					-334.5454545454546,
					-14.545454545454504
				],
				[
					-336.3636363636364,
					-14.545454545454504
				],
				[
					-340.0000000000001,
					-14.545454545454504
				],
				[
					-341.81818181818187,
					-14.545454545454504
				],
				[
					-341.81818181818187,
					-16.363636363636488
				],
				[
					-343.63636363636374,
					-16.363636363636488
				],
				[
					-345.4545454545456,
					-16.363636363636488
				],
				[
					-347.27272727272737,
					-16.363636363636488
				],
				[
					-347.27272727272737,
					-18.181818181818244
				],
				[
					-349.0909090909091,
					-18.181818181818244
				],
				[
					-350.909090909091,
					-18.181818181818244
				],
				[
					-350.909090909091,
					-20
				],
				[
					-352.72727272727286,
					-20
				],
				[
					-352.72727272727286,
					-21.818181818181984
				],
				[
					-354.5454545454546,
					-21.818181818181984
				],
				[
					-356.3636363636365,
					-21.818181818181984
				],
				[
					-358.18181818181836,
					-23.636363636363512
				],
				[
					-360.0000000000001,
					-23.636363636363512
				],
				[
					-361.81818181818187,
					-23.636363636363512
				],
				[
					-363.63636363636374,
					-25.454545454545496
				],
				[
					-365.4545454545456,
					-25.454545454545496
				],
				[
					-367.27272727272737,
					-27.27272727272748
				],
				[
					-370.909090909091,
					-29.09090909090901
				],
				[
					-372.72727272727286,
					-29.09090909090901
				],
				[
					-374.5454545454546,
					-30.90909090909099
				],
				[
					-376.3636363636365,
					-30.90909090909099
				],
				[
					-378.18181818181836,
					-30.90909090909099
				],
				[
					-378.18181818181836,
					-30.90909090909099
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-378.18181818181836,
				-30.90909090909099
			]
		},
		{
			"id": "Ypn5hK6JA_9Qynqcre6OH",
			"type": "freedraw",
			"x": -317.2367854923399,
			"y": 1056.2895552797895,
			"width": 80,
			"height": 7.272727272727479,
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
			"seed": 99437373,
			"version": 20,
			"versionNonce": 411300563,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181817562,
					0
				],
				[
					-5.454545454545382,
					0
				],
				[
					-9.090909090909008,
					0
				],
				[
					-14.545454545454504,
					1.8181818181819835
				],
				[
					-20,
					1.8181818181819835
				],
				[
					-25.454545454545382,
					3.636363636363967
				],
				[
					-30.909090909090878,
					3.636363636363967
				],
				[
					-36.363636363636374,
					5.454545454545496
				],
				[
					-43.636363636363626,
					5.454545454545496
				],
				[
					-49.09090909090901,
					5.454545454545496
				],
				[
					-54.545454545454504,
					7.272727272727479
				],
				[
					-61.818181818181756,
					7.272727272727479
				],
				[
					-67.27272727272725,
					7.272727272727479
				],
				[
					-74.5454545454545,
					7.272727272727479
				],
				[
					-78.18181818181813,
					7.272727272727479
				],
				[
					-80,
					7.272727272727479
				],
				[
					-80,
					7.272727272727479
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-80,
				7.272727272727479
			]
		},
		{
			"id": "gpLnclu18yMSO_UkulzkE",
			"type": "freedraw",
			"x": -319.05496731052165,
			"y": 1056.2895552797895,
			"width": 56.363636363636374,
			"height": 27.27272727272748,
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
			"seed": 1143854515,
			"version": 20,
			"versionNonce": 403150813,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181818699,
					0
				],
				[
					-3.636363636363626,
					1.8181818181819835
				],
				[
					-7.272727272727252,
					5.454545454545496
				],
				[
					-10.909090909090878,
					10.909090909090992
				],
				[
					-16.363636363636374,
					14.545454545454731
				],
				[
					-20,
					16.363636363636488
				],
				[
					-25.454545454545496,
					20.000000000000227
				],
				[
					-29.090909090909122,
					21.818181818181984
				],
				[
					-34.54545454545462,
					23.636363636363967
				],
				[
					-38.181818181818244,
					23.636363636363967
				],
				[
					-41.81818181818187,
					25.454545454545496
				],
				[
					-45.454545454545496,
					25.454545454545496
				],
				[
					-49.09090909090912,
					25.454545454545496
				],
				[
					-50.90909090909088,
					25.454545454545496
				],
				[
					-54.54545454545462,
					27.27272727272748
				],
				[
					-56.363636363636374,
					27.27272727272748
				],
				[
					-56.363636363636374,
					27.27272727272748
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-56.363636363636374,
				27.27272727272748
			]
		},
		{
			"id": "jIxrHCzePboDVS_6MlqEv",
			"type": "freedraw",
			"x": -315.418603674158,
			"y": 1054.471373461608,
			"width": 81.81818181818187,
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
			"seed": 582581853,
			"version": 15,
			"versionNonce": 2143559795,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181818699,
					-3.6363636363637397
				],
				[
					-7.272727272727252,
					-5.454545454545496
				],
				[
					-16.363636363636374,
					-7.272727272727479
				],
				[
					-25.454545454545496,
					-10.909090909090992
				],
				[
					-36.363636363636374,
					-14.545454545454504
				],
				[
					-45.454545454545496,
					-16.363636363636488
				],
				[
					-54.545454545454504,
					-18.18181818181847
				],
				[
					-63.636363636363626,
					-18.18181818181847
				],
				[
					-72.72727272727275,
					-20
				],
				[
					-78.18181818181824,
					-20
				],
				[
					-81.81818181818187,
					-20
				],
				[
					-81.81818181818187,
					-20
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-81.81818181818187,
				-20
			]
		},
		{
			"id": "EE2m9BRyHWRjNZCFkqjvs",
			"type": "freedraw",
			"x": 553.6723054167512,
			"y": 1045.3804643706987,
			"width": 63.63636363636351,
			"height": 41.818181818181756,
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
			"seed": 1099282685,
			"version": 40,
			"versionNonce": 1717736509,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181817562,
					0
				],
				[
					-10.909090909090992,
					0
				],
				[
					-12.727272727272748,
					0
				],
				[
					-20,
					0
				],
				[
					-29.090909090909236,
					-3.6363636363637397
				],
				[
					-38.181818181818244,
					-7.272727272727252
				],
				[
					-43.63636363636374,
					-10.909090909090764
				],
				[
					-49.090909090909236,
					-16.36363636363626
				],
				[
					-52.72727272727275,
					-23.636363636363626
				],
				[
					-52.72727272727275,
					-30.909090909090878
				],
				[
					-52.72727272727275,
					-36.363636363636374
				],
				[
					-49.090909090909236,
					-40
				],
				[
					-47.27272727272725,
					-41.818181818181756
				],
				[
					-41.818181818181756,
					-41.818181818181756
				],
				[
					-38.181818181818244,
					-41.818181818181756
				],
				[
					-32.72727272727275,
					-41.818181818181756
				],
				[
					-25.454545454545496,
					-41.818181818181756
				],
				[
					-16.363636363636488,
					-40
				],
				[
					-9.090909090909236,
					-38.18181818181813
				],
				[
					-1.8181818181817562,
					-38.18181818181813
				],
				[
					3.6363636363635123,
					-36.363636363636374
				],
				[
					5.454545454545496,
					-34.545454545454504
				],
				[
					7.272727272727252,
					-34.545454545454504
				],
				[
					10.909090909090764,
					-34.545454545454504
				],
				[
					10.909090909090764,
					-32.72727272727275
				],
				[
					10.909090909090764,
					-30.909090909090878
				],
				[
					10.909090909090764,
					-29.090909090909122
				],
				[
					10.909090909090764,
					-25.454545454545382
				],
				[
					9.090909090909008,
					-21.818181818181756
				],
				[
					7.272727272727252,
					-18.181818181818244
				],
				[
					5.454545454545496,
					-16.36363636363626
				],
				[
					3.6363636363635123,
					-14.545454545454504
				],
				[
					0,
					-12.727272727272748
				],
				[
					0,
					-10.909090909090764
				],
				[
					-1.8181818181817562,
					-10.909090909090764
				],
				[
					0,
					0
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-1.8181818181817562,
				-10.909090909090764
			]
		},
		{
			"id": "jOoK3NBusDopeKQ5S58XR",
			"type": "freedraw",
			"x": 144.58139632584198,
			"y": 994.4713734616079,
			"width": 0,
			"height": 34.54545454545462,
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
			"seed": 708007987,
			"version": 19,
			"versionNonce": 367893011,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.8181818181817562
				],
				[
					0,
					3.636363636363626
				],
				[
					0,
					7.272727272727252
				],
				[
					0,
					12.727272727272748
				],
				[
					0,
					16.363636363636374
				],
				[
					0,
					18.18181818181813
				],
				[
					0,
					20
				],
				[
					0,
					21.818181818181756
				],
				[
					0,
					23.636363636363626
				],
				[
					0,
					25.454545454545496
				],
				[
					0,
					27.272727272727252
				],
				[
					0,
					29.090909090909122
				],
				[
					0,
					30.909090909090878
				],
				[
					0,
					32.727272727272634
				],
				[
					0,
					34.54545454545462
				],
				[
					0,
					34.54545454545462
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				0,
				34.54545454545462
			]
		},
		{
			"id": "_i4CwTjO9quPWYOt4xFoT",
			"type": "freedraw",
			"x": -200.87314912870352,
			"y": 1001.7441007343351,
			"width": 90.90909090909099,
			"height": 30.909090909090878,
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
			"seed": 169514707,
			"version": 37,
			"versionNonce": 1021248669,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.6363636363637397,
					0
				],
				[
					7.272727272727366,
					0
				],
				[
					10.909090909090992,
					0
				],
				[
					16.363636363636374,
					0
				],
				[
					21.81818181818187,
					0
				],
				[
					25.454545454545496,
					0
				],
				[
					30.90909090909099,
					0
				],
				[
					36.363636363636374,
					0
				],
				[
					40.000000000000114,
					3.636363636363626
				],
				[
					43.63636363636374,
					5.454545454545496
				],
				[
					45.454545454545496,
					10.909090909090878
				],
				[
					47.272727272727366,
					12.727272727272748
				],
				[
					47.272727272727366,
					16.363636363636374
				],
				[
					47.272727272727366,
					20
				],
				[
					45.454545454545496,
					23.636363636363626
				],
				[
					40.000000000000114,
					25.454545454545382
				],
				[
					34.54545454545462,
					29.090909090909122
				],
				[
					29.090909090909122,
					30.909090909090878
				],
				[
					23.63636363636374,
					30.909090909090878
				],
				[
					21.81818181818187,
					30.909090909090878
				],
				[
					20,
					30.909090909090878
				],
				[
					21.81818181818187,
					30.909090909090878
				],
				[
					23.63636363636374,
					30.909090909090878
				],
				[
					29.090909090909122,
					30.909090909090878
				],
				[
					36.363636363636374,
					30.909090909090878
				],
				[
					45.454545454545496,
					30.909090909090878
				],
				[
					54.54545454545462,
					30.909090909090878
				],
				[
					63.63636363636374,
					30.909090909090878
				],
				[
					70.90909090909099,
					30.909090909090878
				],
				[
					78.18181818181824,
					30.909090909090878
				],
				[
					85.4545454545455,
					30.909090909090878
				],
				[
					89.09090909090924,
					30.909090909090878
				],
				[
					90.90909090909099,
					30.909090909090878
				],
				[
					90.90909090909099,
					30.909090909090878
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				90.90909090909099,
				30.909090909090878
			]
		},
		{
			"id": "hmy1bQnB",
			"type": "text",
			"x": -896.327694583249,
			"y": 1393.4107674010017,
			"width": 1320.7989501953125,
			"height": 200,
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
			"seed": 798639773,
			"version": 648,
			"versionNonce": 191972883,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485633914,
			"link": null,
			"locked": false,
			"text": "Check to see if link is null;\ncheck to see if input value is longer than the length of the link;\ncreate temp node and equate it to the head;\ncreate a prev temp node and equate it to head;\ncreate a for loop and do temp.next to equate the value of the index, have this in an if else to make sure you don't step into null;\nnow create a while loop and do a temp.next and a prevTemp.next until the while loop breaks and then return the value of prevTemp\n\n",
			"rawText": "Check to see if link is null;\ncheck to see if input value is longer than the length of the link;\ncreate temp node and equate it to the head;\ncreate a prev temp node and equate it to head;\ncreate a for loop and do temp.next to equate the value of the index, have this in an if else to make sure you don't step into null;\nnow create a while loop and do a temp.next and a prevTemp.next until the while loop breaks and then return the value of prevTemp\n\n",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 193,
			"containerId": null,
			"originalText": "Check to see if link is null;\ncheck to see if input value is longer than the length of the link;\ncreate temp node and equate it to the head;\ncreate a prev temp node and equate it to head;\ncreate a for loop and do temp.next to equate the value of the index, have this in an if else to make sure you don't step into null;\nnow create a while loop and do a temp.next and a prevTemp.next until the while loop breaks and then return the value of prevTemp\n\n",
			"lineHeight": 1.25
		},
		{
			"id": "kMh94dFzKKcSgkr5IHFi7",
			"type": "freedraw",
			"x": -846.479209734764,
			"y": 1603.5622825525174,
			"width": 3.3333333333332575,
			"height": 55,
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
			"seed": 941224605,
			"version": 13,
			"versionNonce": 537293139,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.6666666666666288,
					0
				],
				[
					1.6666666666666288,
					1.666666666666515
				],
				[
					3.3333333333332575,
					6.666666666666515
				],
				[
					3.3333333333332575,
					15
				],
				[
					3.3333333333332575,
					25
				],
				[
					3.3333333333332575,
					35
				],
				[
					1.6666666666666288,
					45
				],
				[
					1.6666666666666288,
					51.666666666666515
				],
				[
					1.6666666666666288,
					55
				],
				[
					1.6666666666666288,
					55
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				1.6666666666666288,
				55
			]
		},
		{
			"id": "IuPq0w6jU77ZabaDDlkjY",
			"type": "freedraw",
			"x": -858.1458764014308,
			"y": 1598.5622825525174,
			"width": 65,
			"height": 1.6666666666667425,
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
			"seed": 1844222173,
			"version": 12,
			"versionNonce": 517095773,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1.6666666666667425
				],
				[
					5,
					-1.6666666666667425
				],
				[
					11.666666666666742,
					-1.6666666666667425
				],
				[
					21.666666666666742,
					-1.6666666666667425
				],
				[
					35,
					-1.6666666666667425
				],
				[
					53.33333333333337,
					-1.6666666666667425
				],
				[
					58.33333333333337,
					-1.6666666666667425
				],
				[
					65,
					-1.6666666666667425
				],
				[
					65,
					-1.6666666666667425
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				65,
				-1.6666666666667425
			]
		},
		{
			"id": "HSP3vtP2i3vqWDEW7102p",
			"type": "freedraw",
			"x": -838.1458764014308,
			"y": 1625.228949219184,
			"width": 35,
			"height": 6.6666666666667425,
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
			"seed": 1523623827,
			"version": 11,
			"versionNonce": 527617779,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.6666666666667425
				],
				[
					5,
					1.6666666666667425
				],
				[
					11.666666666666742,
					3.333333333333485
				],
				[
					20,
					5
				],
				[
					28.33333333333337,
					5
				],
				[
					33.33333333333337,
					6.6666666666667425
				],
				[
					35,
					6.6666666666667425
				],
				[
					35,
					6.6666666666667425
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				35,
				6.6666666666667425
			]
		},
		{
			"id": "-7rwEEfNw25b01eY3DMxP",
			"type": "freedraw",
			"x": -838.1458764014308,
			"y": 1655.228949219184,
			"width": 55,
			"height": 6.6666666666667425,
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
			"seed": 1266060211,
			"version": 12,
			"versionNonce": 1629228477,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.6666666666667425,
					1.6666666666667425
				],
				[
					5,
					1.6666666666667425
				],
				[
					8.333333333333371,
					3.333333333333485
				],
				[
					18.33333333333337,
					3.333333333333485
				],
				[
					26.666666666666742,
					5
				],
				[
					40,
					5
				],
				[
					48.33333333333337,
					6.6666666666667425
				],
				[
					55,
					6.6666666666667425
				],
				[
					55,
					6.6666666666667425
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				55,
				6.6666666666667425
			]
		},
		{
			"id": "96_2IfxEIpmUWI-QRRWPK",
			"type": "freedraw",
			"x": -734.8125430680974,
			"y": 1655.228949219184,
			"width": 41.66666666666663,
			"height": 73.33333333333326,
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
			"seed": 1605418717,
			"version": 35,
			"versionNonce": 1489139859,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					3.333333333333485
				],
				[
					0,
					6.6666666666667425
				],
				[
					0,
					8.333333333333485
				],
				[
					-5,
					10
				],
				[
					-11.666666666666629,
					10
				],
				[
					-18.33333333333337,
					10
				],
				[
					-25,
					10
				],
				[
					-31.66666666666663,
					6.6666666666667425
				],
				[
					-38.33333333333337,
					1.6666666666667425
				],
				[
					-40,
					-1.666666666666515
				],
				[
					-40,
					-3.3333333333332575
				],
				[
					-40,
					-6.666666666666515
				],
				[
					-35,
					-10
				],
				[
					-26.66666666666663,
					-10
				],
				[
					-20,
					-10
				],
				[
					-13.333333333333371,
					-8.333333333333258
				],
				[
					-6.666666666666629,
					-5
				],
				[
					-3.3333333333333712,
					-3.3333333333332575
				],
				[
					-1.6666666666666288,
					-1.666666666666515
				],
				[
					0,
					0
				],
				[
					0,
					1.6666666666667425
				],
				[
					0,
					3.333333333333485
				],
				[
					0,
					5
				],
				[
					1.6666666666666288,
					5
				],
				[
					1.6666666666666288,
					0
				],
				[
					1.6666666666666288,
					-10
				],
				[
					1.6666666666666288,
					-23.333333333333258
				],
				[
					1.6666666666666288,
					-40
				],
				[
					1.6666666666666288,
					-55
				],
				[
					1.6666666666666288,
					-61.666666666666515
				],
				[
					1.6666666666666288,
					-63.33333333333326
				],
				[
					1.6666666666666288,
					-63.33333333333326
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				1.6666666666666288,
				-63.33333333333326
			]
		},
		{
			"id": "ATbhAjSlZHeFRg7uHoKzJ",
			"type": "freedraw",
			"x": -688.1458764014308,
			"y": 1623.5622825525174,
			"width": 50,
			"height": 45,
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
			"seed": 1074938173,
			"version": 28,
			"versionNonce": 1697467933,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.666666666666515
				],
				[
					-3.3333333333332575,
					1.666666666666515
				],
				[
					-8.333333333333258,
					1.666666666666515
				],
				[
					-13.333333333333258,
					0
				],
				[
					-20,
					-3.333333333333485
				],
				[
					-23.333333333333258,
					-6.6666666666667425
				],
				[
					-25,
					-10
				],
				[
					-26.66666666666663,
					-11.666666666666742
				],
				[
					-26.66666666666663,
					-13.333333333333485
				],
				[
					-21.66666666666663,
					-13.333333333333485
				],
				[
					-15,
					-10
				],
				[
					-5,
					-5
				],
				[
					5,
					3.3333333333332575
				],
				[
					13.333333333333371,
					10
				],
				[
					20,
					16.666666666666515
				],
				[
					21.666666666666742,
					23.333333333333258
				],
				[
					23.33333333333337,
					26.666666666666515
				],
				[
					23.33333333333337,
					28.333333333333258
				],
				[
					23.33333333333337,
					30
				],
				[
					18.33333333333337,
					31.666666666666515
				],
				[
					13.333333333333371,
					31.666666666666515
				],
				[
					5,
					31.666666666666515
				],
				[
					0,
					31.666666666666515
				],
				[
					-5,
					30
				],
				[
					-5,
					30
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-5,
				30
			]
		},
		{
			"id": "a704OfTmcMWIO-9PN38ny",
			"type": "freedraw",
			"x": -634.8125430680974,
			"y": 1645.228949219184,
			"width": 61.66666666666663,
			"height": 51.66666666666674,
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
			"seed": 1645809203,
			"version": 42,
			"versionNonce": 1236004403,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.6666666666666288,
					-1.666666666666515
				],
				[
					3.3333333333333712,
					-1.666666666666515
				],
				[
					8.333333333333371,
					-3.3333333333332575
				],
				[
					16.66666666666663,
					-5
				],
				[
					30,
					-6.666666666666515
				],
				[
					43.33333333333337,
					-10
				],
				[
					53.33333333333337,
					-11.666666666666515
				],
				[
					58.33333333333337,
					-16.666666666666515
				],
				[
					60,
					-18.333333333333258
				],
				[
					60,
					-21.666666666666515
				],
				[
					60,
					-23.333333333333258
				],
				[
					58.33333333333337,
					-23.333333333333258
				],
				[
					55,
					-23.333333333333258
				],
				[
					48.33333333333337,
					-23.333333333333258
				],
				[
					40,
					-20
				],
				[
					31.66666666666663,
					-16.666666666666515
				],
				[
					25,
					-13.333333333333258
				],
				[
					18.33333333333337,
					-10
				],
				[
					15,
					-10
				],
				[
					10,
					-6.666666666666515
				],
				[
					6.666666666666629,
					-5
				],
				[
					5,
					-5
				],
				[
					3.3333333333333712,
					-3.3333333333332575
				],
				[
					3.3333333333333712,
					1.6666666666667425
				],
				[
					3.3333333333333712,
					6.6666666666667425
				],
				[
					3.3333333333333712,
					10
				],
				[
					5,
					15
				],
				[
					8.333333333333371,
					20
				],
				[
					15,
					25
				],
				[
					21.66666666666663,
					26.666666666666742
				],
				[
					30,
					28.333333333333485
				],
				[
					38.33333333333337,
					28.333333333333485
				],
				[
					48.33333333333337,
					28.333333333333485
				],
				[
					55,
					28.333333333333485
				],
				[
					58.33333333333337,
					28.333333333333485
				],
				[
					60,
					28.333333333333485
				],
				[
					60,
					26.666666666666742
				],
				[
					61.66666666666663,
					25
				],
				[
					61.66666666666663,
					25
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				61.66666666666663,
				25
			]
		},
		{
			"id": "hZhWzlV36B6HFpSUIzjs1",
			"type": "freedraw",
			"x": -481.479209734764,
			"y": 1610.228949219184,
			"width": 56.66666666666674,
			"height": 63.333333333333485,
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
			"seed": 2067177981,
			"version": 20,
			"versionNonce": 1777828477,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.6666666666667425,
					0
				],
				[
					-8.333333333333371,
					1.6666666666667425
				],
				[
					-18.33333333333337,
					3.333333333333485
				],
				[
					-31.666666666666742,
					8.333333333333485
				],
				[
					-43.33333333333337,
					15
				],
				[
					-51.66666666666674,
					23.333333333333485
				],
				[
					-55,
					31.666666666666742
				],
				[
					-56.66666666666674,
					38.333333333333485
				],
				[
					-55,
					46.66666666666674
				],
				[
					-48.33333333333337,
					53.333333333333485
				],
				[
					-41.66666666666674,
					58.333333333333485
				],
				[
					-35,
					63.333333333333485
				],
				[
					-28.33333333333337,
					63.333333333333485
				],
				[
					-21.666666666666742,
					63.333333333333485
				],
				[
					-15,
					61.66666666666674
				],
				[
					-8.333333333333371,
					58.333333333333485
				],
				[
					-8.333333333333371,
					58.333333333333485
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-8.333333333333371,
				58.333333333333485
			]
		},
		{
			"id": "LNQyLjOzxzdO1QcfMKL6a",
			"type": "freedraw",
			"x": -459.8125430680974,
			"y": 1653.5622825525174,
			"width": 40,
			"height": 26.666666666666515,
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
			"seed": 1653105395,
			"version": 32,
			"versionNonce": 1964355539,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.6666666666666288,
					0
				],
				[
					-3.3333333333333712,
					0
				],
				[
					-5,
					0
				],
				[
					-10,
					0
				],
				[
					-11.666666666666629,
					-3.333333333333485
				],
				[
					-15,
					-10
				],
				[
					-18.33333333333337,
					-13.333333333333485
				],
				[
					-18.33333333333337,
					-20
				],
				[
					-16.66666666666663,
					-23.333333333333485
				],
				[
					-13.333333333333371,
					-25
				],
				[
					-8.333333333333371,
					-25
				],
				[
					-6.666666666666629,
					-25
				],
				[
					-5,
					-25
				],
				[
					-3.3333333333333712,
					-23.333333333333485
				],
				[
					-1.6666666666666288,
					-20
				],
				[
					-1.6666666666666288,
					-16.666666666666742
				],
				[
					-1.6666666666666288,
					-11.666666666666742
				],
				[
					-1.6666666666666288,
					-6.6666666666667425
				],
				[
					-1.6666666666666288,
					-3.333333333333485
				],
				[
					0,
					-1.6666666666667425
				],
				[
					0,
					0
				],
				[
					3.3333333333333712,
					1.666666666666515
				],
				[
					6.666666666666629,
					1.666666666666515
				],
				[
					11.666666666666629,
					1.666666666666515
				],
				[
					16.66666666666663,
					1.666666666666515
				],
				[
					18.33333333333337,
					1.666666666666515
				],
				[
					21.66666666666663,
					1.666666666666515
				],
				[
					21.66666666666663,
					0
				],
				[
					21.66666666666663,
					0
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				21.66666666666663,
				0
			]
		},
		{
			"id": "WyEEQNocRrvB2rBHpgyrx",
			"type": "freedraw",
			"x": -426.479209734764,
			"y": 1618.5622825525174,
			"width": 21.66666666666663,
			"height": 38.33333333333326,
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
			"seed": 1025545053,
			"version": 22,
			"versionNonce": 1413229277,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.6666666666667425,
					0
				],
				[
					-3.3333333333333712,
					0
				],
				[
					-5,
					0
				],
				[
					-5,
					1.666666666666515
				],
				[
					0,
					5
				],
				[
					5,
					8.333333333333258
				],
				[
					8.333333333333258,
					13.333333333333258
				],
				[
					13.333333333333258,
					16.666666666666515
				],
				[
					15,
					21.666666666666515
				],
				[
					16.66666666666663,
					26.666666666666515
				],
				[
					16.66666666666663,
					30
				],
				[
					16.66666666666663,
					33.33333333333326
				],
				[
					13.333333333333258,
					36.666666666666515
				],
				[
					11.666666666666629,
					38.33333333333326
				],
				[
					10,
					38.33333333333326
				],
				[
					8.333333333333258,
					38.33333333333326
				],
				[
					6.666666666666629,
					38.33333333333326
				],
				[
					5,
					38.33333333333326
				],
				[
					5,
					38.33333333333326
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				5,
				38.33333333333326
			]
		},
		{
			"id": "YtOt9glr6HpHOAwyGd879",
			"type": "freedraw",
			"x": -404.8125430680974,
			"y": 1641.8956158858507,
			"width": 30,
			"height": 35,
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
			"seed": 624073011,
			"version": 31,
			"versionNonce": 1024867699,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.6666666666666288,
					0
				],
				[
					6.666666666666629,
					-1.6666666666667425
				],
				[
					8.333333333333371,
					-1.6666666666667425
				],
				[
					13.333333333333371,
					-3.3333333333332575
				],
				[
					15,
					-5
				],
				[
					18.33333333333337,
					-8.333333333333258
				],
				[
					20,
					-11.666666666666742
				],
				[
					21.66666666666663,
					-15
				],
				[
					21.66666666666663,
					-18.333333333333258
				],
				[
					21.66666666666663,
					-20
				],
				[
					20,
					-20
				],
				[
					16.66666666666663,
					-20
				],
				[
					13.333333333333371,
					-18.333333333333258
				],
				[
					10,
					-13.333333333333258
				],
				[
					8.333333333333371,
					-8.333333333333258
				],
				[
					8.333333333333371,
					-1.6666666666667425
				],
				[
					8.333333333333371,
					1.6666666666667425
				],
				[
					8.333333333333371,
					5
				],
				[
					8.333333333333371,
					10
				],
				[
					11.666666666666629,
					11.666666666666742
				],
				[
					15,
					13.333333333333258
				],
				[
					18.33333333333337,
					13.333333333333258
				],
				[
					21.66666666666663,
					15
				],
				[
					25,
					15
				],
				[
					26.66666666666663,
					15
				],
				[
					28.33333333333337,
					15
				],
				[
					30,
					13.333333333333258
				],
				[
					30,
					13.333333333333258
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				30,
				13.333333333333258
			]
		},
		{
			"id": "NZs6N42u6UNujbn0R_61U",
			"type": "freedraw",
			"x": -349.8125430680974,
			"y": 1610.228949219184,
			"width": 20,
			"height": 40,
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
			"seed": 1757379987,
			"version": 29,
			"versionNonce": 1955383101,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.6666666666666288,
					-1.666666666666515
				],
				[
					-5,
					-1.666666666666515
				],
				[
					-6.666666666666629,
					-1.666666666666515
				],
				[
					-10,
					-1.666666666666515
				],
				[
					-11.666666666666629,
					-1.666666666666515
				],
				[
					-13.333333333333371,
					-1.666666666666515
				],
				[
					-13.333333333333371,
					0
				],
				[
					-13.333333333333371,
					1.6666666666667425
				],
				[
					-13.333333333333371,
					3.333333333333485
				],
				[
					-13.333333333333371,
					5
				],
				[
					-11.666666666666629,
					6.6666666666667425
				],
				[
					-8.333333333333371,
					10
				],
				[
					-5,
					13.333333333333485
				],
				[
					0,
					16.666666666666742
				],
				[
					3.3333333333333712,
					21.666666666666742
				],
				[
					6.666666666666629,
					25
				],
				[
					6.666666666666629,
					30
				],
				[
					6.666666666666629,
					31.666666666666742
				],
				[
					6.666666666666629,
					35
				],
				[
					6.666666666666629,
					36.66666666666674
				],
				[
					6.666666666666629,
					38.333333333333485
				],
				[
					5,
					38.333333333333485
				],
				[
					1.6666666666666288,
					38.333333333333485
				],
				[
					-3.3333333333333712,
					38.333333333333485
				],
				[
					-6.666666666666629,
					38.333333333333485
				],
				[
					-6.666666666666629,
					38.333333333333485
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-6.666666666666629,
				38.333333333333485
			]
		},
		{
			"id": "9-baq5VFss43QaqoF6FjU",
			"type": "freedraw",
			"x": -889.8125430680974,
			"y": 1693.5622825525174,
			"width": 576.6666666666666,
			"height": 16.666666666666515,
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
			"seed": 1848651859,
			"version": 35,
			"versionNonce": 2096371475,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.3333333333333712,
					0
				],
				[
					18.33333333333337,
					0
				],
				[
					41.66666666666663,
					0
				],
				[
					76.66666666666663,
					0
				],
				[
					118.33333333333337,
					3.3333333333332575
				],
				[
					156.66666666666663,
					5
				],
				[
					193.33333333333337,
					6.666666666666515
				],
				[
					225,
					8.333333333333258
				],
				[
					251.66666666666663,
					10
				],
				[
					275,
					10
				],
				[
					295,
					11.666666666666515
				],
				[
					316.66666666666663,
					11.666666666666515
				],
				[
					338.33333333333337,
					11.666666666666515
				],
				[
					356.66666666666663,
					11.666666666666515
				],
				[
					376.66666666666663,
					11.666666666666515
				],
				[
					395,
					10
				],
				[
					411.66666666666663,
					8.333333333333258
				],
				[
					430,
					8.333333333333258
				],
				[
					448.33333333333337,
					6.666666666666515
				],
				[
					466.66666666666663,
					5
				],
				[
					485,
					3.3333333333332575
				],
				[
					501.66666666666663,
					1.666666666666515
				],
				[
					518.3333333333334,
					1.666666666666515
				],
				[
					533.3333333333334,
					0
				],
				[
					546.6666666666666,
					0
				],
				[
					556.6666666666666,
					-1.6666666666667425
				],
				[
					565,
					-3.333333333333485
				],
				[
					570,
					-5
				],
				[
					573.3333333333334,
					-5
				],
				[
					575,
					-5
				],
				[
					576.6666666666666,
					-5
				],
				[
					576.6666666666666,
					-5
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				576.6666666666666,
				-5
			]
		},
		{
			"id": "Hc1EREYv",
			"type": "text",
			"x": -829.8125430680974,
			"y": 1733.5622825525174,
			"width": 403.97967529296875,
			"height": 100,
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
			"seed": 393799667,
			"version": 251,
			"versionNonce": 223008669,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485574246,
			"link": null,
			"locked": false,
			"text": "What if the input value does not exsist;\nwhat if the linklist does not exsist;\nwhat if k is not the last node;\nany more edge cases?",
			"rawText": "What if the input value does not exsist;\nwhat if the linklist does not exsist;\nwhat if k is not the last node;\nany more edge cases?",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 93,
			"containerId": null,
			"originalText": "What if the input value does not exsist;\nwhat if the linklist does not exsist;\nwhat if k is not the last node;\nany more edge cases?",
			"lineHeight": 1.25
		},
		{
			"type": "freedraw",
			"version": 136,
			"versionNonce": 1118375325,
			"isDeleted": false,
			"id": "QRgHc5kaEQXXn0OSDWcwG",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 207.69101731601722,
			"y": 1747.3198583100932,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 25,
			"height": 89,
			"seed": 1257587187,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485643119,
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
			"version": 163,
			"versionNonce": 1651369651,
			"isDeleted": false,
			"id": "jrrudqb039f1_IgDxNcZx",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 204.69101731601722,
			"y": 1744.3198583100932,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 71,
			"height": 75,
			"seed": 295304637,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485643119,
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
			"version": 130,
			"versionNonce": 818893309,
			"isDeleted": false,
			"id": "zW4OVS1V77EHqKK6SurX1",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 294.6910173160172,
			"y": 1776.3198583100932,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 12,
			"height": 17,
			"seed": 1700508157,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485643119,
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
			"version": 122,
			"versionNonce": 67410003,
			"isDeleted": false,
			"id": "v6egnEl5ua3vy-1m8auxl",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 293.6910173160172,
			"y": 1758.3198583100932,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 88188019,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485643119,
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
			"version": 146,
			"versionNonce": 510528093,
			"isDeleted": false,
			"id": "GBUZA4qFYTeAtxrwhKQQW",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 359.6910173160172,
			"y": 1741.3198583100932,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 40,
			"height": 50,
			"seed": 301219997,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485643119,
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
			"version": 122,
			"versionNonce": 1326716403,
			"isDeleted": false,
			"id": "tzrVIqumrs17hfjAuUunn",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 359.6910173160172,
			"y": 1768.3198583100932,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 800092371,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485643119,
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
			"versionNonce": 1817622205,
			"isDeleted": false,
			"id": "0pg0Vm4m-NrsbX0i3A01G",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 427.6910173160172,
			"y": 1773.3198583100932,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 81,
			"height": 83,
			"seed": 237549117,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485643119,
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
			"version": 136,
			"versionNonce": 849534867,
			"isDeleted": false,
			"id": "Yub1BQjdZ4jXgt579wjzL",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 172.69101731601722,
			"y": 1849.3198583100932,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 301,
			"height": 71,
			"seed": 2036254451,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485643119,
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
			"version": 682,
			"versionNonce": 218334771,
			"isDeleted": false,
			"id": "wJnO8ZeL",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 108.69101731601722,
			"y": 1871.3198583100932,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 342.43988037109375,
			"height": 25,
			"seed": 1643923645,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682486382374,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "NOT SURE WHAT BIG O IS HERE",
			"rawText": "NOT SURE WHAT BIG O IS HERE",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "NOT SURE WHAT BIG O IS HERE",
			"lineHeight": 1.25,
			"baseline": 18
		},
		{
			"type": "freedraw",
			"version": 102,
			"versionNonce": 2028434739,
			"isDeleted": false,
			"id": "NSwlucVgas-svTVxswg4v",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 260.270790265236,
			"y": 1992.5776708100932,
			"strokeColor": "#000000",
			"backgroundColor": "transparent",
			"width": 0.0001,
			"height": 0.0001,
			"seed": 318262173,
			"groupIds": [],
			"roundness": null,
			"boundElements": [],
			"updated": 1682485643119,
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
			"id": "ZdTcc0oXDKrN7qXPo96Yg",
			"type": "freedraw",
			"x": 487.91472965917524,
			"y": -1551.7407477505133,
			"width": 112.72727272727275,
			"height": 70.90909090909099,
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
			"seed": 1632130771,
			"version": 48,
			"versionNonce": 1728038013,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485654335,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181817562,
					0
				],
				[
					-3.6363636363637397,
					1.8181818181817562
				],
				[
					-9.090909090909008,
					3.6363636363637397
				],
				[
					-16.363636363636488,
					7.272727272727252
				],
				[
					-23.63636363636374,
					7.272727272727252
				],
				[
					-30.90909090909099,
					9.090909090909236
				],
				[
					-36.36363636363649,
					9.090909090909236
				],
				[
					-40,
					9.090909090909236
				],
				[
					-43.63636363636374,
					9.090909090909236
				],
				[
					-49.090909090909236,
					5.454545454545496
				],
				[
					-54.545454545454504,
					1.8181818181817562
				],
				[
					-58.181818181818244,
					-5.4545454545452685
				],
				[
					-63.63636363636374,
					-16.36363636363626
				],
				[
					-70.90909090909099,
					-27.272727272727252
				],
				[
					-74.5454545454545,
					-36.36363636363626
				],
				[
					-78.18181818181824,
					-45.45454545454527
				],
				[
					-81.81818181818176,
					-54.545454545454504
				],
				[
					-81.81818181818176,
					-58.181818181818244
				],
				[
					-81.81818181818176,
					-61.818181818181756
				],
				[
					-78.18181818181824,
					-61.818181818181756
				],
				[
					-70.90909090909099,
					-61.818181818181756
				],
				[
					-60,
					-61.818181818181756
				],
				[
					-47.27272727272725,
					-60
				],
				[
					-32.72727272727275,
					-58.181818181818244
				],
				[
					-18.181818181818244,
					-56.36363636363626
				],
				[
					-5.454545454545496,
					-52.72727272727275
				],
				[
					7.272727272727252,
					-49.09090909090901
				],
				[
					16.36363636363626,
					-43.63636363636351
				],
				[
					21.818181818181756,
					-41.818181818181756
				],
				[
					25.454545454545496,
					-38.181818181818244
				],
				[
					29.09090909090901,
					-36.36363636363626
				],
				[
					29.09090909090901,
					-34.545454545454504
				],
				[
					30.90909090909099,
					-30.909090909090764
				],
				[
					30.90909090909099,
					-25.45454545454527
				],
				[
					30.90909090909099,
					-20
				],
				[
					30.90909090909099,
					-14.545454545454504
				],
				[
					25.454545454545496,
					-12.727272727272748
				],
				[
					21.818181818181756,
					-9.090909090909008
				],
				[
					16.36363636363626,
					-7.272727272727252
				],
				[
					9.090909090909008,
					-7.272727272727252
				],
				[
					1.8181818181817562,
					-7.272727272727252
				],
				[
					-3.6363636363637397,
					-7.272727272727252
				],
				[
					-9.090909090909008,
					-7.272727272727252
				],
				[
					-10.909090909090992,
					-7.272727272727252
				],
				[
					-12.727272727272748,
					-7.272727272727252
				],
				[
					-12.727272727272748,
					-7.272727272727252
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-12.727272727272748,
				-7.272727272727252
			]
		},
		{
			"id": "ed_OjFcdfOivudEGQNL7W",
			"type": "freedraw",
			"x": 547.9147296591752,
			"y": -2939.013475023242,
			"width": 125.4545454545455,
			"height": 70.90909090909099,
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
			"seed": 1563069907,
			"version": 42,
			"versionNonce": 1075674205,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485657443,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181817562,
					1.8181818181819835
				],
				[
					-5.454545454545496,
					1.8181818181819835
				],
				[
					-10.909090909090992,
					1.8181818181819835
				],
				[
					-21.818181818181756,
					3.6363636363635123
				],
				[
					-36.36363636363649,
					3.6363636363635123
				],
				[
					-50.90909090909099,
					3.6363636363635123
				],
				[
					-67.27272727272725,
					5.454545454545496
				],
				[
					-81.81818181818176,
					5.454545454545496
				],
				[
					-92.72727272727275,
					3.6363636363635123
				],
				[
					-105.4545454545455,
					1.8181818181819835
				],
				[
					-112.72727272727275,
					-1.8181818181819835
				],
				[
					-118.18181818181824,
					-5.454545454545496
				],
				[
					-121.81818181818176,
					-7.272727272727025
				],
				[
					-123.63636363636374,
					-10.909090909090992
				],
				[
					-125.4545454545455,
					-14.545454545454504
				],
				[
					-125.4545454545455,
					-21.818181818181984
				],
				[
					-125.4545454545455,
					-29.09090909090901
				],
				[
					-123.63636363636374,
					-36.36363636363649
				],
				[
					-116.36363636363649,
					-45.454545454545496
				],
				[
					-101.81818181818176,
					-54.545454545454504
				],
				[
					-85.4545454545455,
					-60
				],
				[
					-67.27272727272725,
					-63.63636363636351
				],
				[
					-49.09090909090901,
					-65.4545454545455
				],
				[
					-34.545454545454504,
					-65.4545454545455
				],
				[
					-21.818181818181756,
					-61.81818181818198
				],
				[
					-10.909090909090992,
					-56.36363636363649
				],
				[
					-5.454545454545496,
					-52.727272727272975
				],
				[
					-3.6363636363637397,
					-47.272727272727025
				],
				[
					-1.8181818181817562,
					-43.63636363636351
				],
				[
					0,
					-38.18181818181802
				],
				[
					0,
					-32.727272727272975
				],
				[
					0,
					-30.90909090909099
				],
				[
					0,
					-25.454545454545496
				],
				[
					-5.454545454545496,
					-23.636363636363512
				],
				[
					-10.909090909090992,
					-18.181818181818016
				],
				[
					-16.363636363636488,
					-12.727272727272975
				],
				[
					-23.63636363636374,
					-7.272727272727025
				],
				[
					-27.272727272727252,
					-3.6363636363635123
				],
				[
					-29.09090909090901,
					-3.6363636363635123
				],
				[
					-29.09090909090901,
					-3.6363636363635123
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				-29.09090909090901,
				-3.6363636363635123
			]
		},
		{
			"id": "3ZjuleYpulf-PwfOysa1D",
			"type": "freedraw",
			"x": -661.176179431734,
			"y": 1928.259252249487,
			"width": 110.90909090909099,
			"height": 41.81818181818153,
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
			"seed": 1931856157,
			"version": 24,
			"versionNonce": 42559763,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485675051,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181818699,
					0
				],
				[
					-5.454545454545496,
					0
				],
				[
					-16.363636363636374,
					0
				],
				[
					-29.090909090909122,
					3.6363636363635123
				],
				[
					-49.09090909090912,
					10.909090909090992
				],
				[
					-52.72727272727275,
					14.545454545454504
				],
				[
					-60,
					18.181818181818016
				],
				[
					-63.63636363636374,
					21.81818181818153
				],
				[
					-63.63636363636374,
					25.454545454545496
				],
				[
					-61.81818181818187,
					29.09090909090901
				],
				[
					-54.545454545454504,
					32.72727272727252
				],
				[
					-45.454545454545496,
					38.18181818181802
				],
				[
					-36.363636363636374,
					40
				],
				[
					-29.090909090909122,
					41.81818181818153
				],
				[
					-20,
					41.81818181818153
				],
				[
					-12.727272727272748,
					41.81818181818153
				],
				[
					-1.8181818181818699,
					41.81818181818153
				],
				[
					10.909090909090878,
					40
				],
				[
					23.636363636363626,
					36.36363636363649
				],
				[
					36.363636363636374,
					32.72727272727252
				],
				[
					47.27272727272725,
					30.90909090909099
				],
				[
					47.27272727272725,
					30.90909090909099
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				47.27272727272725,
				30.90909090909099
			]
		},
		{
			"id": "erqM-61B4m1J4gB6ULGmP",
			"type": "freedraw",
			"x": -561.176179431734,
			"y": 1955.531979522214,
			"width": 60,
			"height": 34.545454545454504,
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
			"seed": 1407952285,
			"version": 26,
			"versionNonce": 1304410675,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485675779,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.8181818181818699,
					0
				],
				[
					-3.636363636363626,
					0
				],
				[
					-9.090909090909122,
					0
				],
				[
					-18.181818181818244,
					0
				],
				[
					-27.272727272727252,
					-1.8181818181815288
				],
				[
					-36.363636363636374,
					-3.6363636363635123
				],
				[
					-40,
					-7.272727272727025
				],
				[
					-41.81818181818187,
					-10.909090909090537
				],
				[
					-41.81818181818187,
					-14.545454545454504
				],
				[
					-41.81818181818187,
					-21.81818181818153
				],
				[
					-34.545454545454504,
					-27.272727272727025
				],
				[
					-27.272727272727252,
					-32.72727272727252
				],
				[
					-18.181818181818244,
					-34.545454545454504
				],
				[
					-9.090909090909122,
					-34.545454545454504
				],
				[
					0,
					-32.72727272727252
				],
				[
					9.090909090909122,
					-27.272727272727025
				],
				[
					14.545454545454504,
					-23.636363636363512
				],
				[
					18.18181818181813,
					-18.181818181818016
				],
				[
					16.363636363636374,
					-18.181818181818016
				],
				[
					14.545454545454504,
					-18.181818181818016
				],
				[
					9.090909090909122,
					-18.181818181818016
				],
				[
					7.272727272727252,
					-18.181818181818016
				],
				[
					5.454545454545496,
					-16.363636363636033
				],
				[
					5.454545454545496,
					-16.363636363636033
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				5.454545454545496,
				-16.363636363636033
			]
		},
		{
			"id": "ZqLxugscz9Ni8bC6KBTvt",
			"type": "freedraw",
			"x": -497.5398157953704,
			"y": 1948.259252249487,
			"width": 61.818181818181756,
			"height": 61.818181818181756,
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
			"seed": 987133565,
			"version": 29,
			"versionNonce": 1322149821,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485676581,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.8181818181815288
				],
				[
					-3.636363636363626,
					3.6363636363635123
				],
				[
					-9.090909090909122,
					3.6363636363635123
				],
				[
					-16.363636363636374,
					3.6363636363635123
				],
				[
					-23.636363636363626,
					3.6363636363635123
				],
				[
					-32.72727272727275,
					-1.8181818181819835
				],
				[
					-40,
					-5.454545454545496
				],
				[
					-41.818181818181756,
					-9.090909090909008
				],
				[
					-41.818181818181756,
					-10.909090909090992
				],
				[
					-36.363636363636374,
					-12.727272727272748
				],
				[
					-25.454545454545496,
					-12.727272727272748
				],
				[
					-16.363636363636374,
					-12.727272727272748
				],
				[
					-7.272727272727252,
					-10.909090909090992
				],
				[
					-1.8181818181817562,
					-7.272727272727479
				],
				[
					3.636363636363626,
					-3.6363636363635123
				],
				[
					7.272727272727252,
					-1.8181818181819835
				],
				[
					10.909090909090878,
					1.8181818181815288
				],
				[
					12.727272727272748,
					1.8181818181815288
				],
				[
					14.545454545454504,
					1.8181818181815288
				],
				[
					14.545454545454504,
					0
				],
				[
					14.545454545454504,
					-9.090909090909008
				],
				[
					16.363636363636374,
					-21.818181818181984
				],
				[
					16.363636363636374,
					-34.545454545454504
				],
				[
					16.363636363636374,
					-47.27272727272748
				],
				[
					18.181818181818244,
					-54.545454545454504
				],
				[
					20,
					-58.181818181818244
				],
				[
					20,
					-58.181818181818244
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				20,
				-58.181818181818244
			]
		},
		{
			"id": "bE4Lo7fKH6hsFoQy4ktap",
			"type": "freedraw",
			"x": -446.6307248862795,
			"y": 1937.350161340396,
			"width": 94.54545454545462,
			"height": 30.90909090909099,
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
			"seed": 427474579,
			"version": 33,
			"versionNonce": 979482771,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485677380,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.6363636363637397,
					0
				],
				[
					12.727272727272748,
					-3.6363636363635123
				],
				[
					25.454545454545496,
					-7.272727272727252
				],
				[
					34.54545454545462,
					-12.727272727272748
				],
				[
					40,
					-18.181818181818016
				],
				[
					43.63636363636374,
					-21.818181818181756
				],
				[
					43.63636363636374,
					-27.272727272727252
				],
				[
					43.63636363636374,
					-29.09090909090901
				],
				[
					40,
					-29.09090909090901
				],
				[
					36.363636363636374,
					-30.90909090909099
				],
				[
					34.54545454545462,
					-30.90909090909099
				],
				[
					29.090909090909122,
					-30.90909090909099
				],
				[
					27.272727272727366,
					-29.09090909090901
				],
				[
					25.454545454545496,
					-25.454545454545496
				],
				[
					23.63636363636374,
					-20
				],
				[
					23.63636363636374,
					-14.545454545454504
				],
				[
					25.454545454545496,
					-9.090909090909008
				],
				[
					30.90909090909099,
					-7.272727272727252
				],
				[
					34.54545454545462,
					-5.454545454545496
				],
				[
					40,
					-1.8181818181817562
				],
				[
					43.63636363636374,
					-1.8181818181817562
				],
				[
					47.272727272727366,
					-1.8181818181817562
				],
				[
					52.72727272727275,
					0
				],
				[
					58.181818181818244,
					0
				],
				[
					67.27272727272737,
					0
				],
				[
					76.36363636363637,
					0
				],
				[
					83.63636363636374,
					0
				],
				[
					90.90909090909099,
					-1.8181818181817562
				],
				[
					92.72727272727275,
					-3.6363636363635123
				],
				[
					94.54545454545462,
					-3.6363636363635123
				],
				[
					94.54545454545462,
					-3.6363636363635123
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				94.54545454545462,
				-3.6363636363635123
			]
		},
		{
			"id": "ZHImiR6d5Z2qWA9QeVkse",
			"type": "freedraw",
			"x": -721.176179431734,
			"y": 1993.7137977040325,
			"width": 447.27272727272725,
			"height": 14.545454545454504,
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
			"seed": 1612844573,
			"version": 17,
			"versionNonce": 1573675293,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682485678234,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.8181818181817562,
					0
				],
				[
					3.636363636363626,
					0
				],
				[
					14.545454545454504,
					0
				],
				[
					43.636363636363626,
					0
				],
				[
					89.09090909090912,
					0
				],
				[
					152.72727272727275,
					0
				],
				[
					214.5454545454545,
					-1.8181818181819835
				],
				[
					276.3636363636364,
					-3.636363636363967
				],
				[
					329.0909090909091,
					-9.090909090909008
				],
				[
					374.5454545454546,
					-12.727272727272975
				],
				[
					407.27272727272725,
					-14.545454545454504
				],
				[
					430.9090909090909,
					-14.545454545454504
				],
				[
					445.4545454545455,
					-14.545454545454504
				],
				[
					447.27272727272725,
					-14.545454545454504
				],
				[
					447.27272727272725,
					-14.545454545454504
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				447.27272727272725,
				-14.545454545454504
			]
		},
		{
			"id": "uqpYut4e",
			"type": "text",
			"x": -704.8125430680976,
			"y": 2053.713797704032,
			"width": 755.5595092773438,
			"height": 550,
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
			"seed": 678591965,
			"version": 704,
			"versionNonce": 2096286515,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682486680813,
			"link": null,
			"locked": false,
			"text": "public void kthFromEnd(int k)throw IllegalArgumentException{\n     if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n      }\nNode temp = head;\nNode prevTemp = head;\nint i = 0;\n\nwhile (temp.next != null && i < k) { \n    for (int j = 0; j < k; j++) { \n        if (temp.next == null) break; \n        temp = temp.next; \n    }\n    i += k; // Update 'i' by adding 'k' after each iteration of the inner loop\n}\n\nwhile(temp != null){\nprevTemp = prevTemp.next;\ntemp = temp.next;\n}\nreturn preTemp.value;\n}",
			"rawText": "public void kthFromEnd(int k)throw IllegalArgumentException{\n     if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n      }\nNode temp = head;\nNode prevTemp = head;\nint i = 0;\n\nwhile (temp.next != null && i < k) { \n    for (int j = 0; j < k; j++) { \n        if (temp.next == null) break; \n        temp = temp.next; \n    }\n    i += k; // Update 'i' by adding 'k' after each iteration of the inner loop\n}\n\nwhile(temp != null){\nprevTemp = prevTemp.next;\ntemp = temp.next;\n}\nreturn preTemp.value;\n}",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 543,
			"containerId": null,
			"originalText": "public void kthFromEnd(int k)throw IllegalArgumentException{\n     if(head == null){\n        throw new IllegalArgumentException(\"value not in list\")\n      }\nNode temp = head;\nNode prevTemp = head;\nint i = 0;\n\nwhile (temp.next != null && i < k) { \n    for (int j = 0; j < k; j++) { \n        if (temp.next == null) break; \n        temp = temp.next; \n    }\n    i += k; // Update 'i' by adding 'k' after each iteration of the inner loop\n}\n\nwhile(temp != null){\nprevTemp = prevTemp.next;\ntemp = temp.next;\n}\nreturn preTemp.value;\n}",
			"lineHeight": 1.25
		},
		{
			"id": "CVmPveZD8xqqtCbcG33Rq",
			"type": "freedraw",
			"x": -961.176179431734,
			"y": 1991.8956158858505,
			"width": 200,
			"height": 130.909090909091,
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
			"seed": 1385416403,
			"version": 36,
			"versionNonce": 1517676093,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682486129060,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.8181818181817562,
					0
				],
				[
					3.6363636363635123,
					0
				],
				[
					12.727272727272634,
					-1.8181818181819835
				],
				[
					25.454545454545382,
					-1.8181818181819835
				],
				[
					47.27272727272725,
					-1.8181818181819835
				],
				[
					70.90909090909088,
					0
				],
				[
					89.09090909090901,
					1.8181818181819835
				],
				[
					105.4545454545455,
					7.272727272727252
				],
				[
					112.72727272727275,
					10.909090909090992
				],
				[
					120,
					16.363636363636488
				],
				[
					127.27272727272725,
					23.636363636363512
				],
				[
					134.5454545454545,
					34.545454545454504
				],
				[
					141.81818181818176,
					43.63636363636351
				],
				[
					147.27272727272725,
					54.545454545454504
				],
				[
					154.5454545454545,
					63.63636363636351
				],
				[
					160,
					74.5454545454545
				],
				[
					167.27272727272725,
					83.63636363636351
				],
				[
					172.72727272727275,
					90.90909090909099
				],
				[
					176.36363636363626,
					96.36363636363649
				],
				[
					181.81818181818176,
					103.63636363636351
				],
				[
					187.27272727272725,
					110.90909090909099
				],
				[
					190.90909090909088,
					116.36363636363649
				],
				[
					194.5454545454545,
					120
				],
				[
					198.18181818181813,
					123.63636363636351
				],
				[
					198.18181818181813,
					127.27272727272748
				],
				[
					200,
					127.27272727272748
				],
				[
					196.36363636363626,
					127.27272727272748
				],
				[
					187.27272727272725,
					127.27272727272748
				],
				[
					172.72727272727275,
					127.27272727272748
				],
				[
					156.36363636363626,
					129.090909090909
				],
				[
					143.63636363636363,
					129.090909090909
				],
				[
					134.5454545454545,
					129.090909090909
				],
				[
					132.72727272727275,
					129.090909090909
				],
				[
					132.72727272727275,
					129.090909090909
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				132.72727272727275,
				129.090909090909
			]
		},
		{
			"id": "8jlN-KuuTgxuzzRbC0Vtj",
			"type": "freedraw",
			"x": -764.8125430680977,
			"y": 2117.350161340396,
			"width": 25.454545454545496,
			"height": 69.09090909090901,
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
			"seed": 485517331,
			"version": 15,
			"versionNonce": 1475136371,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682486129761,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.8181818181818699,
					0
				],
				[
					1.8181818181818699,
					-1.8181818181819835
				],
				[
					3.6363636363637397,
					-1.8181818181819835
				],
				[
					9.090909090909236,
					-7.272727272727025
				],
				[
					14.545454545454618,
					-16.363636363636488
				],
				[
					18.181818181818244,
					-25.454545454545496
				],
				[
					23.63636363636374,
					-36.36363636363649
				],
				[
					25.454545454545496,
					-47.272727272727025
				],
				[
					25.454545454545496,
					-58.18181818181802
				],
				[
					25.454545454545496,
					-63.63636363636351
				],
				[
					25.454545454545496,
					-67.27272727272702
				],
				[
					25.454545454545496,
					-69.09090909090901
				],
				[
					25.454545454545496,
					-69.09090909090901
				]
			],
			"pressures": [],
			"simulatePressure": true,
			"lastCommittedPoint": [
				25.454545454545496,
				-69.09090909090901
			]
		},
		{
			"id": "wVikPDML",
			"type": "text",
			"x": -1132.085270340825,
			"y": 1955.531979522214,
			"width": 348.459716796875,
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
			"seed": 44964157,
			"version": 55,
			"versionNonce": 2134846397,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1682486139409,
			"link": null,
			"locked": false,
			"text": "not sure how to handle edge cases",
			"rawText": "not sure how to handle edge cases",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "not sure how to handle edge cases",
			"lineHeight": 1.25
		},
		{
			"id": "eMwc1Jtz",
			"type": "text",
			"x": 445.1874569319027,
			"y": 1766.8956158858507,
			"width": 10,
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
			"seed": 726397715,
			"version": 2,
			"versionNonce": 1978579869,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1682485586691,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
		},
		{
			"id": "CFxhmYsA",
			"type": "text",
			"x": -755.7216339771885,
			"y": 1993.7137977040325,
			"width": 10,
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
			"seed": 2009908211,
			"version": 2,
			"versionNonce": 1263003837,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1682485672341,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
		},
		{
			"id": "LoStF1MC",
			"type": "text",
			"x": -659.3579976135522,
			"y": 2039.168343158578,
			"width": 10,
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
			"seed": 2088471347,
			"version": 2,
			"versionNonce": 1128019325,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1682485681868,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
		},
		{
			"id": "uxSZAUTZ",
			"type": "text",
			"x": 104.2783660228115,
			"y": 1890.0774340676685,
			"width": 10,
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
			"seed": 1826391165,
			"version": 2,
			"versionNonce": 1081724371,
			"isDeleted": true,
			"boundElements": null,
			"updated": 1682486375625,
			"link": null,
			"locked": false,
			"text": "",
			"rawText": "",
			"fontSize": 20,
			"fontFamily": 1,
			"textAlign": "left",
			"verticalAlign": "top",
			"baseline": 18,
			"containerId": null,
			"originalText": "",
			"lineHeight": 1.25
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
		"scrollX": 1182.085270340825,
		"scrollY": -1461.8672067949412,
		"zoom": {
			"value": 0.5499999999999999
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