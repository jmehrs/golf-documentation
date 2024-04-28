---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
Assign Hole ^I1RyDEFf

Swap Hole
Assignments ^KFTg30wK

Un-assign Hole ^isnarPrV

Hole Assigning ^kP8p4DSD

Start Hole ^XR29vvuZ

Stop Hole ^PpP8Gt3C

Hole-specific Controls ^XK2YoUiU

Get all Hole
Assignments ^L4iZQorh

These should leverage the K/V
store of NATS Jetstream. This
also allows other applications to
access the store. ^lBxN5t61

These can publish to appropriate
NATS topics (e.g., "course.hole1.start"). ^XAT5LSys

Hole Assignment Task ^Lqb35G0A

Listen to Hole
pings ^a0HxbDHZ

HTTP Server Task ^laMPjF8l

Listen to HTTP
client connections ^HjrUyvz0

This can listen to an appropriate
NATS topic (e.g., "hole.*.ping").
The wildcard (*) in the topic should
be the client's UID (letters & numbers only). ^0WFQTs6v

Assigns Client to a Hole #.
There should be logic around
limit hole assignments to 18
holes. Any further requests
should be ignored/denied. ^nTIeP5ms

These don't necessarily need to 
be in the same process/language.
This is bc the application state
should reside in the NATS
Jetstream K/V store. ^EKLqlbfI

This should serve the client some
HTML/JSON payload based on the
route and method requested.
Should expose all server functions.
Can expose additional task-specific
sub-tasks (e.g., listening to
K/V store updates & updating clients
via Websockets/SSR). ^SYapg1YQ

Server ^jj6pUgU5

The server is comprised of a set of shared functions which are primarily accessed via a CLI
and a few tasks:
    - listen on <hole / * / ping>
        - stores the id 
    - when prompted (UI/cli/etc..), will re-assign/un-assign hole #
      to/from the specified id in the NATS Jetstream K/V store ^p3WWf4aO

CLI should expose commands that map to all
server functions ^L7dbjOGK

Start Client ^mgin3XoV

Stop Client ^PH44gAuN

Client Controls ^tRkZMS2w

Client ^2u1c1ZxW

The server is comprised of a set of shared functions which are primarily accessed via a CLI
and a few tasks. ^ns5D4lp1

Send Ping ^6DC7zhVe

Client Discovery ^qUNDdOzJ

These control the starting/stopping
of local processes & any connected
peripheral. ^j1lX6GSY

Course Event Tasks ^PFXIAxXQ

Listen to Course
start/stop events ^rjQr3gYT

This can listen to an appropriate
NATS topic (e.g., "course.client_id.start").
The wildcard (*) in the topic should
be the client's UID (letters & numbers only). ^9BlSwu36

Calls the appropriate Client
Control function ^naCu77BJ

Clients/Holes ^biKj4CuZ

The client is comprised of a set of functions and a listener task:
    - generate a UID on boot (or perhaps hardcode/configured?)
    - listen on <course / client_id / *> and take appropriate action
      for each message type
    - publishes a <hole / client_id / ping> to make the server aware of it ^KnnWgrFM

These can publish to appropriate
NATS topics (e.g., "hole.hole_id.ping"). ^iF6MfDt5

Participant ^AHzVCKq4

map to azure token / unique microsoft ID (?) -- can get profile picture / name

map to course_<id> : time participant started course_<id>

map to course_<id> : time participant ended course_<id>

map to course_<id> : elapsed time of participant at course_<id>

map to course_<id> : [1/0] if participant has a start and end time tracked for hole ^LDZ2ejMs

participant_id

start_time

end_time

elapsed_time

completed ^tmbRlnul

Proximity Sensor ^BFoxYtJ6

Microcontroller
Home ^WNIfwc9w

Micro-controllers ^zPXtDgqV

Jai







Bradley








Rowan ^BSU3MdP8


# Embedded files
101a012f112bb18a111fd006f1f71ca3c312a903: [[jai-microcontroller-selection.png]]

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/2.0.25",
	"elements": [
		{
			"type": "rectangle",
			"version": 308,
			"versionNonce": 1207628272,
			"isDeleted": false,
			"id": "kaZf_1BHN6heO6TTc9JOE",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -388.87313729737616,
			"y": 166.32983559981028,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 1524942608,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "I1RyDEFf"
				},
				{
					"id": "S_rBNNYAK8TRDbOM9fjLs",
					"type": "arrow"
				},
				{
					"id": "_S8JvRk-jszNpCxgaX7Hc",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 298,
			"versionNonce": 1739427312,
			"isDeleted": false,
			"id": "I1RyDEFf",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -358.53476331761726,
			"y": 185.94987063772084,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 85.375,
			"height": 18.4,
			"seed": 2128176400,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690852,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Assign Hole",
			"rawText": "Assign Hole",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "kaZf_1BHN6heO6TTc9JOE",
			"originalText": "Assign Hole",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "rectangle",
			"version": 471,
			"versionNonce": 8074736,
			"isDeleted": false,
			"id": "r4Wu2BI3kdJcmKPYQGStn",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -386.5312328046566,
			"y": 320.57961132012804,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 915030800,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "KFTg30wK"
				},
				{
					"id": "4rSqnYDRauW6SaonUc64H",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 441,
			"versionNonce": 1218858992,
			"isDeleted": false,
			"id": "KFTg30wK",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -359.3022338248977,
			"y": 330.9996463580386,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91.59375,
			"height": 36.8,
			"seed": 1081041168,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690852,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Swap Hole\nAssignments",
			"rawText": "Swap Hole\nAssignments",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "r4Wu2BI3kdJcmKPYQGStn",
			"originalText": "Swap Hole\nAssignments",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "rectangle",
			"version": 485,
			"versionNonce": 12220912,
			"isDeleted": false,
			"id": "HzWZ3zEyZufA3ZzZ7zrpX",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -386.6785674269122,
			"y": 242.9390311741248,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 1275117328,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "isnarPrV"
				},
				{
					"id": "YBKcosaoMjRSsgpm4UpnB",
					"type": "arrow"
				},
				{
					"id": "KmKqclwnwaXrJcDtR17Gk",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 473,
			"versionNonce": 1362547184,
			"isDeleted": false,
			"id": "isnarPrV",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -368.3440996971533,
			"y": 262.55906621203536,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 109.3828125,
			"height": 18.4,
			"seed": 1505123600,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690853,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Un-assign Hole",
			"rawText": "Un-assign Hole",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "HzWZ3zEyZufA3ZzZ7zrpX",
			"originalText": "Un-assign Hole",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "text",
			"version": 117,
			"versionNonce": 620281328,
			"isDeleted": false,
			"id": "kP8p4DSD",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -366.26451494998173,
			"y": 118.8854212088678,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 106.7265625,
			"height": 18.4,
			"seed": 453524240,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Hole Assigning",
			"rawText": "Hole Assigning",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Hole Assigning",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "line",
			"version": 289,
			"versionNonce": 353075184,
			"isDeleted": false,
			"id": "F1ZsfNGMygIvpzWsNWmi_",
			"fillStyle": "cross-hatch",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 20,
			"angle": 0,
			"x": -208.59843589628463,
			"y": 110.42991211135143,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 357.22293845320587,
			"seed": 1382963472,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					357.22293845320587
				]
			]
		},
		{
			"type": "rectangle",
			"version": 398,
			"versionNonce": 964035056,
			"isDeleted": false,
			"id": "vw_T5sYL3ySMxS8hIMMJr",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -172.18715522089315,
			"y": 168.7817955490217,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 861976336,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "XR29vvuZ"
				},
				{
					"id": "jZp1kePpoVf9lxFRzcLWs",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 400,
			"versionNonce": 946279408,
			"isDeleted": false,
			"id": "XR29vvuZ",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -134.73159374113428,
			"y": 188.40183058693225,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 71.140625,
			"height": 18.4,
			"seed": 1113019664,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690853,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Start Hole",
			"rawText": "Start Hole",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "vw_T5sYL3ySMxS8hIMMJr",
			"originalText": "Start Hole",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "rectangle",
			"version": 589,
			"versionNonce": 2054309360,
			"isDeleted": false,
			"id": "4s8qfgwyDcO4j2l50Huke",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -172.4374842659272,
			"y": 243.6120025959125,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 885666576,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "PpP8Gt3C"
				},
				{
					"id": "tGTVkq7K75K7PKRCWcA7f",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 588,
			"versionNonce": 339678704,
			"isDeleted": false,
			"id": "PpP8Gt3C",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -134.54442278616833,
			"y": 263.23203763382304,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 70.265625,
			"height": 18.4,
			"seed": 1362186512,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690853,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Stop Hole",
			"rawText": "Stop Hole",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "4s8qfgwyDcO4j2l50Huke",
			"originalText": "Stop Hole",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "text",
			"version": 181,
			"versionNonce": 338528752,
			"isDeleted": false,
			"id": "XK2YoUiU",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -178.68388846239668,
			"y": 118.53899437317602,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 155.609375,
			"height": 18.4,
			"seed": 1325707024,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Hole-specific Controls",
			"rawText": "Hole-specific Controls",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Hole-specific Controls",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "rectangle",
			"version": 501,
			"versionNonce": 1539754992,
			"isDeleted": false,
			"id": "qi1wgpL9eHA0HXeNc9_tL",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -386.50637467324304,
			"y": 400.76081969635777,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 918310160,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "L4iZQorh"
				},
				{
					"id": "L8W8b93BkTg9nH2b0o1o4",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 507,
			"versionNonce": 2043074544,
			"isDeleted": false,
			"id": "L4iZQorh",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -359.27737569348415,
			"y": 411.18085473426834,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 91.59375,
			"height": 36.8,
			"seed": 1104161552,
			"groupIds": [],
			"frameId": "WjaAVyY30km1xdoBeyfVu",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690853,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Get all Hole\nAssignments",
			"rawText": "Get all Hole\nAssignments",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "qi1wgpL9eHA0HXeNc9_tL",
			"originalText": "Get all Hole\nAssignments",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "frame",
			"version": 248,
			"versionNonce": 580423664,
			"isDeleted": false,
			"id": "WjaAVyY30km1xdoBeyfVu",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -437.1658684712529,
			"y": 82.2123416227547,
			"strokeColor": "#bbb",
			"backgroundColor": "transparent",
			"width": 463.71109187316773,
			"height": 415.562242360838,
			"seed": 985155856,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "KmKqclwnwaXrJcDtR17Gk",
					"type": "arrow"
				},
				{
					"id": "Blya_4nxQfFQnRoh4yvr9",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"customData": {
				"frameColor": {
					"stroke": "#2B2B2B",
					"fill": "#525252",
					"nameColor": "#858585"
				}
			},
			"name": "Server Functions"
		},
		{
			"type": "arrow",
			"version": 271,
			"versionNonce": 1330531088,
			"isDeleted": false,
			"id": "S_rBNNYAK8TRDbOM9fjLs",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -539.8505970121846,
			"y": 30.054985140303074,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 140.17278479493848,
			"height": 170.32626865517597,
			"seed": 1559013136,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260691246,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "lBxN5t61",
				"focus": 0.03626569651808894,
				"gap": 8.71074707814364
			},
			"endBinding": {
				"elementId": "kaZf_1BHN6heO6TTc9JOE",
				"gap": 10.804674919869967,
				"focus": -0.3977823035382638
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
					4.074790074921566,
					154.8420228470202
				],
				[
					140.17278479493848,
					170.32626865517597
				]
			]
		},
		{
			"type": "text",
			"version": 268,
			"versionNonce": 1791579120,
			"isDeleted": false,
			"id": "lBxN5t61",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -649.8699290350669,
			"y": -52.255761937840475,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 225.90625,
			"height": 73.6,
			"seed": 887440656,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "YBKcosaoMjRSsgpm4UpnB",
					"type": "arrow"
				},
				{
					"id": "4rSqnYDRauW6SaonUc64H",
					"type": "arrow"
				},
				{
					"id": "S_rBNNYAK8TRDbOM9fjLs",
					"type": "arrow"
				},
				{
					"id": "L8W8b93BkTg9nH2b0o1o4",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "These should leverage the K/V\nstore of NATS Jetstream. This\nalso allows other applications to\naccess the store.",
			"rawText": "These should leverage the K/V\nstore of NATS Jetstream. This\nalso allows other applications to\naccess the store.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "These should leverage the K/V\nstore of NATS Jetstream. This\nalso allows other applications to\naccess the store.",
			"lineHeight": 1.15,
			"baseline": 70
		},
		{
			"type": "arrow",
			"version": 414,
			"versionNonce": 496461072,
			"isDeleted": false,
			"id": "YBKcosaoMjRSsgpm4UpnB",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -539.7156776439774,
			"y": 30.996820045720938,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 146.55755441715178,
			"height": 246.80538299690596,
			"seed": 1712912,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260691247,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "lBxN5t61",
				"focus": 0.029161498692513478,
				"gap": 9.652581983561504
			},
			"endBinding": {
				"elementId": "HzWZ3zEyZufA3ZzZ7zrpX",
				"gap": 6.479555799913442,
				"focus": -0.5446214658537475
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
					2.3099484591100463,
					211.7622256583977
				],
				[
					146.55755441715178,
					246.80538299690596
				]
			]
		},
		{
			"type": "arrow",
			"version": 479,
			"versionNonce": 2036516624,
			"isDeleted": false,
			"id": "4rSqnYDRauW6SaonUc64H",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -540.067579048191,
			"y": 30.181874466009162,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 151.58220943999254,
			"height": 321.7815576812805,
			"seed": 218317072,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260691247,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "lBxN5t61",
				"focus": 0.021121056014457813,
				"gap": 8.837636403849729
			},
			"endBinding": {
				"elementId": "r4Wu2BI3kdJcmKPYQGStn",
				"gap": 6.626890422168799,
				"focus": -0.4800033461920883
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
					-4.6727536186269845,
					283.4784936712001
				],
				[
					146.90945582136555,
					321.7815576812805
				]
			]
		},
		{
			"type": "text",
			"version": 401,
			"versionNonce": 932223472,
			"isDeleted": false,
			"id": "XAT5LSys",
			"fillStyle": "cross-hatch",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -48.43081915768926,
			"y": -52.065634966759376,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 281.390625,
			"height": 36.8,
			"seed": 454598416,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "jZp1kePpoVf9lxFRzcLWs",
					"type": "arrow"
				},
				{
					"id": "tGTVkq7K75K7PKRCWcA7f",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "These can publish to appropriate\nNATS topics (e.g., \"course.hole1.start\").",
			"rawText": "These can publish to appropriate\nNATS topics (e.g., \"course.hole1.start\").",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "These can publish to appropriate\nNATS topics (e.g., \"course.hole1.start\").",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "arrow",
			"version": 490,
			"versionNonce": 1300775696,
			"isDeleted": false,
			"id": "jZp1kePpoVf9lxFRzcLWs",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": 93.62322831510573,
			"y": -4.798045227123907,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 118.90463173801464,
			"height": 202.0076063236105,
			"seed": 986856720,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260691248,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "XAT5LSys",
				"focus": 0.000413518891838442,
				"gap": 10.467589739635514
			},
			"endBinding": {
				"elementId": "vw_T5sYL3ySMxS8hIMMJr",
				"gap": 9.567126961407439,
				"focus": 0.37939739754866025
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
					8.713123122940942,
					177.47044982832404
				],
				[
					-110.1915086150737,
					202.0076063236105
				]
			]
		},
		{
			"type": "arrow",
			"version": 580,
			"versionNonce": 1202544912,
			"isDeleted": false,
			"id": "tGTVkq7K75K7PKRCWcA7f",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": 93.97249188282967,
			"y": -5.816680569492405,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 127.869095291208,
			"height": 276.000419957909,
			"seed": 765991696,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260691248,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "XAT5LSys",
				"focus": 0.002218629793984437,
				"gap": 9.448954397267016
			},
			"endBinding": {
				"elementId": "4s8qfgwyDcO4j2l50Huke",
				"gap": 9.999515275766953,
				"focus": 0.41923338163954754
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
					17.510382377735823,
					241.03713769128308
				],
				[
					-110.35871291347217,
					276.000419957909
				]
			]
		},
		{
			"type": "text",
			"version": 250,
			"versionNonce": 102080496,
			"isDeleted": false,
			"id": "Lqb35G0A",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1201.6036851526487,
			"y": 207.20186413441263,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 158.2890625,
			"height": 18.4,
			"seed": 1175599376,
			"groupIds": [],
			"frameId": "EQQHrioA-hwh3vOGbUBEi",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Hole Assignment Task",
			"rawText": "Hole Assignment Task",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Hole Assignment Task",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "rectangle",
			"version": 713,
			"versionNonce": 1144791536,
			"isDeleted": false,
			"id": "5c5UdQmtrwqfQXau3GcEU",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1199.7074873153479,
			"y": 235.0179601136623,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 1200133904,
			"groupIds": [],
			"frameId": "EQQHrioA-hwh3vOGbUBEi",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "a0HxbDHZ"
				},
				{
					"id": "EwH6tXCVc0MMTZvAOVJIp",
					"type": "arrow"
				},
				{
					"id": "_S8JvRk-jszNpCxgaX7Hc",
					"type": "arrow"
				},
				{
					"id": "l-sEn9Lw_IUn4jyAAIExe",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 751,
			"versionNonce": 486955504,
			"isDeleted": false,
			"id": "a0HxbDHZ",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1175.599582085589,
			"y": 245.43799515157284,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 97.8359375,
			"height": 36.8,
			"seed": 1183003920,
			"groupIds": [],
			"frameId": "EQQHrioA-hwh3vOGbUBEi",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690854,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Listen to Hole\npings",
			"rawText": "Listen to Hole\npings",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "5c5UdQmtrwqfQXau3GcEU",
			"originalText": "Listen to Hole\npings",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "line",
			"version": 498,
			"versionNonce": 1647338992,
			"isDeleted": false,
			"id": "1k4MLY7TQ9RDuR6Va7D5L",
			"fillStyle": "cross-hatch",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 20,
			"angle": 0,
			"x": -1220.474407470756,
			"y": 318.6968122232548,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 193.22739867801783,
			"height": 0,
			"seed": 142218000,
			"groupIds": [],
			"frameId": "EQQHrioA-hwh3vOGbUBEi",
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					193.22739867801783,
					0
				]
			]
		},
		{
			"type": "text",
			"version": 309,
			"versionNonce": 487466992,
			"isDeleted": false,
			"id": "laMPjF8l",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1190.2132491506472,
			"y": 333.30034939767813,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 130.6875,
			"height": 18.4,
			"seed": 1675964688,
			"groupIds": [],
			"frameId": "EQQHrioA-hwh3vOGbUBEi",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "HTTP Server Task",
			"rawText": "HTTP Server Task",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "HTTP Server Task",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "rectangle",
			"version": 774,
			"versionNonce": 2061740528,
			"isDeleted": false,
			"id": "YOBiaOVRlnWplBu_uJ1Dx",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1197.8226543281398,
			"y": 361.1164453769278,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 540839696,
			"groupIds": [],
			"frameId": "EQQHrioA-hwh3vOGbUBEi",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "HjrUyvz0"
				},
				{
					"id": "Ad4v_uQBTgkTdhAcsrNGC",
					"type": "arrow"
				},
				{
					"id": "KmKqclwnwaXrJcDtR17Gk",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 839,
			"versionNonce": 1896193008,
			"isDeleted": false,
			"id": "HjrUyvz0",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1188.390530348381,
			"y": 371.53648041483837,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 127.1875,
			"height": 36.8,
			"seed": 1442327824,
			"groupIds": [],
			"frameId": "EQQHrioA-hwh3vOGbUBEi",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690854,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Listen to HTTP\nclient connections",
			"rawText": "Listen to HTTP\nclient connections",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "YOBiaOVRlnWplBu_uJ1Dx",
			"originalText": "Listen to HTTP\nclient connections",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "frame",
			"version": 505,
			"versionNonce": 714468848,
			"isDeleted": false,
			"id": "EQQHrioA-hwh3vOGbUBEi",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1238.853987252358,
			"y": 191.33747812150398,
			"strokeColor": "#bbb",
			"backgroundColor": "transparent",
			"width": 232.07289030113623,
			"height": 263.32401351356816,
			"seed": 1318062864,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "EwH6tXCVc0MMTZvAOVJIp",
					"type": "arrow"
				},
				{
					"id": "l-sEn9Lw_IUn4jyAAIExe",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"customData": {
				"frameColor": {
					"stroke": "#2B2B2B",
					"fill": "#525252",
					"nameColor": "#858585"
				}
			},
			"name": "Server Tasks"
		},
		{
			"type": "arrow",
			"version": 1889,
			"versionNonce": 1333964784,
			"isDeleted": false,
			"id": "EwH6tXCVc0MMTZvAOVJIp",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1376.3399396936748,
			"y": 190.82430363044784,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 167.6416931215067,
			"height": 77.05772366008978,
			"seed": 1685858576,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "0WFQTs6v",
				"focus": -0.21063918038107507,
				"gap": 8.710747078143413
			},
			"endBinding": {
				"elementId": "EQQHrioA-hwh3vOGbUBEi",
				"focus": 0.374735357941738,
				"gap": 1
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
					23.26188797172881,
					70.60786088722102
				],
				[
					167.6416931215067,
					77.05772366008978
				]
			]
		},
		{
			"type": "text",
			"version": 1059,
			"versionNonce": 2106012144,
			"isDeleted": false,
			"id": "0WFQTs6v",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1580.363557149285,
			"y": 108.51355655230452,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 308.0625,
			"height": 73.6,
			"seed": 1664386832,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "EwH6tXCVc0MMTZvAOVJIp",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "This can listen to an appropriate\nNATS topic (e.g., \"hole.*.ping\").\nThe wildcard (*) in the topic should\nbe the client's UID (letters & numbers only).",
			"rawText": "This can listen to an appropriate\nNATS topic (e.g., \"hole.*.ping\").\nThe wildcard (*) in the topic should\nbe the client's UID (letters & numbers only).",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "This can listen to an appropriate\nNATS topic (e.g., \"hole.*.ping\").\nThe wildcard (*) in the topic should\nbe the client's UID (letters & numbers only).",
			"lineHeight": 1.15,
			"baseline": 70
		},
		{
			"type": "arrow",
			"version": 848,
			"versionNonce": 695491856,
			"isDeleted": false,
			"id": "_S8JvRk-jszNpCxgaX7Hc",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1048.0574964298223,
			"y": 239.3988061472762,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 649.6367988006039,
			"height": 40.26588893422945,
			"seed": 1731274000,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "nTIeP5ms"
				}
			],
			"updated": 1714260691249,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "5c5UdQmtrwqfQXau3GcEU",
				"gap": 5.598242926007742,
				"focus": -0.4578076657718136
			},
			"endBinding": {
				"elementId": "kaZf_1BHN6heO6TTc9JOE",
				"gap": 9.547560331842305,
				"focus": -0.04164492083484937
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
					282.2441054292856,
					-28.32406315050079
				],
				[
					649.6367988006039,
					-40.26588893422945
				]
			]
		},
		{
			"type": "text",
			"version": 231,
			"versionNonce": 1204592112,
			"isDeleted": false,
			"id": "nTIeP5ms",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -869.4383910005367,
			"y": 165.0747429967754,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 207.25,
			"height": 92,
			"seed": 1038746384,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690854,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Assigns Client to a Hole #.\nThere should be logic around\nlimit hole assignments to 18\nholes. Any further requests\nshould be ignored/denied.",
			"rawText": "Assigns Client to a Hole #.\nThere should be logic around\nlimit hole assignments to 18\nholes. Any further requests\nshould be ignored/denied.",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "_S8JvRk-jszNpCxgaX7Hc",
			"originalText": "Assigns Client to a Hole #.\nThere should be logic around\nlimit hole assignments to 18\nholes. Any further requests\nshould be ignored/denied.",
			"lineHeight": 1.15,
			"baseline": 88
		},
		{
			"type": "arrow",
			"version": 1063,
			"versionNonce": 2138257392,
			"isDeleted": false,
			"id": "l-sEn9Lw_IUn4jyAAIExe",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1432.0122360845735,
			"y": 448.06343385118623,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 222.25737864698965,
			"height": 181.64680110753534,
			"seed": 1171726608,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "EKLqlbfI",
				"focus": 0.019055643820483165,
				"gap": 6.645286975939143
			},
			"endBinding": {
				"elementId": "EQQHrioA-hwh3vOGbUBEi",
				"focus": 0.4619782500636212,
				"gap": 1
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
					38.45025554389497,
					-158.25314581736416
				],
				[
					222.25737864698965,
					-181.64680110753534
				]
			]
		},
		{
			"type": "arrow",
			"version": 1243,
			"versionNonce": 1124481808,
			"isDeleted": false,
			"id": "Ad4v_uQBTgkTdhAcsrNGC",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1434.3304658650268,
			"y": 449.66279279670937,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 230.4240222499859,
			"height": 60.01184431427265,
			"seed": 1315995408,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260691249,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "EKLqlbfI",
				"focus": -0.16040658976924832,
				"gap": 5.0459280304160075
			},
			"endBinding": {
				"elementId": "YOBiaOVRlnWplBu_uJ1Dx",
				"gap": 6.0837892869010375,
				"focus": 0.11088526737503304
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
					38.494560175750394,
					-52.146286724365154
				],
				[
					230.4240222499859,
					-60.01184431427265
				]
			]
		},
		{
			"type": "text",
			"version": 1405,
			"versionNonce": 2132409328,
			"isDeleted": false,
			"id": "EKLqlbfI",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1567.3825572094538,
			"y": 454.7087208271254,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 240.15625,
			"height": 92,
			"seed": 2016288016,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "l-sEn9Lw_IUn4jyAAIExe",
					"type": "arrow"
				},
				{
					"id": "Ad4v_uQBTgkTdhAcsrNGC",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "These don't necessarily need to \nbe in the same process/language.\nThis is bc the application state\nshould reside in the NATS\nJetstream K/V store.",
			"rawText": "These don't necessarily need to \nbe in the same process/language.\nThis is bc the application state\nshould reside in the NATS\nJetstream K/V store.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "These don't necessarily need to \nbe in the same process/language.\nThis is bc the application state\nshould reside in the NATS\nJetstream K/V store.",
			"lineHeight": 1.15,
			"baseline": 88
		},
		{
			"type": "arrow",
			"version": 1180,
			"versionNonce": 1252808976,
			"isDeleted": false,
			"id": "KmKqclwnwaXrJcDtR17Gk",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1045.7337281220018,
			"y": 393.486492184285,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 597.5409558489271,
			"height": 59.10400104999201,
			"seed": 344455952,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "SYapg1YQ"
				}
			],
			"updated": 1714260691249,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "YOBiaOVRlnWplBu_uJ1Dx",
				"gap": 6.037178246620215,
				"focus": -0.25044289409753906
			},
			"endBinding": {
				"elementId": "WjaAVyY30km1xdoBeyfVu",
				"focus": -0.7916785125362534,
				"gap": 11.026903801821618
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
					275.3941251592428,
					48.79344625021429
				],
				[
					597.5409558489271,
					59.10400104999201
				]
			]
		},
		{
			"type": "text",
			"version": 780,
			"versionNonce": 1919115248,
			"isDeleted": false,
			"id": "SYapg1YQ",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -899.308352962759,
			"y": 368.67993843449926,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 257.9375,
			"height": 147.2,
			"seed": 100014352,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690855,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "This should serve the client some\nHTML/JSON payload based on the\nroute and method requested.\nShould expose all server functions.\nCan expose additional task-specific\nsub-tasks (e.g., listening to\nK/V store updates & updating clients\nvia Websockets/SSR).",
			"rawText": "This should serve the client some\nHTML/JSON payload based on the\nroute and method requested.\nShould expose all server functions.\nCan expose additional task-specific\nsub-tasks (e.g., listening to\nK/V store updates & updating clients\nvia Websockets/SSR).",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "KmKqclwnwaXrJcDtR17Gk",
			"originalText": "This should serve the client some\nHTML/JSON payload based on the\nroute and method requested.\nShould expose all server functions.\nCan expose additional task-specific\nsub-tasks (e.g., listening to\nK/V store updates & updating clients\nvia Websockets/SSR).",
			"lineHeight": 1.15,
			"baseline": 143
		},
		{
			"type": "arrow",
			"version": 590,
			"versionNonce": 998162192,
			"isDeleted": false,
			"id": "L8W8b93BkTg9nH2b0o1o4",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -540.6327362930533,
			"y": 27.570012836141927,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 153.84357712521933,
			"height": 398.66922356521786,
			"seed": 535852816,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260691248,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "lBxN5t61",
				"focus": 0.023649394871261158,
				"gap": 6.225774773982494
			},
			"endBinding": {
				"elementId": "qi1wgpL9eHA0HXeNc9_tL",
				"gap": 8.347675906705263,
				"focus": -0.4944406805233008
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
					-8.06489141211432,
					338.88282148289704
				],
				[
					145.778685713105,
					398.66922356521786
				]
			]
		},
		{
			"type": "rectangle",
			"version": 110,
			"versionNonce": 1929675760,
			"isDeleted": false,
			"id": "qx_v1X_YcUgQR_GhisaCN",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1706.3438661551827,
			"y": -406.57973001830703,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1965.1966241880336,
			"height": 986.4291007813285,
			"seed": 116331792,
			"groupIds": [
				"EoIlmc-3X1NjNsd_pCe_Z"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 121,
			"versionNonce": 2041480688,
			"isDeleted": false,
			"id": "jj6pUgU5",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1690.2985695502066,
			"y": -533.3824226200976,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 316.4737548828125,
			"height": 123.57667288199637,
			"seed": 275378960,
			"groupIds": [
				"EoIlmc-3X1NjNsd_pCe_Z"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 107.45797641912729,
			"fontFamily": 2,
			"text": "Server",
			"rawText": "Server",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Server",
			"lineHeight": 1.15,
			"baseline": 99
		},
		{
			"type": "text",
			"version": 581,
			"versionNonce": 1606961136,
			"isDeleted": false,
			"id": "p3WWf4aO",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1664.1595109419413,
			"y": -372.45349038870324,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1450.6171875,
			"height": 248.39999999999998,
			"seed": 584651024,
			"groupIds": [
				"EoIlmc-3X1NjNsd_pCe_Z"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "The server is comprised of a set of shared functions which are primarily accessed via a CLI\nand a few tasks:\n    - listen on <hole / * / ping>\n        - stores the id \n    - when prompted (UI/cli/etc..), will re-assign/un-assign hole #\n      to/from the specified id in the NATS Jetstream K/V store",
			"rawText": "The server is comprised of a set of shared functions which are primarily accessed via a CLI\nand a few tasks:\n    - listen on <hole / * / ping>\n        - stores the id \n    - when prompted (UI/cli/etc..), will re-assign/un-assign hole #\n      to/from the specified id in the NATS Jetstream K/V store",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "The server is comprised of a set of shared functions which are primarily accessed via a CLI\nand a few tasks:\n    - listen on <hole / * / ping>\n        - stores the id \n    - when prompted (UI/cli/etc..), will re-assign/un-assign hole #\n      to/from the specified id in the NATS Jetstream K/V store",
			"lineHeight": 1.15,
			"baseline": 240
		},
		{
			"type": "text",
			"version": 108,
			"versionNonce": 559532528,
			"isDeleted": false,
			"id": "L7dbjOGK",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -412.49218334487387,
			"y": -179.54021565248547,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 400.21484375,
			"height": 46,
			"seed": 364146448,
			"groupIds": [],
			"frameId": "gmWyZQjWILFJY1E-YjVjk",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "CLI should expose commands that map to all\nserver functions",
			"rawText": "CLI should expose commands that map to all\nserver functions",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "CLI should expose commands that map to all\nserver functions",
			"lineHeight": 1.15,
			"baseline": 41
		},
		{
			"type": "frame",
			"version": 143,
			"versionNonce": 2037058544,
			"isDeleted": false,
			"id": "gmWyZQjWILFJY1E-YjVjk",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -436.5796643821618,
			"y": -202.28262368740195,
			"strokeColor": "#bbb",
			"backgroundColor": "transparent",
			"width": 471.1875748052069,
			"height": 91.93907462860852,
			"seed": 292818192,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "Blya_4nxQfFQnRoh4yvr9",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"customData": {
				"frameColor": {
					"stroke": "#2B2B2B",
					"fill": "#525252",
					"nameColor": "#858585"
				}
			},
			"name": "CLI"
		},
		{
			"type": "arrow",
			"version": 54,
			"versionNonce": 33820144,
			"isDeleted": false,
			"id": "Blya_4nxQfFQnRoh4yvr9",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -212.9570505679385,
			"y": -105.13615939040562,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 186.15842594339142,
			"seed": 1871702800,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "gmWyZQjWILFJY1E-YjVjk",
				"focus": 0.050812772783021654,
				"gap": 5.207389668387805
			},
			"endBinding": {
				"elementId": "WjaAVyY30km1xdoBeyfVu",
				"focus": -0.03298056987328019,
				"gap": 1.190075069768909
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
					0,
					186.15842594339142
				]
			]
		},
		{
			"type": "rectangle",
			"version": 446,
			"versionNonce": 1412222960,
			"isDeleted": false,
			"id": "32VTj5SUuFt7lBJNngN9k",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -354.8918042260939,
			"y": 1490.4782973918327,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 444598544,
			"groupIds": [],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "mgin3XoV"
				},
				{
					"id": "403x-ZFs5ihqg9cxgZJgN",
					"type": "arrow"
				},
				{
					"id": "fFMGyqyWFG2MX-n42NAqh",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 445,
			"versionNonce": 1624367600,
			"isDeleted": false,
			"id": "mgin3XoV",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -321.436242746335,
			"y": 1510.0983324297433,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 79.140625,
			"height": 18.4,
			"seed": 1841063696,
			"groupIds": [],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690855,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Start Client",
			"rawText": "Start Client",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "32VTj5SUuFt7lBJNngN9k",
			"originalText": "Start Client",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "rectangle",
			"version": 623,
			"versionNonce": 1951241200,
			"isDeleted": false,
			"id": "mSdCjJUWX0odsgh3ghAys",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -352.6972343556308,
			"y": 1567.0874929661472,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 364709136,
			"groupIds": [],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "PH44gAuN"
				},
				{
					"id": "UmZwebYhgRW0GtLEIDNxc",
					"type": "arrow"
				}
			],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 620,
			"versionNonce": 1109402608,
			"isDeleted": false,
			"id": "PH44gAuN",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -318.8041728758719,
			"y": 1586.7075280040578,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 78.265625,
			"height": 18.4,
			"seed": 1878647568,
			"groupIds": [],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690855,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Stop Client",
			"rawText": "Stop Client",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "mSdCjJUWX0odsgh3ghAys",
			"originalText": "Stop Client",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "text",
			"version": 278,
			"versionNonce": 1309497328,
			"isDeleted": false,
			"id": "tRkZMS2w",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -332.2831818786999,
			"y": 1443.0338830008905,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 104.9296875,
			"height": 18.4,
			"seed": 1793786128,
			"groupIds": [],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Client Controls",
			"rawText": "Client Controls",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Client Controls",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "rectangle",
			"version": 157,
			"versionNonce": 612162032,
			"isDeleted": false,
			"id": "hyOtdtKQ5st4tKJZPik4W",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1895.8445665413437,
			"y": 917.5687317737157,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1965.1966241880336,
			"height": 986.4291007813285,
			"seed": 1711824656,
			"groupIds": [
				"iopnIIQBrTnwQhwUS3BkF"
			],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1714260690848,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 174,
			"versionNonce": 1168907248,
			"isDeleted": false,
			"id": "2u1c1ZxW",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1879.7992699363676,
			"y": 790.7660391719247,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 274.71099853515625,
			"height": 123.57667288199637,
			"seed": 298450192,
			"groupIds": [
				"iopnIIQBrTnwQhwUS3BkF"
			],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 107.45797641912729,
			"fontFamily": 2,
			"text": "Client",
			"rawText": "Client",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Client",
			"lineHeight": 1.15,
			"baseline": 99
		},
		{
			"type": "text",
			"version": 624,
			"versionNonce": 1134763504,
			"isDeleted": false,
			"id": "ns5D4lp1",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1853.6602113281024,
			"y": 951.6949714033191,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1450.6171875,
			"height": 82.8,
			"seed": 1336400656,
			"groupIds": [
				"iopnIIQBrTnwQhwUS3BkF"
			],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "The server is comprised of a set of shared functions which are primarily accessed via a CLI\nand a few tasks.",
			"rawText": "The server is comprised of a set of shared functions which are primarily accessed via a CLI\nand a few tasks.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "The server is comprised of a set of shared functions which are primarily accessed via a CLI\nand a few tasks.",
			"lineHeight": 1.15,
			"baseline": 74
		},
		{
			"type": "rectangle",
			"version": 454,
			"versionNonce": 795467760,
			"isDeleted": false,
			"id": "bMpJ4Cia7635UbB9WD38T",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -579.084885733645,
			"y": 1488.5371782213665,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 303692048,
			"groupIds": [],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "6DC7zhVe"
				},
				{
					"id": "0in98QOyK3gLNL2PsPLmH",
					"type": "arrow"
				}
			],
			"updated": 1714260690849,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 477,
			"versionNonce": 609625584,
			"isDeleted": false,
			"id": "6DC7zhVe",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -542.9769805038861,
			"y": 1508.1572132592771,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 73.8359375,
			"height": 18.4,
			"seed": 1016616720,
			"groupIds": [],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690856,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Send Ping",
			"rawText": "Send Ping",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "bMpJ4Cia7635UbB9WD38T",
			"originalText": "Send Ping",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "text",
			"version": 283,
			"versionNonce": 1334223856,
			"isDeleted": false,
			"id": "qUNDdOzJ",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -561.4319077937143,
			"y": 1441.0927638304238,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 115.5859375,
			"height": 18.4,
			"seed": 60486928,
			"groupIds": [],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Client Discovery",
			"rawText": "Client Discovery",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Client Discovery",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "line",
			"version": 437,
			"versionNonce": 1089250800,
			"isDeleted": false,
			"id": "GiBw-klVgH1Jl4XwlhouU",
			"fillStyle": "cross-hatch",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 20,
			"angle": 0,
			"x": -394.50462185166134,
			"y": 1444.904888292709,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 199.61098243279935,
			"seed": 1285149456,
			"groupIds": [],
			"frameId": "LM4Q5e5CEbYAYMMoHLins",
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					199.61098243279935
				]
			]
		},
		{
			"type": "frame",
			"version": 446,
			"versionNonce": 1514301424,
			"isDeleted": false,
			"id": "LM4Q5e5CEbYAYMMoHLins",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -628.3959091585175,
			"y": 1406.3608034147774,
			"strokeColor": "#bbb",
			"backgroundColor": "transparent",
			"width": 498.40485062545156,
			"height": 263.43361225792967,
			"seed": 235729168,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "403x-ZFs5ihqg9cxgZJgN",
					"type": "arrow"
				}
			],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"customData": {
				"frameColor": {
					"stroke": "#2B2B2B",
					"fill": "#525252",
					"nameColor": "#858585"
				}
			},
			"name": "Client Functions"
		},
		{
			"type": "text",
			"version": 643,
			"versionNonce": 126872048,
			"isDeleted": false,
			"id": "j1lX6GSY",
			"fillStyle": "cross-hatch",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -234.19092255953092,
			"y": 1270.6549506688953,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 251.703125,
			"height": 55.199999999999996,
			"seed": 795627280,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "fFMGyqyWFG2MX-n42NAqh",
					"type": "arrow"
				},
				{
					"id": "UmZwebYhgRW0GtLEIDNxc",
					"type": "arrow"
				}
			],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "These control the starting/stopping\nof local processes & any connected\nperipheral.",
			"rawText": "These control the starting/stopping\nof local processes & any connected\nperipheral.",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "These control the starting/stopping\nof local processes & any connected\nperipheral.",
			"lineHeight": 1.15,
			"baseline": 51
		},
		{
			"type": "arrow",
			"version": 1248,
			"versionNonce": 1943975696,
			"isDeleted": false,
			"id": "fFMGyqyWFG2MX-n42NAqh",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -92.67853136974463,
			"y": 1335.1052466454298,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 120.12197193966631,
			"height": 189.89490132687615,
			"seed": 1764748560,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260691250,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "j1lX6GSY",
				"focus": -0.10022488406201033,
				"gap": 9.250295976534744
			},
			"endBinding": {
				"elementId": "32VTj5SUuFt7lBJNngN9k",
				"gap": 8.946445845175731,
				"focus": 0.4918664350619713
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
					12.906892888010589,
					167.79251811199882
				],
				[
					-107.21507905165572,
					189.89490132687615
				]
			]
		},
		{
			"type": "arrow",
			"version": 1290,
			"versionNonce": 1125471504,
			"isDeleted": false,
			"id": "UmZwebYhgRW0GtLEIDNxc",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -92.81892264416274,
			"y": 1329.2172040578998,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 127.86909529120777,
			"height": 267.53978200468487,
			"seed": 617597712,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260691250,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "j1lX6GSY",
				"focus": -0.09506328971525788,
				"gap": 3.3622533890047634
			},
			"endBinding": {
				"elementId": "mSdCjJUWX0odsgh3ghAys",
				"gap": 10.58604872609908,
				"focus": 0.4860154665750138
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
					24.628580265356504,
					232.57649973805837
				],
				[
					-103.24051502585127,
					267.53978200468487
				]
			]
		},
		{
			"type": "text",
			"version": 336,
			"versionNonce": 815198192,
			"isDeleted": false,
			"id": "PFXIAxXQ",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1231.9954087588485,
			"y": 1531.3503259264353,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 142.28125,
			"height": 18.4,
			"seed": 1556343056,
			"groupIds": [],
			"frameId": "_wKelmtidVFU51vyPsneh",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Course Event Tasks",
			"rawText": "Course Event Tasks",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Course Event Tasks",
			"lineHeight": 1.15,
			"baseline": 14
		},
		{
			"type": "rectangle",
			"version": 765,
			"versionNonce": 840135152,
			"isDeleted": false,
			"id": "W5hL3ekGUVhXIAs9J0Poa",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1233.751324403609,
			"y": 1559.1664219056847,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 146.05174795951774,
			"height": 57.64007007582109,
			"seed": 2089043728,
			"groupIds": [],
			"frameId": "_wKelmtidVFU51vyPsneh",
			"roundness": {
				"type": 3
			},
			"boundElements": [
				{
					"type": "text",
					"id": "rjQr3gYT"
				},
				{
					"id": "oeVfQGUUyaxd65QfLXhCy",
					"type": "arrow"
				},
				{
					"id": "403x-ZFs5ihqg9cxgZJgN",
					"type": "arrow"
				}
			],
			"updated": 1714260690849,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 828,
			"versionNonce": 343664624,
			"isDeleted": false,
			"id": "rjQr3gYT",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1219.4207629238501,
			"y": 1569.5864569435953,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 117.390625,
			"height": 36.8,
			"seed": 1082713360,
			"groupIds": [],
			"frameId": "_wKelmtidVFU51vyPsneh",
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690856,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "Listen to Course\nstart/stop events",
			"rawText": "Listen to Course\nstart/stop events",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "W5hL3ekGUVhXIAs9J0Poa",
			"originalText": "Listen to Course\nstart/stop events",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "frame",
			"version": 585,
			"versionNonce": 510899696,
			"isDeleted": false,
			"id": "_wKelmtidVFU51vyPsneh",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1272.897824340619,
			"y": 1515.4859399135266,
			"strokeColor": "#bbb",
			"backgroundColor": "transparent",
			"width": 232.07289030113623,
			"height": 133.67476676731724,
			"seed": 373932816,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "oeVfQGUUyaxd65QfLXhCy",
					"type": "arrow"
				}
			],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"customData": {
				"frameColor": {
					"stroke": "#2B2B2B",
					"fill": "#525252",
					"nameColor": "#858585"
				}
			},
			"name": "Client Tasks"
		},
		{
			"type": "arrow",
			"version": 2168,
			"versionNonce": 342325232,
			"isDeleted": false,
			"id": "oeVfQGUUyaxd65QfLXhCy",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1406.7887679817213,
			"y": 1460.410338592926,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 164.046684321292,
			"height": 131.6201504896339,
			"seed": 2084495632,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "9BlSwu36",
				"focus": 0.1572483755366698,
				"gap": 7.274916803013866
			},
			"endBinding": {
				"elementId": "_wKelmtidVFU51vyPsneh",
				"focus": -0.18805198943233908,
				"gap": 1
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
					19.666879171514097,
					125.17028771676519
				],
				[
					164.046684321292,
					131.6201504896339
				]
			]
		},
		{
			"type": "text",
			"version": 1192,
			"versionNonce": 1519581680,
			"isDeleted": false,
			"id": "9BlSwu36",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1542.6147302393783,
			"y": 1379.535421789912,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 308.0625,
			"height": 73.6,
			"seed": 1642086160,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "oeVfQGUUyaxd65QfLXhCy",
					"type": "arrow"
				}
			],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "This can listen to an appropriate\nNATS topic (e.g., \"course.client_id.start\").\nThe wildcard (*) in the topic should\nbe the client's UID (letters & numbers only).",
			"rawText": "This can listen to an appropriate\nNATS topic (e.g., \"course.client_id.start\").\nThe wildcard (*) in the topic should\nbe the client's UID (letters & numbers only).",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "This can listen to an appropriate\nNATS topic (e.g., \"course.client_id.start\").\nThe wildcard (*) in the topic should\nbe the client's UID (letters & numbers only).",
			"lineHeight": 1.15,
			"baseline": 70
		},
		{
			"type": "arrow",
			"version": 1179,
			"versionNonce": 980373776,
			"isDeleted": false,
			"id": "403x-ZFs5ihqg9cxgZJgN",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1079.9964197414754,
			"y": 1583.3698455691529,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 450.83418957067056,
			"height": 28.05709275996807,
			"seed": 128310544,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "naCu77BJ"
				}
			],
			"updated": 1714260691251,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "W5hL3ekGUVhXIAs9J0Poa",
				"gap": 7.703156702615843,
				"focus": -0.03113747198788942
			},
			"endBinding": {
				"elementId": "LM4Q5e5CEbYAYMMoHLins",
				"focus": 0.020382202548531358,
				"gap": 1
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
					235.80183785063969,
					-10.565910061272234
				],
				[
					450.83418957067056,
					-28.05709275996807
				]
			]
		},
		{
			"type": "text",
			"version": 148,
			"versionNonce": 1050241520,
			"isDeleted": false,
			"id": "naCu77BJ",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -964.8146990783357,
			"y": 1549.8039355078806,
			"strokeColor": "#2f9e44",
			"backgroundColor": "transparent",
			"width": 241.240234375,
			"height": 46,
			"seed": 1594342160,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690856,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "Calls the appropriate Client\nControl function",
			"rawText": "Calls the appropriate Client\nControl function",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "403x-ZFs5ihqg9cxgZJgN",
			"originalText": "Calls the appropriate Client\nControl function",
			"lineHeight": 1.15,
			"baseline": 41
		},
		{
			"type": "rectangle",
			"version": 119,
			"versionNonce": 1739849712,
			"isDeleted": false,
			"id": "AJB9xJ2S8s761AmEdwowP",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1699.2945590035397,
			"y": 924.6459249515761,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1965.1966241880336,
			"height": 986.4291007813285,
			"seed": 1786632464,
			"groupIds": [
				"cKx_1fCKw4rFACOR5sPKl"
			],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 143,
			"versionNonce": 588153328,
			"isDeleted": false,
			"id": "biKj4CuZ",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1683.2492623985636,
			"y": 797.843232349786,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 632.9999389648438,
			"height": 123.57667288199637,
			"seed": 494941968,
			"groupIds": [
				"cKx_1fCKw4rFACOR5sPKl"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 107.45797641912729,
			"fontFamily": 2,
			"text": "Clients/Holes",
			"rawText": "Clients/Holes",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Clients/Holes",
			"lineHeight": 1.15,
			"baseline": 99
		},
		{
			"type": "text",
			"version": 674,
			"versionNonce": 1405666288,
			"isDeleted": false,
			"id": "KnnWgrFM",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -1657.6875898957596,
			"y": 957.1947784757184,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1108.599609375,
			"height": 207,
			"seed": 1015469328,
			"groupIds": [
				"cKx_1fCKw4rFACOR5sPKl"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 2,
			"text": "The client is comprised of a set of functions and a listener task:\n    - generate a UID on boot (or perhaps hardcode/configured?)\n    - listen on <course / client_id / *> and take appropriate action\n      for each message type\n    - publishes a <hole / client_id / ping> to make the server aware of it",
			"rawText": "The client is comprised of a set of functions and a listener task:\n    - generate a UID on boot (or perhaps hardcode/configured?)\n    - listen on <course / client_id / *> and take appropriate action\n      for each message type\n    - publishes a <hole / client_id / ping> to make the server aware of it",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "The client is comprised of a set of functions and a listener task:\n    - generate a UID on boot (or perhaps hardcode/configured?)\n    - listen on <course / client_id / *> and take appropriate action\n      for each message type\n    - publishes a <hole / client_id / ping> to make the server aware of it",
			"lineHeight": 1.15,
			"baseline": 198
		},
		{
			"type": "text",
			"version": 524,
			"versionNonce": 938132976,
			"isDeleted": false,
			"id": "iF6MfDt5",
			"fillStyle": "cross-hatch",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -861.6827656231071,
			"y": 1302.2395345374775,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 275.203125,
			"height": 36.8,
			"seed": 1024045840,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "0in98QOyK3gLNL2PsPLmH",
					"type": "arrow"
				}
			],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 16,
			"fontFamily": 2,
			"text": "These can publish to appropriate\nNATS topics (e.g., \"hole.hole_id.ping\").",
			"rawText": "These can publish to appropriate\nNATS topics (e.g., \"hole.hole_id.ping\").",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "These can publish to appropriate\nNATS topics (e.g., \"hole.hole_id.ping\").",
			"lineHeight": 1.15,
			"baseline": 33
		},
		{
			"type": "arrow",
			"version": 420,
			"versionNonce": 1841836816,
			"isDeleted": false,
			"id": "0in98QOyK3gLNL2PsPLmH",
			"fillStyle": "cross-hatch",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": -730.0489384386447,
			"y": 1347.3456346358098,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 142.68906514561786,
			"height": 170.32626865517614,
			"seed": 629199120,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260691251,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "iF6MfDt5",
				"focus": 0.05133886924492313,
				"gap": 8.306100098332081
			},
			"endBinding": {
				"elementId": "bMpJ4Cia7635UbB9WD38T",
				"gap": 8.27498755938177,
				"focus": -0.25760648319686763
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
					6.591070425600719,
					154.8420228470202
				],
				[
					142.68906514561786,
					170.32626865517614
				]
			]
		},
		{
			"type": "rectangle",
			"version": 896,
			"versionNonce": 763759088,
			"isDeleted": false,
			"id": "s-CUS2FjNquyPYpUwks9z",
			"fillStyle": "cross-hatch",
			"strokeWidth": 4,
			"strokeStyle": "solid",
			"roughness": 0,
			"opacity": 100,
			"angle": 0,
			"x": 283.98338025455905,
			"y": -408.6825336935748,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1965.1966241880336,
			"height": 986.4291007813285,
			"seed": 1835282192,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 767,
			"versionNonce": 906972144,
			"isDeleted": false,
			"id": "AHzVCKq4",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 326.11115579595025,
			"y": -377.8287993627822,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 94.4921875,
			"height": 23,
			"seed": 1563151632,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "Participant",
			"rawText": "Participant",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Participant",
			"lineHeight": 1.15,
			"baseline": 18
		},
		{
			"type": "text",
			"version": 1235,
			"versionNonce": 538988016,
			"isDeleted": false,
			"id": "LDZ2ejMs",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 546.2919370367335,
			"y": -196.72596147621823,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 709.287109375,
			"height": 207,
			"seed": 1850714896,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "map to azure token / unique microsoft ID (?) -- can get profile picture / name\n\nmap to course_<id> : time participant started course_<id>\n\nmap to course_<id> : time participant ended course_<id>\n\nmap to course_<id> : elapsed time of participant at course_<id>\n\nmap to course_<id> : [1/0] if participant has a start and end time tracked for hole",
			"rawText": "map to azure token / unique microsoft ID (?) -- can get profile picture / name\n\nmap to course_<id> : time participant started course_<id>\n\nmap to course_<id> : time participant ended course_<id>\n\nmap to course_<id> : elapsed time of participant at course_<id>\n\nmap to course_<id> : [1/0] if participant has a start and end time tracked for hole",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "map to azure token / unique microsoft ID (?) -- can get profile picture / name\n\nmap to course_<id> : time participant started course_<id>\n\nmap to course_<id> : time participant ended course_<id>\n\nmap to course_<id> : elapsed time of participant at course_<id>\n\nmap to course_<id> : [1/0] if participant has a start and end time tracked for hole",
			"lineHeight": 1.15,
			"baseline": 202
		},
		{
			"type": "rectangle",
			"version": 600,
			"versionNonce": 1690374128,
			"isDeleted": false,
			"id": "QgfEd8NEjlZXPjNmOIq5k",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 334.17088473123385,
			"y": -231.12278711574538,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 958.7596710355108,
			"height": 277.2140924956478,
			"seed": 726124816,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 904,
			"versionNonce": 469340656,
			"isDeleted": false,
			"id": "tmbRlnul",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 373.3572493899637,
			"y": -196.7259616470675,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 118.96484375,
			"height": 207,
			"seed": 260843280,
			"groupIds": [
				"r1S9MLkzS4bWP8oex4Dyf"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 2,
			"text": "participant_id\n\nstart_time\n\nend_time\n\nelapsed_time\n\ncompleted",
			"rawText": "participant_id\n\nstart_time\n\nend_time\n\nelapsed_time\n\ncompleted",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "participant_id\n\nstart_time\n\nend_time\n\nelapsed_time\n\ncompleted",
			"lineHeight": 1.15,
			"baseline": 202
		},
		{
			"type": "line",
			"version": 418,
			"versionNonce": 483513328,
			"isDeleted": false,
			"id": "wWilGTwnQOQbjOpHFq_Y7",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 520.4464031854418,
			"y": -201.77778943654596,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 232.2012414229157,
			"seed": 1737803024,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					0,
					232.2012414229157
				]
			]
		},
		{
			"type": "freedraw",
			"version": 27,
			"versionNonce": 491902448,
			"isDeleted": false,
			"id": "NBW7moIqeYOYqBVFAyKc0",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2828.600687327541,
			"y": -458.00377363043674,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 902.2222900390625,
			"height": 305.5555216471353,
			"seed": 819569424,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					5.55562337239553,
					-2.2221883138020075
				],
				[
					12.2222900390625,
					-5.555521647135265
				],
				[
					25.55562337239553,
					-11.11114501953125
				],
				[
					50,
					-22.222188313802008
				],
				[
					83.33333333333303,
					-34.44447835286451
				],
				[
					128.88895670572902,
					-48.88885498046875
				],
				[
					187.77791341145848,
					-66.66666666666652
				],
				[
					254.444580078125,
					-87.77781168619782
				],
				[
					326.6666666666665,
					-114.44447835286445
				],
				[
					406.6666666666665,
					-138.8888549804687
				],
				[
					486.6666666666665,
					-164.44447835286445
				],
				[
					564.444580078125,
					-186.66666666666657
				],
				[
					627.7779134114585,
					-208.8888549804687
				],
				[
					697.7779134114585,
					-228.8888549804687
				],
				[
					755.555623372396,
					-246.66666666666657
				],
				[
					805.555623372396,
					-262.22218831380195
				],
				[
					843.3333333333335,
					-275.5555216471353
				],
				[
					868.888956705729,
					-286.6666666666666
				],
				[
					886.6666666666665,
					-295.5555216471353
				],
				[
					896.6666666666665,
					-302.22218831380195
				],
				[
					902.2222900390625,
					-305.5555216471353
				],
				[
					902.2222900390625,
					-305.5555216471353
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 32,
			"versionNonce": 1384224752,
			"isDeleted": false,
			"id": "Tku6SojJTjMa3t2knfaSp",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3730.8229773666035,
			"y": -753.559295277572,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 478.888956705729,
			"height": 242.22218831380206,
			"seed": 2043855120,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.2222900390625,
					2.2221883138021212
				],
				[
					7.7777099609375,
					7.7777099609375
				],
				[
					17.7777099609375,
					18.88885498046875
				],
				[
					32.2222900390625,
					33.33333333333337
				],
				[
					54.444376627604015,
					50
				],
				[
					87.7777099609375,
					70
				],
				[
					133.33333333333348,
					91.11104329427087
				],
				[
					184.44437662760402,
					115.55552164713538
				],
				[
					240,
					135.55552164713538
				],
				[
					292.2222900390625,
					156.66666666666663
				],
				[
					332.2222900390625,
					171.11104329427087
				],
				[
					372.2222900390625,
					184.44437662760413
				],
				[
					400,
					193.33333333333337
				],
				[
					423.3333333333335,
					202.22218831380212
				],
				[
					434.444376627604,
					207.7777099609375
				],
				[
					443.3333333333335,
					210
				],
				[
					447.7777099609375,
					214.44437662760407
				],
				[
					452.2222900390625,
					217.77770996093756
				],
				[
					455.555623372396,
					222.22218831380206
				],
				[
					458.888956705729,
					227.77770996093756
				],
				[
					464.444376627604,
					232.22218831380206
				],
				[
					467.7777099609375,
					236.66666666666657
				],
				[
					472.2222900390625,
					238.8888549804688
				],
				[
					475.555623372396,
					241.11104329427081
				],
				[
					477.7777099609375,
					241.11104329427081
				],
				[
					478.888956705729,
					242.22218831380206
				],
				[
					478.888956705729,
					242.22218831380206
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 36,
			"versionNonce": 275323376,
			"isDeleted": false,
			"id": "QUhjN0N_vngaTvAaAq3lz",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4211.934020660874,
			"y": -515.7815853166345,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 1310.0000000000005,
			"height": 558.888956705729,
			"seed": 1106779920,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.22208658854197,
					0
				],
				[
					-6.66666666666697,
					4.4444783528645075
				],
				[
					-13.333333333333485,
					7.777811686197765
				],
				[
					-24.44437662760447,
					15.555623372395758
				],
				[
					-45.555419921875,
					26.666666666666515
				],
				[
					-73.33333333333348,
					42.2222900390625
				],
				[
					-115.555419921875,
					62.2222900390625
				],
				[
					-171.11104329427098,
					90
				],
				[
					-247.7777099609375,
					123.33333333333326
				],
				[
					-337.7777099609375,
					160
				],
				[
					-440,
					198.88895670572902
				],
				[
					-546.666666666667,
					237.77781168619777
				],
				[
					-653.3333333333335,
					276.6666666666665
				],
				[
					-753.3333333333335,
					313.33333333333326
				],
				[
					-850,
					352.2222900390625
				],
				[
					-941.111043294271,
					387.77781168619777
				],
				[
					-1022.222086588542,
					420
				],
				[
					-1087.7777099609375,
					445.55562337239576
				],
				[
					-1140,
					465.55562337239576
				],
				[
					-1173.3333333333335,
					482.2222900390625
				],
				[
					-1205.555419921875,
					497.77781168619777
				],
				[
					-1231.111043294271,
					510
				],
				[
					-1250.0000000000005,
					521.1112467447915
				],
				[
					-1265.5554199218755,
					530
				],
				[
					-1283.3333333333335,
					540
				],
				[
					-1294.4443766276045,
					547.7779134114583
				],
				[
					-1302.222086588542,
					553.3333333333333
				],
				[
					-1306.666666666667,
					557.7779134114583
				],
				[
					-1308.8887532552085,
					558.888956705729
				],
				[
					-1310.0000000000005,
					558.888956705729
				],
				[
					-1310.0000000000005,
					558.888956705729
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 31,
			"versionNonce": 1779457008,
			"isDeleted": false,
			"id": "96qWS_Vaw2mIEsogjg4mr",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2910.8229773666035,
			"y": 54.218414683365495,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 320,
			"height": 384.44437662760424,
			"seed": 1505869072,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.111043294270985,
					-1.111043294270985
				],
				[
					-2.2222900390625,
					-4.4443766276042425
				],
				[
					-4.44437662760447,
					-6.6666666666667425
				],
				[
					-7.7777099609375,
					-12.222086588541742
				],
				[
					-12.2222900390625,
					-17.7777099609375
				],
				[
					-16.66666666666697,
					-26.666666666666742
				],
				[
					-23.333333333333485,
					-37.7777099609375
				],
				[
					-33.333333333333485,
					-52.22208658854174
				],
				[
					-51.111043294270985,
					-71.11104329427098
				],
				[
					-67.7777099609375,
					-91.11104329427098
				],
				[
					-91.11104329427098,
					-118.88885498046875
				],
				[
					-116.66666666666697,
					-145.5555216471355
				],
				[
					-146.66666666666697,
					-177.7777099609375
				],
				[
					-175.55562337239598,
					-207.7777099609375
				],
				[
					-203.33333333333348,
					-238.88885498046875
				],
				[
					-231.11104329427098,
					-267.7777099609375
				],
				[
					-254.44437662760447,
					-295.5555216471355
				],
				[
					-274.44437662760447,
					-318.88885498046875
				],
				[
					-291.11114501953125,
					-341.111043294271
				],
				[
					-304.44447835286473,
					-357.7777099609375
				],
				[
					-312.2222900390625,
					-370
				],
				[
					-316.66666666666697,
					-377.7777099609375
				],
				[
					-318.88895670572947,
					-381.111043294271
				],
				[
					-320,
					-383.3333333333335
				],
				[
					-320,
					-384.44437662760424
				],
				[
					-320,
					-384.44437662760424
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 32,
			"versionNonce": 1367301616,
			"isDeleted": false,
			"id": "LXcl0B76jJqpkku2T9-Zr",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2583.0451656804053,
			"y": -338.00377363043674,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 146.66676839192723,
			"height": 75.55552164713527,
			"seed": 1118280464,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-1.11114501953125
				],
				[
					0,
					-2.2221883138020075
				],
				[
					0,
					-3.3333333333332575
				],
				[
					-2.22218831380178,
					-5.555521647135265
				],
				[
					-4.44447835286428,
					-10
				],
				[
					-5.555521647135265,
					-11.11114501953125
				],
				[
					-6.666666666666515,
					-13.333333333333258
				],
				[
					-8.88885498046875,
					-16.666666666666515
				],
				[
					-10,
					-17.777811686197765
				],
				[
					-7.777811686197765,
					-17.777811686197765
				],
				[
					-6.666666666666515,
					-17.777811686197765
				],
				[
					-4.44447835286428,
					-17.777811686197765
				],
				[
					-2.22218831380178,
					-18.88885498046875
				],
				[
					7.77781168619822,
					-21.11114501953125
				],
				[
					13.333333333333485,
					-22.222188313802008
				],
				[
					18.88885498046875,
					-23.333333333333258
				],
				[
					27.77781168619822,
					-26.666666666666515
				],
				[
					36.66666666666697,
					-31.11114501953125
				],
				[
					47.77781168619822,
					-34.44447835286451
				],
				[
					63.33343505859375,
					-41.11114501953125
				],
				[
					77.77781168619822,
					-45.555521647135265
				],
				[
					91.11114501953125,
					-52.22218831380201
				],
				[
					105.55552164713572,
					-58.88885498046875
				],
				[
					118.88885498046875,
					-65.55552164713527
				],
				[
					132.22218831380223,
					-72.22218831380201
				],
				[
					136.66676839192723,
					-75.55552164713527
				],
				[
					136.66676839192723,
					-75.55552164713527
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 23,
			"versionNonce": 935206896,
			"isDeleted": false,
			"id": "j2QAOUNlf2dp-Nt5E58A3",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2835.2673539942075,
			"y": -463.559295277572,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 47.7777099609375,
			"height": 21.111043294270758,
			"seed": 253868304,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.333333333333485,
					1.1110432942707575
				],
				[
					-6.666666666666515,
					3.3333333333332575
				],
				[
					-12.222086588541515,
					5.555521647135265
				],
				[
					-16.666666666666515,
					7.7777099609375
				],
				[
					-22.222086588541515,
					10
				],
				[
					-25.555419921875,
					12.222188313802008
				],
				[
					-31.111043294270985,
					14.444376627604015
				],
				[
					-35.555419921875,
					15.555521647135265
				],
				[
					-38.888753255208485,
					16.666666666666515
				],
				[
					-41.111043294270985,
					17.7777099609375
				],
				[
					-42.222086588541515,
					17.7777099609375
				],
				[
					-43.333333333333485,
					18.88885498046875
				],
				[
					-44.444376627604015,
					18.88885498046875
				],
				[
					-44.444376627604015,
					20
				],
				[
					-45.555419921875,
					20
				],
				[
					-46.666666666666515,
					21.111043294270758
				],
				[
					-47.7777099609375,
					21.111043294270758
				],
				[
					-47.7777099609375,
					21.111043294270758
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 15,
			"versionNonce": 752132592,
			"isDeleted": false,
			"id": "zLU5SE_o_04EieWNbSylq",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2908.600687327541,
			"y": 36.440704722427995,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 4.444580078125,
			"height": 35.55562337239576,
			"seed": 1118312208,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.111246744791515,
					0
				],
				[
					1.111246744791515,
					3.3333333333332575
				],
				[
					0,
					10
				],
				[
					-2.22208658854197,
					17.7777099609375
				],
				[
					-2.22208658854197,
					23.333333333333258
				],
				[
					-2.22208658854197,
					27.7777099609375
				],
				[
					-3.333333333333485,
					32.2222900390625
				],
				[
					-3.333333333333485,
					34.444376627604015
				],
				[
					-3.333333333333485,
					35.55562337239576
				],
				[
					-3.333333333333485,
					35.55562337239576
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 20,
			"versionNonce": 2144003056,
			"isDeleted": false,
			"id": "Ffd8ZPEh-U4--5cg759Fg",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2583.0451656804053,
			"y": -351.33710696377,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 2.22218831380178,
			"height": 34.44447835286451,
			"seed": 833795344,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.11114501953125,
					1.11114501953125
				],
				[
					-2.22218831380178,
					2.2221883138020075
				],
				[
					-2.22218831380178,
					7.7778116861979925
				],
				[
					-2.22218831380178,
					10
				],
				[
					-2.22218831380178,
					15.555521647135492
				],
				[
					-2.22218831380178,
					18.88885498046875
				],
				[
					-2.22218831380178,
					22.222188313802008
				],
				[
					-2.22218831380178,
					26.666666666666742
				],
				[
					-2.22218831380178,
					27.777811686197992
				],
				[
					-1.11114501953125,
					28.88885498046875
				],
				[
					-1.11114501953125,
					31.11114501953125
				],
				[
					-1.11114501953125,
					32.22218831380201
				],
				[
					-1.11114501953125,
					33.33333333333326
				],
				[
					-1.11114501953125,
					34.44447835286451
				],
				[
					-1.11114501953125,
					34.44447835286451
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 79,
			"versionNonce": 1588127216,
			"isDeleted": false,
			"id": "IWPuAa91AvI9e-_E-fh29",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2901.934020660874,
			"y": 74.2184146833655,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 328.88885498046875,
			"height": 380,
			"seed": 1639551760,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.1110432942705302,
					-1.111043294270985
				],
				[
					-2.222086588541515,
					-2.2220865885417425
				],
				[
					-4.444376627604015,
					-5.555419921875
				],
				[
					-6.666666666666515,
					-8.888753255208485
				],
				[
					-10,
					-12.222086588541742
				],
				[
					-12.222086588541515,
					-15.555419921875
				],
				[
					-15.555419921875,
					-20
				],
				[
					-17.7777099609375,
					-23.333333333333485
				],
				[
					-24.444376627604015,
					-30
				],
				[
					-28.88875325520803,
					-35.555419921875
				],
				[
					-34.444376627604015,
					-41.111043294270985
				],
				[
					-41.11104329427053,
					-48.888753255208485
				],
				[
					-47.7777099609375,
					-56.66666666666674
				],
				[
					-54.444376627604015,
					-64.44437662760424
				],
				[
					-63.33333333333303,
					-74.44437662760424
				],
				[
					-71.11104329427053,
					-84.44437662760424
				],
				[
					-81.11104329427053,
					-93.33333333333348
				],
				[
					-91.11104329427053,
					-103.33333333333348
				],
				[
					-103.33333333333303,
					-114.44437662760424
				],
				[
					-113.33333333333303,
					-126.66666666666674
				],
				[
					-126.66666666666652,
					-137.7777099609375
				],
				[
					-136.66666666666652,
					-147.7777099609375
				],
				[
					-147.7777099609375,
					-160
				],
				[
					-156.66666666666652,
					-168.88885498046875
				],
				[
					-164.44437662760402,
					-178.88885498046875
				],
				[
					-173.33333333333303,
					-187.7777099609375
				],
				[
					-180,
					-195.5555216471355
				],
				[
					-186.66666666666652,
					-204.44437662760424
				],
				[
					-193.33333333333303,
					-212.22218831380223
				],
				[
					-200,
					-221.11104329427098
				],
				[
					-207.7777099609375,
					-228.88885498046875
				],
				[
					-214.44437662760402,
					-236.66666666666674
				],
				[
					-220,
					-245.5555216471355
				],
				[
					-228.88875325520803,
					-253.33333333333348
				],
				[
					-233.33333333333303,
					-261.111043294271
				],
				[
					-238.88875325520803,
					-267.7777099609375
				],
				[
					-243.33333333333303,
					-274.44437662760424
				],
				[
					-247.7777099609375,
					-280
				],
				[
					-251.11104329427053,
					-284.44437662760424
				],
				[
					-255.555419921875,
					-287.7777099609375
				],
				[
					-257.7777099609375,
					-293.3333333333335
				],
				[
					-260,
					-296.66666666666674
				],
				[
					-263.33333333333303,
					-300
				],
				[
					-265.555419921875,
					-303.3333333333335
				],
				[
					-268.88875325520803,
					-306.66666666666674
				],
				[
					-271.11104329427053,
					-311.111043294271
				],
				[
					-276.6666666666665,
					-315.5555216471355
				],
				[
					-281.11104329427053,
					-320
				],
				[
					-285.55552164713527,
					-325.5555216471355
				],
				[
					-288.88885498046875,
					-328.88885498046875
				],
				[
					-293.33333333333303,
					-333.3333333333335
				],
				[
					-295.55552164713527,
					-336.66666666666674
				],
				[
					-298.88885498046875,
					-338.88885498046875
				],
				[
					-301.11104329427053,
					-342.22218831380223
				],
				[
					-302.2221883138018,
					-344.44437662760424
				],
				[
					-303.33333333333303,
					-345.5555216471355
				],
				[
					-304.444376627604,
					-347.7777099609375
				],
				[
					-306.6666666666665,
					-350
				],
				[
					-307.7777099609375,
					-352.22218831380223
				],
				[
					-308.88885498046875,
					-354.44437662760424
				],
				[
					-311.11104329427053,
					-356.66666666666674
				],
				[
					-314.444376627604,
					-358.88885498046875
				],
				[
					-315.55552164713527,
					-362.22218831380223
				],
				[
					-320,
					-366.66666666666674
				],
				[
					-322.2221883138018,
					-368.88885498046875
				],
				[
					-323.33333333333303,
					-372.22218831380223
				],
				[
					-325.55552164713527,
					-373.3333333333335
				],
				[
					-326.6666666666665,
					-374.44437662760424
				],
				[
					-326.6666666666665,
					-375.5555216471355
				],
				[
					-327.7777099609375,
					-376.66666666666674
				],
				[
					-327.7777099609375,
					-377.7777099609375
				],
				[
					-328.88885498046875,
					-378.88885498046875
				],
				[
					-328.88885498046875,
					-380
				],
				[
					-328.88885498046875,
					-380
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 18,
			"versionNonce": 1987487728,
			"isDeleted": false,
			"id": "E3VBB_zxK2mU8rHmRWf9o",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 4203.045267405666,
			"y": -508.00377363043674,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 3.333333333333485,
			"height": 22.222188313802235,
			"seed": 1765060880,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.11114501953125
				],
				[
					0,
					3.333333333333485
				],
				[
					-1.111246744791515,
					4.444478352864735
				],
				[
					-2.2222900390625,
					7.7778116861979925
				],
				[
					-3.333333333333485,
					10
				],
				[
					-3.333333333333485,
					13.333333333333485
				],
				[
					-3.333333333333485,
					15.555521647135492
				],
				[
					-3.333333333333485,
					16.666666666666742
				],
				[
					-3.333333333333485,
					18.88885498046875
				],
				[
					-3.333333333333485,
					20
				],
				[
					-3.333333333333485,
					21.11114501953125
				],
				[
					-3.333333333333485,
					22.222188313802235
				],
				[
					-3.333333333333485,
					22.222188313802235
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 38,
			"versionNonce": 322710000,
			"isDeleted": false,
			"id": "1deZQmmlP2uU53bdB8-gW",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2904.1563106999365,
			"y": 61.99632809482375,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 708.8889567057295,
			"height": 303.33343505859375,
			"seed": 1335627536,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.2222900390625,
					0
				],
				[
					4.44437662760447,
					-2.2222900390625
				],
				[
					5.555623372395985,
					-2.2222900390625
				],
				[
					7.7777099609375,
					-3.3333333333332575
				],
				[
					10,
					-5.5556233723957575
				],
				[
					14.44437662760447,
					-7.7779134114582575
				],
				[
					18.88895670572947,
					-8.888956705729242
				],
				[
					23.333333333333485,
					-12.2222900390625
				],
				[
					30,
					-15.555623372395758
				],
				[
					37.7777099609375,
					-18.888956705729242
				],
				[
					46.66666666666697,
					-23.333333333333258
				],
				[
					56.66666666666697,
					-27.777913411458258
				],
				[
					68.88895670572947,
					-34.444580078125
				],
				[
					83.33333333333348,
					-42.2222900390625
				],
				[
					100.00000000000045,
					-50
				],
				[
					120.00000000000045,
					-61.11124674479174
				],
				[
					141.11104329427098,
					-70.00010172526049
				],
				[
					166.66666666666697,
					-81.11124674479174
				],
				[
					194.44437662760447,
					-94.444580078125
				],
				[
					226.66666666666697,
					-107.77791341145826
				],
				[
					258.88895670572947,
					-122.2222900390625
				],
				[
					294.44437662760447,
					-135.55562337239576
				],
				[
					333.3333333333335,
					-150.0001017252605
				],
				[
					370.00000000000045,
					-164.444580078125
				],
				[
					415.555623372396,
					-183.33343505859375
				],
				[
					466.66666666666697,
					-202.2222900390625
				],
				[
					518.8889567057295,
					-223.33343505859375
				],
				[
					580.0000000000005,
					-247.77791341145826
				],
				[
					622.222290039063,
					-265.55562337239576
				],
				[
					667.777709960938,
					-285.55562337239576
				],
				[
					703.3333333333335,
					-300.0001017252605
				],
				[
					708.8889567057295,
					-303.33343505859375
				],
				[
					708.8889567057295,
					-303.33343505859375
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 44,
			"versionNonce": 1073834992,
			"isDeleted": false,
			"id": "4XfhmoURy1F7PMKWQoxuu",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3614.156310699937,
			"y": -244.67044029710326,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 575.5556233723955,
			"height": 236.66666666666674,
			"seed": 1835511056,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					3.33333333333303,
					-2.222188313802235
				],
				[
					5.55562337239553,
					-2.222188313802235
				],
				[
					10,
					-5.5555216471354925
				],
				[
					16.666666666666515,
					-7.7778116861979925
				],
				[
					23.33333333333303,
					-10
				],
				[
					28.888956705729015,
					-12.222188313802235
				],
				[
					36.666666666666515,
					-14.444478352864735
				],
				[
					45.55562337239553,
					-20
				],
				[
					56.666666666666515,
					-24.444478352864735
				],
				[
					70,
					-30
				],
				[
					83.33333333333303,
					-35.55552164713549
				],
				[
					96.66666666666652,
					-42.222188313802235
				],
				[
					113.33333333333303,
					-48.88885498046875
				],
				[
					132.2222900390625,
					-55.55552164713549
				],
				[
					152.2222900390625,
					-63.333333333333485
				],
				[
					176.66666666666652,
					-73.33333333333348
				],
				[
					201.11104329427053,
					-81.11114501953125
				],
				[
					226.66666666666652,
					-88.88885498046875
				],
				[
					253.33333333333303,
					-96.66666666666674
				],
				[
					278.888956705729,
					-105.55552164713549
				],
				[
					306.6666666666665,
					-114.44447835286473
				],
				[
					333.33333333333303,
					-121.11114501953125
				],
				[
					357.7777099609375,
					-128.88885498046875
				],
				[
					376.6666666666665,
					-134.44447835286473
				],
				[
					397.7777099609375,
					-143.33333333333348
				],
				[
					416.6666666666665,
					-152.22218831380223
				],
				[
					436.6666666666665,
					-162.22218831380223
				],
				[
					455.55562337239553,
					-172.22218831380223
				],
				[
					473.33333333333303,
					-183.33333333333348
				],
				[
					492.2222900390625,
					-193.33333333333348
				],
				[
					510,
					-204.44447835286473
				],
				[
					531.1110432942705,
					-215.5555216471355
				],
				[
					544.444376627604,
					-223.33333333333348
				],
				[
					555.5556233723955,
					-228.88885498046875
				],
				[
					565.5556233723955,
					-233.33333333333348
				],
				[
					572.2222900390625,
					-235.5555216471355
				],
				[
					574.444376627604,
					-236.66666666666674
				],
				[
					575.5556233723955,
					-236.66666666666674
				],
				[
					575.5556233723955,
					-236.66666666666674
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 16,
			"versionNonce": 1724804592,
			"isDeleted": false,
			"id": "j2BOowb37n4IxX_Xjoz-g",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3807.7742493291053,
			"y": -619.4335966855791,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 17.72203128230558,
			"height": 135.86892288657305,
			"seed": 1276087056,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.6851890326806824,
					-10.740657797365714
				],
				[
					4.296282785618132,
					-22.55531254111679
				],
				[
					6.981373484940377,
					-37.59220395742119
				],
				[
					8.592467237876917,
					-53.703141486790344
				],
				[
					10.740657797365202,
					-70.35112665603162
				],
				[
					12.351751550302652,
					-88.61015641153034
				],
				[
					15.036842249624897,
					-104.18409546770687
				],
				[
					16.647936002561437,
					-118.68393924413908
				],
				[
					17.72203128230558,
					-131.57268926763442
				],
				[
					17.72203128230558,
					-135.86892288657305
				],
				[
					17.72203128230558,
					-135.86892288657305
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 19,
			"versionNonce": 1890267120,
			"isDeleted": false,
			"id": "y24-r9es4YtlueUxmo6p1",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3829.2554665904777,
			"y": -754.7654719322801,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 37.05515631754906,
			"height": 26.85154616005542,
			"seed": 101427472,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.6110937529369949,
					1.0740461130647532
				],
				[
					2.685189032681137,
					2.685139866001691
				],
				[
					5.370378065362274,
					4.833281258810757
				],
				[
					7.518470291491667,
					7.518421124812448
				],
				[
					10.740657797365657,
					10.740608630686268
				],
				[
					15.036940582983789,
					13.962796136560087
				],
				[
					20.944218788180024,
					17.184983642433963
				],
				[
					26.314596853542298,
					20.407171148307782
				],
				[
					30.610781305801083,
					23.092311014309473
				],
				[
					33.83296881167507,
					24.70340476724641
				],
				[
					35.98115937116336,
					25.777500046990667
				],
				[
					36.518157844356665,
					26.85154616005542
				],
				[
					37.05515631754906,
					26.85154616005542
				],
				[
					37.05515631754906,
					26.85154616005542
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 22,
			"versionNonce": 1704964592,
			"isDeleted": false,
			"id": "QPMp4k62lBwOiTDaQRDFU",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3864.6995291550897,
			"y": -727.9139257722246,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 45.11062508223358,
			"height": 0.537047639872128,
			"seed": 651429648,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5369984731928525,
					0
				],
				[
					-1.6110937529369949,
					0
				],
				[
					-2.685090699322245,
					0
				],
				[
					-5.370279732003382,
					0.537047639872128
				],
				[
					-8.05546876468452,
					0.537047639872128
				],
				[
					-11.814654743751362,
					0.537047639872128
				],
				[
					-16.110937529369494,
					0.537047639872128
				],
				[
					-21.48121726137242,
					0.537047639872128
				],
				[
					-26.85149699337626,
					0.537047639872128
				],
				[
					-32.22187505873853,
					0.537047639872128
				],
				[
					-37.05515631754906,
					0.537047639872128
				],
				[
					-40.81434229661545,
					0.537047639872128
				],
				[
					-43.49953132929704,
					0
				],
				[
					-44.57352827568184,
					0
				],
				[
					-45.11062508223358,
					0
				],
				[
					-44.57352827568184,
					0
				],
				[
					-44.57352827568184,
					0
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 14,
			"versionNonce": 213119984,
			"isDeleted": false,
			"id": "o2v1uJcfoK0hEyIZig6lO",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3824.4221853316667,
			"y": -761.7468945838999,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 0,
			"height": 10.740608630686324,
			"seed": 182494480,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.611093752936938
				],
				[
					0,
					3.222187505873876
				],
				[
					0,
					5.370328898682885
				],
				[
					0,
					6.444375011747695
				],
				[
					0,
					7.518421124812448
				],
				[
					0,
					9.129514877749386
				],
				[
					0,
					10.203610157493642
				],
				[
					0,
					10.740608630686324
				],
				[
					0,
					10.740608630686324
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 81,
			"versionNonce": 200275440,
			"isDeleted": false,
			"id": "KbBJ5Rqhd0SNtbF0ORUq7",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3809.385343082042,
			"y": -618.8965982123865,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 26.85149699337626,
			"height": 16.110937529369153,
			"seed": 1068073744,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5369984731928525,
					0
				],
				[
					1.0740952797441423,
					0
				],
				[
					1.6110937529369949,
					0
				],
				[
					2.685189032681592,
					0
				],
				[
					3.7591859790663875,
					0
				],
				[
					4.833281258810985,
					0
				],
				[
					5.370279732003837,
					0
				],
				[
					5.907376538555127,
					0
				],
				[
					6.981373484940377,
					0
				],
				[
					8.05546876468452,
					0
				],
				[
					8.05546876468452,
					0.537047639872128
				],
				[
					9.66656251762197,
					0.537047639872128
				],
				[
					10.203560990814367,
					0.537047639872128
				],
				[
					10.740657797366111,
					1.074095279744256
				],
				[
					11.27765627055851,
					1.074095279744256
				],
				[
					12.351751550302652,
					1.611093752936938
				],
				[
					12.888750023495504,
					2.148141392809066
				],
				[
					13.962845303239646,
					3.222187505873819
				],
				[
					14.499843776432499,
					3.759235145745947
				],
				[
					15.573939056176641,
					4.833281258810757
				],
				[
					16.64793600256189,
					5.370328898682885
				],
				[
					17.185032809113636,
					5.907376538555013
				],
				[
					17.72203128230649,
					6.981422651619766
				],
				[
					18.259029755498887,
					6.981422651619766
				],
				[
					18.79612656205063,
					7.518470291491951
				],
				[
					19.33312503524303,
					8.055468764684576
				],
				[
					19.87012350843588,
					8.592516404556704
				],
				[
					19.87012350843588,
					9.666562517621514
				],
				[
					19.87012350843588,
					11.277656270558396
				],
				[
					19.87012350843588,
					11.814703910430524
				],
				[
					19.87012350843588,
					12.888750023495334
				],
				[
					19.87012350843588,
					13.96284530323959
				],
				[
					19.33312503524303,
					15.0368914163044
				],
				[
					18.79612656205063,
					15.573939056176528
				],
				[
					18.79612656205063,
					16.110937529369153
				],
				[
					18.259029755498887,
					16.110937529369153
				],
				[
					17.72203128230649,
					16.110937529369153
				],
				[
					16.64793600256189,
					16.110937529369153
				],
				[
					16.11093752936904,
					16.110937529369153
				],
				[
					14.499843776432499,
					16.110937529369153
				],
				[
					13.425748496688357,
					16.110937529369153
				],
				[
					12.351751550302652,
					16.110937529369153
				],
				[
					11.27765627055851,
					16.110937529369153
				],
				[
					10.740657797366111,
					16.110937529369153
				],
				[
					9.66656251762197,
					16.110937529369153
				],
				[
					9.129564044428662,
					16.110937529369153
				],
				[
					8.592467237877372,
					16.110937529369153
				],
				[
					7.518470291492122,
					16.110937529369153
				],
				[
					6.981373484940377,
					15.573939056176528
				],
				[
					6.444375011747979,
					15.573939056176528
				],
				[
					5.907376538555127,
					15.573939056176528
				],
				[
					5.370279732003837,
					15.0368914163044
				],
				[
					4.833281258810985,
					13.96284530323959
				],
				[
					3.7591859790663875,
					13.425797663367462
				],
				[
					2.685189032681592,
					12.888750023495334
				],
				[
					2.1480922261298474,
					12.351751550302652
				],
				[
					1.6110937529369949,
					12.351751550302652
				],
				[
					1.0740952797441423,
					12.351751550302652
				],
				[
					0.5369984731928525,
					11.814703910430524
				],
				[
					0,
					11.814703910430524
				],
				[
					-0.5369984731923978,
					11.814703910430524
				],
				[
					-0.5369984731923978,
					11.277656270558396
				],
				[
					-1.0740952797441423,
					11.277656270558396
				],
				[
					-1.6110937529365401,
					10.74065779736577
				],
				[
					-2.1480922261293927,
					10.203610157493642
				],
				[
					-3.2221875058739897,
					9.666562517621514
				],
				[
					-3.7591859790663875,
					9.129564044428832
				],
				[
					-4.296282785618132,
					8.592516404556704
				],
				[
					-5.370279732002928,
					8.592516404556704
				],
				[
					-5.907376538554672,
					8.055468764684576
				],
				[
					-6.444375011747525,
					8.055468764684576
				],
				[
					-6.444375011747525,
					7.518470291491951
				],
				[
					-6.444375011747525,
					6.981422651619766
				],
				[
					-6.981373484940377,
					6.981422651619766
				],
				[
					-6.981373484940377,
					6.444375011747638
				],
				[
					-6.981373484940377,
					6.444375011747638
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 20,
			"versionNonce": 140228592,
			"isDeleted": false,
			"id": "NcInO8rs914wAUvLUs-eP",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2584.434696876827,
			"y": -380.3762367830831,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 26.34656333360317,
			"height": 16.52240236441378,
			"seed": 1671864592,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.8930906760824655,
					1.3396564556588828
				],
				[
					-0.8930906760824655,
					2.232747131741462
				],
				[
					-2.679312911317993,
					4.018969366976876
				],
				[
					-4.0189693669769895,
					5.358625822635872
				],
				[
					-7.144848057871286,
					7.144807174800803
				],
				[
					-9.824160969189279,
					9.824120086118796
				],
				[
					-12.949998777013434,
					10.717251645271858
				],
				[
					-16.07587746790773,
					12.50343299743679
				],
				[
					-18.755190379225724,
					13.396564556589851
				],
				[
					-21.434503290543717,
					14.736221012248848
				],
				[
					-23.66725042228518,
					15.629311688331313
				],
				[
					-25.006906877944175,
					16.075877467907844
				],
				[
					-25.900038437097237,
					16.52240236441378
				],
				[
					-26.34656333360317,
					16.52240236441378
				],
				[
					-26.34656333360317,
					16.52240236441378
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 16,
			"versionNonce": 1174354416,
			"isDeleted": false,
			"id": "bXKNBh6YLhyyzQsWLG_MR",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2559.874314895388,
			"y": -359.8348650516924,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 4.4655351465535205,
			"height": 6.6982822782949825,
			"seed": 105905936,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.446565779576531
				],
				[
					0,
					0.893131559153062
				],
				[
					0,
					1.7862222352355275
				],
				[
					0.446565779576531,
					3.5724444704709413
				],
				[
					1.3396564556589965,
					4.4655351465535205
				],
				[
					2.679312911317993,
					5.805191602212403
				],
				[
					2.679312911317993,
					6.251757381788934
				],
				[
					3.572444470471055,
					6.6982822782949825
				],
				[
					4.0189693669769895,
					6.6982822782949825
				],
				[
					4.4655351465535205,
					6.6982822782949825
				],
				[
					4.4655351465535205,
					6.6982822782949825
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 18,
			"versionNonce": 1206025200,
			"isDeleted": false,
			"id": "12A5uc2ZifZAp6RNDMCSv",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2883.2049168186736,
			"y": 43.23664673061114,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 19.589617726790493,
			"height": 21.040744804899987,
			"seed": 136158480,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.7255635390547468
				],
				[
					1.4510606528108383,
					1.4511270781094936
				],
				[
					2.9021877309205593,
					2.9021877309205593
				],
				[
					4.35324838373117,
					5.078811922785917
				],
				[
					7.255436114651729,
					7.255436114651729
				],
				[
					9.432060306517315,
					10.883120959328153
				],
				[
					12.334181612138764,
					13.05974515119351
				],
				[
					13.785308690248485,
					15.236369343059323
				],
				[
					15.96193288211407,
					16.687496421168817
				],
				[
					18.138557073979655,
					18.86412061303463
				],
				[
					18.864054187735746,
					19.589617726790493
				],
				[
					19.589617726790493,
					21.040744804899987
				],
				[
					19.589617726790493,
					21.040744804899987
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 21,
			"versionNonce": 1879932400,
			"isDeleted": false,
			"id": "znUR_l2PYLHJSfkywVJq1",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2875.949480704022,
			"y": 70.80726411110811,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 26.11949030238725,
			"height": 18.138490648680772,
			"seed": 2055699216,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.7254971137558641
				],
				[
					0,
					1.451060652810611
				],
				[
					2.902187730920332,
					2.1766241918653577
				],
				[
					5.078811922785917,
					2.902121305621449
				],
				[
					7.255436114651502,
					5.078745497487034
				],
				[
					10.883120959327925,
					6.529872575596755
				],
				[
					13.785308690248485,
					8.70649676746234
				],
				[
					15.961932882113842,
					10.883120959327925
				],
				[
					19.589617726790266,
					12.334181612138764
				],
				[
					20.315181265845013,
					14.510805804004349
				],
				[
					23.217368996765572,
					15.236369343059096
				],
				[
					24.66842964957641,
					16.687429995869934
				],
				[
					25.393993188631157,
					17.41299353492468
				],
				[
					26.11949030238725,
					17.41299353492468
				],
				[
					26.11949030238725,
					18.138490648680772
				],
				[
					26.11949030238725,
					18.138490648680772
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 17,
			"versionNonce": 529022960,
			"isDeleted": false,
			"id": "wiDNM3eEH2NDYHa4ydVaS",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2713.1405113423302,
			"y": -257.89752899369125,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 87.82908888818656,
			"height": 26.951151046214477,
			"seed": 366864,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					1.2682710191324986,
					-0.6341355095662493
				],
				[
					3.4877888459086535,
					-1.2682710191324986
				],
				[
					6.658524451465837,
					-2.536571067127852
				],
				[
					12.365831124150645,
					-4.121924355474903
				],
				[
					19.975573354397056,
					-6.975577691817421
				],
				[
					30.756022161337796,
					-10.146313297374377
				],
				[
					43.438935554702994,
					-13.951184412497696
				],
				[
					58.34133774598149,
					-18.073137796835454
				],
				[
					73.56082220647431,
					-22.51214442152491
				],
				[
					86.56081786905406,
					-26.63409780586278
				],
				[
					87.82908888818656,
					-26.951151046214477
				],
				[
					87.82908888818656,
					-26.951151046214477
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 25,
			"versionNonce": 1448788464,
			"isDeleted": false,
			"id": "A5TJxejnXJqm4PTXN8Ohh",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2807.945206951197,
			"y": -288.0194156454628,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 122.0729579531585,
			"height": 85.29251782105871,
			"seed": 739243792,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.6341355095662493,
					0
				],
				[
					1.9024645864244576,
					1.9024355575617165
				],
				[
					3.8049001439860604,
					3.487788845908767
				],
				[
					6.6585534803284645,
					7.292659961032086
				],
				[
					10.780477835803367,
					12.048748854936093
				],
				[
					16.804837748839873,
					18.390220066050006
				],
				[
					24.41457997908651,
					25.36579775786754
				],
				[
					33.92675776689475,
					32.658486747762254
				],
				[
					45.658482410342,
					41.219446756789694
				],
				[
					59.60963779397662,
					49.1462422273878
				],
				[
					74.51206901411797,
					58.02428450562968
				],
				[
					87.19495337862008,
					64.99989122630996
				],
				[
					99.24373126241926,
					71.34133340856101
				],
				[
					106.21930895423657,
					74.82912225446978
				],
				[
					112.24372692499878,
					78.3169401292414
				],
				[
					116.99981581890279,
					80.85351119636925
				],
				[
					119.53635785716779,
					83.07302902314541
				],
				[
					121.12174017437792,
					84.65838231149246
				],
				[
					122.0729579531585,
					85.29251782105871
				],
				[
					122.0729579531585,
					85.29251782105871
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 19,
			"versionNonce": 1401750512,
			"isDeleted": false,
			"id": "EQcY3Yjc1Jesl6TaUCOr2",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2710.6039112463395,
			"y": -256.94631121491045,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 9.512177787808014,
			"height": 6.975606720680275,
			"seed": 1662948624,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.31705324035169724,
					0.31708226921455207
				],
				[
					-0.6341355095662493,
					0.9512177787808014
				],
				[
					-1.2682710191324986,
					1.5853823172099055
				],
				[
					-1.9024355575616028,
					2.219517826776155
				],
				[
					-3.1707065766941014,
					3.170735605556956
				],
				[
					-4.439006624689455,
					4.121953384337758
				],
				[
					-5.707306672684808,
					4.756088893904007
				],
				[
					-6.975577691817307,
					5.390253432333225
				],
				[
					-8.24387773981266,
					6.024388941899474
				],
				[
					-8.87801324937891,
					6.341471211114026
				],
				[
					-9.195095518593462,
					6.658524451465723
				],
				[
					-9.512177787808014,
					6.658524451465723
				],
				[
					-9.512177787808014,
					6.975606720680275
				],
				[
					-9.512177787808014,
					6.975606720680275
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 29,
			"versionNonce": 891749872,
			"isDeleted": false,
			"id": "5tm1YdTJ2ApIn5EMzijp8",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2703.945386794874,
			"y": -248.385351205883,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 141.73144903834122,
			"height": 115.09735123247845,
			"seed": 984183568,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.9512177787808014,
					0.9512177787808014
				],
				[
					1.2683000479953535,
					2.5366000959908206
				],
				[
					2.536600095990707,
					4.439035653552423
				],
				[
					4.121953384337758,
					7.609742230246525
				],
				[
					6.02438894189936,
					10.780477835803481
				],
				[
					9.195124547456317,
					15.536566729707602
				],
				[
					13.634131172145999,
					20.609737892826274
				],
				[
					19.341437844830807,
					26.951180075077332
				],
				[
					27.26826234429177,
					33.92678679575761
				],
				[
					37.09749337245171,
					42.48774680478493
				],
				[
					48.195053477469855,
					51.04870681381226
				],
				[
					60.87793784197197,
					59.92672006319128
				],
				[
					73.87793350455172,
					70.07306238942851
				],
				[
					86.56081786905384,
					78.95107563880754
				],
				[
					98.92664899320448,
					87.51203564783486
				],
				[
					108.75593807909013,
					93.85350685894889
				],
				[
					118.26811586689814,
					99.8778667719854
				],
				[
					125.87785809714478,
					104.95106696396692
				],
				[
					132.5363825486104,
					108.75593807909024
				],
				[
					136.975360144437,
					111.92664465578434
				],
				[
					139.5119602404277,
					113.51202697299425
				],
				[
					141.41439579798953,
					114.78029799212675
				],
				[
					141.73144903834122,
					115.09735123247845
				],
				[
					141.73144903834122,
					115.09735123247845
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 25,
			"versionNonce": 405850096,
			"isDeleted": false,
			"id": "azM3oWzFzHjuf477K6m-4",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2844.0915115737307,
			"y": -133.28799997340468,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 109.70709780014522,
			"height": 52.31697783294476,
			"seed": 1495830800,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.6341064807031671,
					-0.31705324035169724
				],
				[
					0.9512177787808014,
					-0.6341064807033945
				],
				[
					1.9024355575616028,
					-1.9024355575616028
				],
				[
					3.1707065766941014,
					-2.853653336342404
				],
				[
					6.0243599130365055,
					-5.073142134255704
				],
				[
					9.829231028159711,
					-7.292630932169004
				],
				[
					14.585319922063945,
					-10.146284268511522
				],
				[
					20.926791133177858,
					-13.634102143283144
				],
				[
					29.170639844127663,
					-17.756026498758047
				],
				[
					38.36576439158421,
					-22.195062152310356
				],
				[
					49.780377736953824,
					-26.31698650778526
				],
				[
					62.14620886110447,
					-30.756022161337796
				],
				[
					74.51203998525511,
					-35.5121110552418
				],
				[
					85.92665333062473,
					-39.95114670879411
				],
				[
					94.80466658000387,
					-44.07307106426913
				],
				[
					101.78030232954711,
					-46.609671160259836
				],
				[
					105.90222668502179,
					-49.1462422273878
				],
				[
					108.43882678101272,
					-51.048677784949405
				],
				[
					109.70709780014522,
					-52.31697783294476
				],
				[
					109.70709780014522,
					-52.31697783294476
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 17,
			"versionNonce": 951208432,
			"isDeleted": false,
			"id": "uhjayAoPZeaGOV4oWswr2",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2950.3107914991047,
			"y": -189.0927666522581,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 18.39019103718738,
			"height": 17.121920018054652,
			"seed": 1444146960,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.6341064807033945,
					-0.31708226921455207
				],
				[
					-1.5853242594844232,
					-1.9024355575616028
				],
				[
					-3.1707065766941014,
					-3.170735605556956
				],
				[
					-5.073142134255704,
					-4.756088893904007
				],
				[
					-6.975577691817307,
					-6.658524451465723
				],
				[
					-9.195066489730834,
					-9.195095518593575
				],
				[
					-12.048719826073238,
					-11.414613345369844
				],
				[
					-14.585319922063945,
					-13.317048902931447
				],
				[
					-16.487755479625548,
					-15.536566729707602
				],
				[
					-17.756026498758047,
					-16.8048377488401
				],
				[
					-18.39019103718738,
					-17.121920018054652
				],
				[
					-18.39019103718738,
					-17.121920018054652
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 224,
			"versionNonce": 296979440,
			"isDeleted": false,
			"id": "gqnoK5hKPpbbTnx7Q1kQZ",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2807.4238081352178,
			"y": -218.4865314237196,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 8.253856893444663,
			"height": 6.8782170765340425,
			"seed": 434343184,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.09825420378570016,
					0
				],
				[
					0.19651740356152914,
					-0.09825420378570016
				],
				[
					0.2947806033373581,
					-0.09825420378570016
				],
				[
					0.3930348071228309,
					-0.19651740356152914
				],
				[
					0.4912980068986599,
					-0.19651740356152914
				],
				[
					1.5721572204722634,
					-0.09825420378570016
				],
				[
					1.866937823809394,
					0
				],
				[
					2.4564990304841103,
					0.3930438031131871
				],
				[
					2.7512796338214685,
					0.6878244064504315
				],
				[
					3.0460602371588266,
					0.8843418100119607
				],
				[
					3.1443234369346555,
					1.179122413349205
				],
				[
					3.2425866367104845,
					1.4739030166865632
				],
				[
					3.3408408404959573,
					1.6704294162382212
				],
				[
					3.3408408404959573,
					1.9652100195754656
				],
				[
					3.3408408404959573,
					2.1617274231369947
				],
				[
					3.3408408404959573,
					2.554771226250068
				],
				[
					3.3408408404959573,
					2.8495518295874263
				],
				[
					3.2425866367104845,
					3.2425866367104845
				],
				[
					3.1443234369346555,
					3.537367240047729
				],
				[
					3.0460602371588266,
					3.832147843385087
				],
				[
					2.8495428335972974,
					4.028674242936631
				],
				[
					2.6530254300357683,
					4.1269284467223315
				],
				[
					2.5547622302599393,
					4.3234548462739895
				],
				[
					2.35824482669841,
					4.42170905005969
				],
				[
					2.063464223361052,
					4.42170905005969
				],
				[
					1.866937823809394,
					4.519972249835519
				],
				[
					1.5721572204722634,
					4.519972249835519
				],
				[
					1.2773766171349052,
					4.519972249835519
				],
				[
					0.884341810011847,
					4.519972249835519
				],
				[
					0.687815410460189,
					4.519972249835519
				],
				[
					0.2947806033373581,
					4.519972249835519
				],
				[
					0.09825420378570016,
					4.519972249835519
				],
				[
					-0.19652639955165796,
					4.519972249835519
				],
				[
					-0.2947806033373581,
					4.519972249835519
				],
				[
					-0.3930438031131871,
					4.519972249835519
				],
				[
					-0.4913070028890161,
					4.3234548462739895
				],
				[
					-0.7860876062263742,
					4.3234548462739895
				],
				[
					-0.9826050097879033,
					4.028674242936631
				],
				[
					-1.179122413349205,
					4.028674242936631
				],
				[
					-1.4739030166865632,
					3.733893639599387
				],
				[
					-1.7686836200239213,
					3.537367240047729
				],
				[
					-2.0634642233612794,
					3.3408498364863135
				],
				[
					-2.2599906229129374,
					3.1443324329247844
				],
				[
					-2.4565080264744665,
					2.9478060333731264
				],
				[
					-2.6530254300357683,
					2.8495518295874263
				],
				[
					-2.6530254300357683,
					2.7512886298115973
				],
				[
					-2.6530254300357683,
					2.6530254300357683
				],
				[
					-2.6530254300357683,
					2.554771226250068
				],
				[
					-2.6530254300357683,
					2.456508026474353
				],
				[
					-2.6530254300357683,
					2.358244826698524
				],
				[
					-2.6530254300357683,
					2.2599906229128237
				],
				[
					-2.6530254300357683,
					2.0634642233611658
				],
				[
					-2.6530254300357683,
					1.9652100195754656
				],
				[
					-2.6530254300357683,
					1.8669468197997503
				],
				[
					-2.6530254300357683,
					1.7686836200239213
				],
				[
					-2.6530254300357683,
					1.6704294162382212
				],
				[
					-2.5547712262502955,
					1.6704294162382212
				],
				[
					-2.5547712262502955,
					1.5721662164623922
				],
				[
					-2.4565080264744665,
					1.4739030166865632
				],
				[
					-2.4565080264744665,
					1.375648812900863
				],
				[
					-2.3582448266986376,
					1.179122413349205
				],
				[
					-2.2599906229129374,
					1.179122413349205
				],
				[
					-2.1617274231371084,
					1.080868209563505
				],
				[
					-2.1617274231371084,
					0.9826050097877896
				],
				[
					-2.0634642233612794,
					0.7860876062262605
				],
				[
					-2.0634642233612794,
					0.6878244064504315
				],
				[
					-1.9652100195755793,
					0.5895612066746025
				],
				[
					-1.8669468197997503,
					0.5895612066746025
				],
				[
					-1.8669468197997503,
					0.4913070028889024
				],
				[
					-1.8669468197997503,
					0.3930438031131871
				],
				[
					-1.7686836200239213,
					0.2947806033373581
				],
				[
					-1.7686836200239213,
					0.19652639955165796
				],
				[
					-1.6704294162382212,
					0.09826319977582898
				],
				[
					-1.5721662164623922,
					0
				],
				[
					-1.5721662164623922,
					-0.09825420378570016
				],
				[
					-1.4739030166865632,
					-0.09825420378570016
				],
				[
					-1.277385613125034,
					-0.29478060333724443
				],
				[
					-1.0808682095637323,
					-0.39303480712305827
				],
				[
					-0.9826050097879033,
					-0.49129800689877356
				],
				[
					-0.9826050097879033,
					-0.5895612066746025
				],
				[
					-0.7860876062263742,
					-0.5895612066746025
				],
				[
					-0.7860876062263742,
					-0.6878154104603027
				],
				[
					-0.6878244064505452,
					-0.6878154104603027
				],
				[
					-0.6878244064505452,
					-0.7860786102361317
				],
				[
					-0.5895612066747162,
					-0.7860786102361317
				],
				[
					-0.4913070028890161,
					-0.7860786102361317
				],
				[
					-0.3930438031131871,
					-0.7860786102361317
				],
				[
					-0.19652639955165796,
					-0.7860786102361317
				],
				[
					0,
					-0.7860786102361317
				],
				[
					0.19651740356152914,
					-0.7860786102361317
				],
				[
					0.4912980068986599,
					-0.7860786102361317
				],
				[
					0.687815410460189,
					-0.6878154104603027
				],
				[
					0.884341810011847,
					-0.6878154104603027
				],
				[
					1.179122413349205,
					-0.6878154104603027
				],
				[
					1.3756398169107342,
					-0.6878154104603027
				],
				[
					1.5721572204722634,
					-0.5895612066746025
				],
				[
					1.6704204202480923,
					-0.5895612066746025
				],
				[
					1.6704204202480923,
					-0.49129800689877356
				],
				[
					1.7686836200239213,
					-0.49129800689877356
				],
				[
					1.866937823809394,
					-0.29478060333724443
				],
				[
					1.866937823809394,
					-0.19651740356152914
				],
				[
					1.866937823809394,
					0
				],
				[
					2.063464223361052,
					0.3930438031131871
				],
				[
					2.161718427146752,
					0.6878244064504315
				],
				[
					2.35824482669841,
					1.080868209563505
				],
				[
					2.35824482669841,
					1.4739030166865632
				],
				[
					2.4564990304841103,
					1.7686836200239213
				],
				[
					2.5547622302599393,
					2.1617274231369947
				],
				[
					2.5547622302599393,
					2.358244826698524
				],
				[
					2.5547622302599393,
					2.6530254300357683
				],
				[
					2.5547622302599393,
					2.9478060333731264
				],
				[
					2.5547622302599393,
					3.1443324329247844
				],
				[
					2.5547622302599393,
					3.3408498364863135
				],
				[
					2.4564990304841103,
					3.733893639599387
				],
				[
					2.35824482669841,
					4.028674242936631
				],
				[
					2.259981626922581,
					4.3234548462739895
				],
				[
					2.063464223361052,
					4.519972249835519
				],
				[
					1.965201023585223,
					4.814752853172877
				],
				[
					1.866937823809394,
					5.011270256734292
				],
				[
					1.6704204202480923,
					5.30605086007165
				],
				[
					1.4739030166865632,
					5.5025772596231945
				],
				[
					1.3756398169107342,
					5.600831463408895
				],
				[
					1.3756398169107342,
					5.699094663184724
				],
				[
					1.179122413349205,
					5.797357862960553
				],
				[
					1.080859213573376,
					5.895612066746253
				],
				[
					0.786078610236018,
					5.895612066746253
				],
				[
					0.687815410460189,
					5.993875266522082
				],
				[
					0.3930348071228309,
					6.092138466297911
				],
				[
					0.19651740356152914,
					6.092138466297911
				],
				[
					-0.09826319977582898,
					6.092138466297911
				],
				[
					-0.3930438031131871,
					6.092138466297911
				],
				[
					-0.5895612066747162,
					6.092138466297911
				],
				[
					-0.8843418100120743,
					6.092138466297911
				],
				[
					-1.179122413349205,
					6.092138466297911
				],
				[
					-1.375648812900863,
					6.092138466297911
				],
				[
					-1.4739030166865632,
					6.092138466297911
				],
				[
					-1.6704294162382212,
					5.993875266522082
				],
				[
					-1.9652100195755793,
					5.993875266522082
				],
				[
					-2.0634642233612794,
					5.895612066746253
				],
				[
					-2.2599906229129374,
					5.797357862960553
				],
				[
					-2.5547712262502955,
					5.699094663184724
				],
				[
					-2.7512886298115973,
					5.699094663184724
				],
				[
					-3.0460692331489554,
					5.600831463408895
				],
				[
					-3.2425866367104845,
					5.5025772596231945
				],
				[
					-3.2425866367104845,
					5.30605086007165
				],
				[
					-3.4391130362621425,
					5.20779665628595
				],
				[
					-3.5373672400478426,
					5.109533456510121
				],
				[
					-3.5373672400478426,
					5.011270256734292
				],
				[
					-3.6356304398236716,
					4.913016052948592
				],
				[
					-3.7338936395995006,
					4.814752853172877
				],
				[
					-3.7338936395995006,
					4.716489653397048
				],
				[
					-3.8321478433852008,
					4.519972249835519
				],
				[
					-3.8321478433852008,
					4.42170905005969
				],
				[
					-3.9304110431610297,
					4.2251916464981605
				],
				[
					-4.028674242936859,
					4.028674242936631
				],
				[
					-4.1269284467223315,
					3.832147843385087
				],
				[
					-4.2251916464981605,
					3.537367240047729
				],
				[
					-4.3234548462739895,
					3.2425866367104845
				],
				[
					-4.3234548462739895,
					3.0460692331489554
				],
				[
					-4.42170905005969,
					2.8495518295874263
				],
				[
					-4.519972249835519,
					2.554771226250068
				],
				[
					-4.618235449611348,
					2.456508026474353
				],
				[
					-4.618235449611348,
					2.2599906229128237
				],
				[
					-4.618235449611348,
					2.1617274231369947
				],
				[
					-4.618235449611348,
					2.0634642233611658
				],
				[
					-4.618235449611348,
					1.8669468197997503
				],
				[
					-4.618235449611348,
					1.6704294162382212
				],
				[
					-4.618235449611348,
					1.5721662164623922
				],
				[
					-4.519972249835519,
					1.4739030166865632
				],
				[
					-4.519972249835519,
					1.277385613125034
				],
				[
					-4.42170905005969,
					1.080868209563505
				],
				[
					-4.42170905005969,
					0.9826050097877896
				],
				[
					-4.3234548462739895,
					0.7860876062262605
				],
				[
					-4.1269284467223315,
					0.6878244064504315
				],
				[
					-4.1269284467223315,
					0.5895612066746025
				],
				[
					-3.9304110431610297,
					0.3930438031131871
				],
				[
					-3.8321478433852008,
					0.2947806033373581
				],
				[
					-3.7338936395995006,
					0.19652639955165796
				],
				[
					-3.4391130362621425,
					0
				],
				[
					-3.3408498364863135,
					0
				],
				[
					-3.1443324329247844,
					-0.09825420378570016
				],
				[
					-2.9478060333731264,
					-0.19651740356152914
				],
				[
					-2.7512886298115973,
					-0.29478060333724443
				],
				[
					-2.6530254300357683,
					-0.39303480712305827
				],
				[
					-2.4565080264744665,
					-0.49129800689877356
				],
				[
					-2.2599906229129374,
					-0.49129800689877356
				],
				[
					-2.1617274231371084,
					-0.5895612066746025
				],
				[
					-1.9652100195755793,
					-0.5895612066746025
				],
				[
					-1.7686836200239213,
					-0.5895612066746025
				],
				[
					-1.5721662164623922,
					-0.5895612066746025
				],
				[
					-1.375648812900863,
					-0.5895612066746025
				],
				[
					-1.0808682095637323,
					-0.5895612066746025
				],
				[
					-0.7860876062263742,
					-0.6878154104603027
				],
				[
					-0.4913070028890161,
					-0.6878154104603027
				],
				[
					-0.09826319977582898,
					-0.6878154104603027
				],
				[
					0.2947806033373581,
					-0.6878154104603027
				],
				[
					0.786078610236018,
					-0.7860786102361317
				],
				[
					1.080859213573376,
					-0.7860786102361317
				],
				[
					1.2773766171349052,
					-0.7860786102361317
				],
				[
					1.6704204202480923,
					-0.7860786102361317
				],
				[
					1.866937823809394,
					-0.7860786102361317
				],
				[
					1.965201023585223,
					-0.7860786102361317
				],
				[
					2.063464223361052,
					-0.7860786102361317
				],
				[
					2.161718427146752,
					-0.6878154104603027
				],
				[
					2.259981626922581,
					-0.6878154104603027
				],
				[
					2.35824482669841,
					-0.6878154104603027
				],
				[
					2.4564990304841103,
					-0.6878154104603027
				],
				[
					2.4564990304841103,
					-0.5895612066746025
				],
				[
					2.6530254300357683,
					-0.39303480712305827
				],
				[
					2.8495428335972974,
					-0.19651740356152914
				],
				[
					3.0460602371588266,
					-0.09825420378570016
				],
				[
					3.1443234369346555,
					0.19652639955165796
				],
				[
					3.2425866367104845,
					0.4913070028889024
				],
				[
					3.4391040402717863,
					0.5895612066746025
				],
				[
					3.5373672400476153,
					0.7860876062262605
				],
				[
					3.6356214438333154,
					0.8843418100119607
				],
				[
					3.6356214438333154,
					0.9826050097877896
				],
				[
					3.6356214438333154,
					1.080868209563505
				],
				[
					3.6356214438333154,
					1.080868209563505
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 15,
			"versionNonce": 2101120496,
			"isDeleted": false,
			"id": "TxW940Mz1RtPym6wNAuiL",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2960.1316840560303,
			"y": -186.53238933768432,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 5.442735944910282,
			"height": 0.13956159087251763,
			"seed": 1041197840,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.27912318174503525,
					0
				],
				[
					0.6977951775074871,
					0
				],
				[
					1.2560159872869008,
					0
				],
				[
					1.8142367970665418,
					0
				],
				[
					2.791155156319064,
					0
				],
				[
					3.7680479618609297,
					0
				],
				[
					4.605391953385606,
					0
				],
				[
					5.163612763165247,
					-0.13956159087251763
				],
				[
					5.442735944910282,
					-0.13956159087251763
				],
				[
					5.442735944910282,
					-0.13956159087251763
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 18,
			"versionNonce": 1414877168,
			"isDeleted": false,
			"id": "bYCSAdm1VGynPLVvvcrQ_",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2843.7408692341005,
			"y": -128.47654351759206,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 0.9768928055418655,
			"height": 4.744953544258237,
			"seed": 1829734672,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.13954881401718922,
					0.41867199576233816
				],
				[
					-0.27912318174503525,
					1.1164671732697116
				],
				[
					-0.27912318174503525,
					1.5351391690320497
				],
				[
					-0.41867199576222447,
					2.372483160556726
				],
				[
					-0.41867199576222447,
					2.930703970336367
				],
				[
					-0.6977951775074871,
					3.6284991478437405
				],
				[
					-0.6977951775074871,
					3.907609552733561
				],
				[
					-0.8373439915246763,
					4.326281548495899
				],
				[
					-0.8373439915246763,
					4.465843139368417
				],
				[
					-0.8373439915246763,
					4.60539195338572
				],
				[
					-0.9768928055418655,
					4.60539195338572
				],
				[
					-0.9768928055418655,
					4.744953544258237
				],
				[
					-0.9768928055418655,
					4.744953544258237
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 13,
			"versionNonce": 252039664,
			"isDeleted": false,
			"id": "wnsmwXo03GftOMUaFWE-Q",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2805.867543469213,
			"y": -294.1456217038816,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 0.49784697491963925,
			"height": 3.9830265005443835,
			"seed": 1113319184,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.2489462784767511
				],
				[
					0,
					-0.9957623228903003
				],
				[
					0,
					-1.24468581035012
				],
				[
					0.24892348745970594,
					-2.240448133240534
				],
				[
					0.24892348745970594,
					-2.7383178991772184
				],
				[
					0.49784697491963925,
					-3.4851339435907676
				],
				[
					0.49784697491963925,
					-3.9830265005443835
				],
				[
					0.49784697491963925,
					-3.9830265005443835
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 16,
			"versionNonce": 1683362800,
			"isDeleted": false,
			"id": "Ly6UDBgGi63Fwmx2pShRB",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2691.853612161404,
			"y": -252.3239232167242,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 2.9872641776539695,
			"height": 0,
			"seed": 711755024,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.2489462784767511,
					0
				],
				[
					-0.7468160444134355,
					0
				],
				[
					-1.244708601367165,
					0
				],
				[
					-1.493632088826871,
					0
				],
				[
					-1.7425783673038495,
					0
				],
				[
					-2.240448133240534,
					0
				],
				[
					-2.489394411717285,
					0
				],
				[
					-2.738340690194036,
					0
				],
				[
					-2.9872641776539695,
					0
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
			"version": 144,
			"versionNonce": 1783502320,
			"isDeleted": false,
			"id": "TyoX8ys46FTI5B9Qh8dmE",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2952.6756906684236,
			"y": -181.3273809489308,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 101.20002685883992,
			"height": 53.10177833065029,
			"seed": 1119445776,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.3228021775724983
				],
				[
					-0.1613937003180581,
					0.3228021775724983
				],
				[
					-0.48421065482716585,
					0.4842106548269385
				],
				[
					-0.9684213096541043,
					0.6456043551449966
				],
				[
					-1.129815009971935,
					1.129815009971935
				],
				[
					-1.7754489189899232,
					1.4526319644809291
				],
				[
					-1.9368426193079813,
					1.7754341420534274
				],
				[
					-2.4210532741349198,
					1.9368426193078676
				],
				[
					-2.9052639289620856,
					2.4210532741349198
				],
				[
					-3.550868284106855,
					2.743855451707418
				],
				[
					-4.035078938934021,
					3.0666576292799164
				],
				[
					-4.680712847951781,
					3.3894745837889104
				],
				[
					-5.164923502778947,
					3.712276761361295
				],
				[
					-5.810527857923944,
					4.196487416188347
				],
				[
					-6.617555467259763,
					4.5192895937608455
				],
				[
					-7.424553522722817,
					5.164908725842338
				],
				[
					-8.231581132058864,
					5.649119380669276
				],
				[
					-9.038608741394683,
					6.294738512750769
				],
				[
					-10.168423751366845,
					6.940342867895765
				],
				[
					-11.136845061020722,
					7.585961999977258
				],
				[
					-12.266660070992657,
					8.23158113205875
				],
				[
					-13.557898335155642,
					9.200002441712627
				],
				[
					-14.849136599318626,
					10.007015274112177
				],
				[
					-16.14034530960862,
					10.65263440619367
				],
				[
					-17.592977274089435,
					11.298238761338666
				],
				[
					-18.40000488342548,
					11.943857893420159
				],
				[
					-19.691243147588466,
					12.428068548247097
				],
				[
					-20.498241203051293,
					12.750870725819595
				],
				[
					-21.30526881238734,
					13.235081380646534
				],
				[
					-21.950873167532336,
					13.719292035473586
				],
				[
					-22.919294477186213,
					14.042108989982466
				],
				[
					-23.40350513201338,
					14.364911167555078
				],
				[
					-24.049139041031367,
					14.687713345127463
				],
				[
					-24.85613709649442,
					15.01053029963657
				],
				[
					-25.8245584061483,
					15.656134654781454
				],
				[
					-26.631586015484118,
					15.978951609290448
				],
				[
					-27.922824279647102,
					16.624555964435444
				],
				[
					-29.052639289619037,
					17.108766619262383
				],
				[
					-30.666664954418138,
					17.91579422859843
				],
				[
					-32.11929691889918,
					18.400004883425368
				],
				[
					-33.57192888338,
					19.207032492761414
				],
				[
					-35.18598410205186,
					19.85263684790641
				],
				[
					-36.638616066532904,
					20.498241203051407
				],
				[
					-37.76843107650484,
					20.982451857878345
				],
				[
					-39.38245674130394,
					21.628085766896334
				],
				[
					-40.673695005466925,
					22.27369012204133
				],
				[
					-41.80351001543886,
					22.435083822359275
				],
				[
					-42.77193132509274,
					22.919294477186327
				],
				[
					-43.740352634746614,
					23.403505132013265
				],
				[
					-44.70877394440072,
					23.72632208652226
				],
				[
					-45.677195254054595,
					24.049139041031253
				],
				[
					-46.80703981789952,
					24.533349695858192
				],
				[
					-47.936854827871684,
					24.856137096494194
				],
				[
					-49.06666983784362,
					25.17895405100319
				],
				[
					-50.196514401688546,
					25.663164705830127
				],
				[
					-51.64914636616959,
					25.98598166033912
				],
				[
					-52.940355076459355,
					26.631586015484118
				],
				[
					-54.3929870409404,
					27.11579667031117
				],
				[
					-55.84561900542121,
					27.600007325138108
				],
				[
					-57.1368572695842,
					28.245611680283105
				],
				[
					-58.42809553374718,
					28.5684286347921
				],
				[
					-59.55791054371912,
					29.052639289619037
				],
				[
					-60.52633185337322,
					29.53684994444609
				],
				[
					-61.33335946270927,
					29.698243644764034
				],
				[
					-62.140357518172095,
					30.182454299591086
				],
				[
					-62.94738512750814,
					30.505271254099966
				],
				[
					-63.75441273684419,
					30.828088208609074
				],
				[
					-64.56141079230702,
					31.312298863436013
				],
				[
					-65.52983210196112,
					31.79650951826295
				],
				[
					-66.498253411615,
					32.28072017309
				],
				[
					-67.30528102095104,
					32.603507573726006
				],
				[
					-68.11230863028686,
					33.249141482743994
				],
				[
					-69.08072993994097,
					33.57192888337988
				],
				[
					-70.04915124959484,
					34.21756279239787
				],
				[
					-71.01757255924895,
					34.54035019303387
				],
				[
					-72.14738756922088,
					35.34737780236992
				],
				[
					-73.11580887887476,
					35.9929821575148
				],
				[
					-74.2456238888467,
					36.63861606653279
				],
				[
					-75.2140451985008,
					37.12282672135984
				],
				[
					-76.34388976234573,
					37.76843107650484
				],
				[
					-77.3123110719996,
					38.25264173133178
				],
				[
					-78.11930912746266,
					38.73685238615883
				],
				[
					-79.08773043711653,
					39.22106304098577
				],
				[
					-79.89475804645258,
					39.70527369581271
				],
				[
					-80.70178565578863,
					40.0280906503217
				],
				[
					-81.50878371125145,
					40.51230130514875
				],
				[
					-82.3158113205875,
					40.835088705784756
				],
				[
					-82.63862827509638,
					41.319299360611694
				],
				[
					-83.2842326302416,
					41.48072261480263
				],
				[
					-83.76844328506854,
					41.96493326962968
				],
				[
					-84.25265393989548,
					42.287720670265685
				],
				[
					-84.73686459472242,
					42.61053762477468
				],
				[
					-85.38246894986742,
					43.09474827960162
				],
				[
					-86.0281028588854,
					43.57895893442867
				],
				[
					-86.6737072140304,
					44.224563289573666
				],
				[
					-87.64212852368428,
					44.708773944400605
				],
				[
					-88.61054983333838,
					45.35440785341859
				],
				[
					-89.90178809750114,
					45.83861850824553
				],
				[
					-91.35442006198218,
					46.645616563708586
				],
				[
					-92.48423507195412,
					47.129827218535524
				],
				[
					-93.61405008192605,
					47.61403787336246
				],
				[
					-94.4210776912621,
					48.098248528189515
				],
				[
					-94.90528834608904,
					48.098248528189515
				],
				[
					-95.0666820464071,
					48.25967178238045
				],
				[
					-95.22810530059814,
					48.42106548269851
				],
				[
					-95.3894990009162,
					48.58245918301657
				],
				[
					-95.3894990009162,
					48.74388243720739
				],
				[
					-95.71231595542508,
					48.74388243720739
				],
				[
					-95.87370965574314,
					48.90527613752545
				],
				[
					-96.0351033560612,
					49.066669837843506
				],
				[
					-96.19652661025202,
					49.22809309203444
				],
				[
					-96.35792031057008,
					49.389486792352386
				],
				[
					-96.51931401088814,
					49.550880492670444
				],
				[
					-96.68073726507919,
					49.550880492670444
				],
				[
					-96.84213096539702,
					49.87369744717944
				],
				[
					-97.00352466571508,
					50.03509114749738
				],
				[
					-97.32634162022396,
					50.35790810200649
				],
				[
					-97.64915857473306,
					50.519301802324435
				],
				[
					-97.97194597536895,
					50.84211875683343
				],
				[
					-98.29476292987806,
					51.00351245715149
				],
				[
					-98.778973584705,
					51.32632941166037
				],
				[
					-98.778973584705,
					51.64914636616936
				],
				[
					-99.10179053921411,
					51.810540066487306
				],
				[
					-99.26318423953194,
					51.810540066487306
				],
				[
					-99.42457793985,
					51.810540066487306
				],
				[
					-99.42457793985,
					51.971933766805364
				],
				[
					-99.58600119404105,
					51.971933766805364
				],
				[
					-99.58600119404105,
					52.133357020996414
				],
				[
					-99.74739489435888,
					52.29475072131436
				],
				[
					-99.74739489435888,
					52.4561444216323
				],
				[
					-99.90878859467693,
					52.4561444216323
				],
				[
					-100.23160554918604,
					52.61756767582335
				],
				[
					-100.23160554918604,
					52.77896137614141
				],
				[
					-100.55442250369492,
					52.77896137614141
				],
				[
					-100.71581620401298,
					52.940355076459355
				],
				[
					-100.87720990433104,
					53.10177833065029
				],
				[
					-101.03863315852186,
					53.10177833065029
				],
				[
					-101.20002685883992,
					53.10177833065029
				],
				[
					-101.20002685883992,
					53.10177833065029
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 19,
			"versionNonce": 905304048,
			"isDeleted": false,
			"id": "FTAhNioOf3sY9m0Dd6EpK",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3726.288551736151,
			"y": -658.7647364553258,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 0.15776377106976724,
			"height": 30.289719676587595,
			"seed": 968524048,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.6310334193849485
				],
				[
					0,
					1.8931074797867495
				],
				[
					0,
					3.628458410135181
				],
				[
					0,
					5.679322439360192
				],
				[
					0,
					8.67674020847852
				],
				[
					0,
					11.358644878720384
				],
				[
					0,
					14.513826418908877
				],
				[
					0.15776377106976724,
					17.19572386751878
				],
				[
					0.15776377106976724,
					20.035385087198847
				],
				[
					0.15776377106976724,
					23.032810077949136
				],
				[
					0.15776377106976724,
					25.71470752655904
				],
				[
					0.15776377106976724,
					28.23885564736264
				],
				[
					0.15776377106976724,
					30.289719676587595
				],
				[
					0.15776377106976724,
					30.289719676587595
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 26,
			"versionNonce": 2069191152,
			"isDeleted": false,
			"id": "_DP4g7jiM_1WPILBdrPtO",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3725.3419979962573,
			"y": -607.4930779516459,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 1.577594380910341,
			"height": 37.54663649685796,
			"seed": 786947856,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.6310406410168525
				],
				[
					0.157763771070222,
					1.7353581519803924
				],
				[
					0.315527542140444,
					2.8396612196800675
				],
				[
					0.4732768699468579,
					4.25949182952013
				],
				[
					0.4732768699468579,
					5.679322439360192
				],
				[
					0.4732768699468579,
					7.256916820270419
				],
				[
					0.4732768699468579,
					9.150024300057112
				],
				[
					0.4732768699468579,
					11.200895550914026
				],
				[
					0.4732768699468579,
					13.567279900647407
				],
				[
					0.4732768699468579,
					15.933664250380843
				],
				[
					0.4732768699468579,
					18.615561698990746
				],
				[
					0.4732768699468579,
					21.13970981979429
				],
				[
					0.4732768699468579,
					23.821607268404193
				],
				[
					0.6310406410170799,
					26.661268488084318
				],
				[
					0.7888044120873019,
					28.712139738941175
				],
				[
					0.7888044120873019,
					30.920760317604447
				],
				[
					1.104317510963483,
					33.28714466733783
				],
				[
					1.262081282033705,
					35.33801591819474
				],
				[
					1.577594380910341,
					37.231123397981435
				],
				[
					1.577594380910341,
					37.54663649685796
				],
				[
					1.577594380910341,
					37.54663649685796
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 23,
			"versionNonce": 762616816,
			"isDeleted": false,
			"id": "4HzeSeF-vczqa5FnmrxpA",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3726.1308024083446,
			"y": -539.8144855492704,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 2.8396612196797832,
			"height": 9.781064941073964,
			"seed": 314146064,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.15774932780641393,
					0.3155275421403303
				],
				[
					0.3155130988761812,
					0.6310406410168525
				],
				[
					0.6310261977528171,
					0.9465537398933748
				],
				[
					0.6310261977528171,
					1.8931074797867495
				],
				[
					0.7887899688230391,
					2.6819118918737104
				],
				[
					1.104303067699675,
					3.628465631767085
				],
				[
					1.262066838769897,
					4.57501937166046
				],
				[
					1.419830609840119,
					5.521573111553835
				],
				[
					1.5775799376460782,
					6.3103630803769875
				],
				[
					1.5775799376460782,
					7.099153049200254
				],
				[
					1.7353437087163002,
					7.7301936902171065
				],
				[
					1.8931074797865222,
					8.51898365904026
				],
				[
					2.208620578663158,
					8.992260528987003
				],
				[
					2.524133677539794,
					9.465537398933634
				],
				[
					2.524133677539794,
					9.623301170003856
				],
				[
					2.6818974486095613,
					9.781064941073964
				],
				[
					2.8396612196797832,
					9.781064941073964
				],
				[
					2.8396612196797832,
					9.781064941073964
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 23,
			"versionNonce": 509320688,
			"isDeleted": false,
			"id": "bxPA29zW2YKcoDY216J3N",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3743.6420465963715,
			"y": -529.2446306393734,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 26.030227847067636,
			"height": 1.8931074797867495,
			"seed": 111631120,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.15774932780641393,
					0
				],
				[
					0.3155130988766359,
					0
				],
				[
					0.7887899688234938,
					0
				],
				[
					1.262066838769897,
					0
				],
				[
					2.050856807593391,
					0
				],
				[
					3.312938089627096,
					0
				],
				[
					5.048281798343396,
					0.157763771070222
				],
				[
					6.941389278130373,
					0.31551309887652224
				],
				[
					9.465537398933975,
					0.6310406410168525
				],
				[
					12.778475488560616,
					0.9465537398933748
				],
				[
					15.933649807117035,
					1.262066838769897
				],
				[
					19.08882412567391,
					1.5775943809102273
				],
				[
					21.928485345353693,
					1.7353437087165275
				],
				[
					23.82159282514067,
					1.7353437087165275
				],
				[
					25.083674107174375,
					1.8931074797867495
				],
				[
					25.872464075997414,
					1.8931074797867495
				],
				[
					26.030227847067636,
					1.8931074797867495
				],
				[
					26.030227847067636,
					1.8931074797867495
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 21,
			"versionNonce": 521297904,
			"isDeleted": false,
			"id": "Kd7XwkR8N4_sl4aKOey1Q",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3804.379235277353,
			"y": -529.7179075093201,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 30.920774760868426,
			"height": 0.47327686994663054,
			"seed": 1026128144,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.631055084280888,
					0
				],
				[
					1.262081282033705,
					0
				],
				[
					2.839661219680238,
					0.157763771070222
				],
				[
					4.732768699467215,
					0.31551309887652224
				],
				[
					7.099153049200595,
					0.47327686994663054
				],
				[
					9.781064941073964,
					0.47327686994663054
				],
				[
					12.778475488560616,
					0.47327686994663054
				],
				[
					15.933664250380843,
					0.47327686994663054
				],
				[
					19.088853012201525,
					0.47327686994663054
				],
				[
					21.455237361934905,
					0.47327686994663054
				],
				[
					24.137120367281113,
					0.47327686994663054
				],
				[
					26.661282931348524,
					0.47327686994663054
				],
				[
					28.396612196801016,
					0.47327686994663054
				],
				[
					29.974221020975165,
					0.31551309887652224
				],
				[
					30.920774760868426,
					0.31551309887652224
				],
				[
					30.920774760868426,
					0.31551309887652224
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 25,
			"versionNonce": 530637296,
			"isDeleted": false,
			"id": "Ori0X0URILfM9CPR7PWAS",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3879.9457851410157,
			"y": -528.2980768994802,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 23.663843497334256,
			"height": 0.3155275421403303,
			"seed": 1505220368,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.15774932780641393,
					0
				],
				[
					0.315527542140444,
					0
				],
				[
					0.9465537398937158,
					0
				],
				[
					1.577579937646533,
					0
				],
				[
					2.681911891873824,
					0
				],
				[
					4.101742501713943,
					0
				],
				[
					5.994849981500465,
					0
				],
				[
					8.203456116899815,
					0
				],
				[
					10.72761868096768,
					0
				],
				[
					13.09400303070106,
					0.157763771070222
				],
				[
					15.46038738043444,
					0.157763771070222
				],
				[
					17.511244188027376,
					0.157763771070222
				],
				[
					18.931074797867495,
					0.157763771070222
				],
				[
					20.1931560799012,
					0.157763771070222
				],
				[
					21.297459147600875,
					0
				],
				[
					22.086263559687723,
					-0.1577637710701083
				],
				[
					22.717289757440994,
					-0.1577637710701083
				],
				[
					23.190566627387398,
					-0.1577637710701083
				],
				[
					23.663843497334256,
					-0.1577637710701083
				],
				[
					23.663843497334256,
					-0.1577637710701083
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 21,
			"versionNonce": 1326392304,
			"isDeleted": false,
			"id": "fg04yz8_gGaL0VNgNl4Nn",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3925.853641525844,
			"y": -533.0308455989469,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 0.3154986556123731,
			"height": 20.350905407707273,
			"seed": 1355445520,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.4732768699467442
				],
				[
					0,
					-1.1043175109635968
				],
				[
					0,
					-1.8931074797867495
				],
				[
					0,
					-2.6818974486099023
				],
				[
					-0.15774932780641393,
					-4.417255600590352
				],
				[
					0,
					-5.837086210430357
				],
				[
					0.15774932780595918,
					-7.887943018023407
				],
				[
					0.15774932780595918,
					-9.307773627863469
				],
				[
					0.15774932780595918,
					-11.516408649790549
				],
				[
					0.15774932780595918,
					-13.409516129577241
				],
				[
					0.15774932780595918,
					-15.302623609363991
				],
				[
					0.15774932780595918,
					-16.880203547010353
				],
				[
					0.15774932780595918,
					-18.45779792792058
				],
				[
					0.15774932780595918,
					-19.56211543888412
				],
				[
					0.15774932780595918,
					-20.350905407707273
				],
				[
					0.15774932780595918,
					-20.350905407707273
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 23,
			"versionNonce": 996484592,
			"isDeleted": false,
			"id": "fmb6dZkKChYDwgckosOy3",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3925.6958921980377,
			"y": -582.5671531722782,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 0.6310261977528171,
			"height": 19.877628537760643,
			"seed": 1205424912,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.4732768699467442
				],
				[
					0,
					-1.262081282033705
				],
				[
					0.15774932780641393,
					-2.20863502192708
				],
				[
					0.3154986556123731,
					-3.470701860696977
				],
				[
					0.3154986556123731,
					-4.575019371660517
				],
				[
					0.47327686994640317,
					-5.837086210430357
				],
				[
					0.47327686994640317,
					-6.941403721393897
				],
				[
					0.6310261977528171,
					-8.203470560163794
				],
				[
					0.6310261977528171,
					-9.781064941073964
				],
				[
					0.6310261977528171,
					-10.885368008773696
				],
				[
					0.6310261977528171,
					-12.305198618613758
				],
				[
					0.6310261977528171,
					-13.725029228453764
				],
				[
					0.47327686994640317,
					-15.144859838293826
				],
				[
					0.47327686994640317,
					-16.722454219204053
				],
				[
					0.47327686994640317,
					-18.14228482904406
				],
				[
					0.47327686994640317,
					-19.56211543888412
				],
				[
					0.47327686994640317,
					-19.877628537760643
				],
				[
					0.47327686994640317,
					-19.877628537760643
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 24,
			"versionNonce": 1907025904,
			"isDeleted": false,
			"id": "tTuc9KE_AVI7sFAW-15JI",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3927.115722807878,
			"y": -645.6707406462568,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 2.050856807592936,
			"height": 21.297459147600648,
			"seed": 1968992528,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.15774932780595918,
					-2.36638434973338
				],
				[
					0.3154986556123731,
					-4.1017352800818685
				],
				[
					0.47327686994640317,
					-5.837086210430357
				],
				[
					0.6310261977528171,
					-7.256916820270362
				],
				[
					0.788775525559231,
					-8.676747430110424
				],
				[
					0.788775525559231,
					-9.938814268880265
				],
				[
					1.104303067699675,
					-11.043131779843861
				],
				[
					1.262052395506089,
					-12.14744206917544
				],
				[
					1.419830609840119,
					-13.093995809068815
				],
				[
					1.5775799376460782,
					-14.04054954896219
				],
				[
					1.735329265452492,
					-14.987103288855508
				],
				[
					1.735329265452492,
					-16.091413578187144
				],
				[
					1.8931074797865222,
					-17.03796731808052
				],
				[
					1.8931074797865222,
					-18.14228482904406
				],
				[
					1.8931074797865222,
					-19.246595118375637
				],
				[
					2.050856807592936,
					-20.193148858269012
				],
				[
					2.050856807592936,
					-21.139702598162387
				],
				[
					2.050856807592936,
					-21.297459147600648
				],
				[
					2.050856807592936,
					-21.297459147600648
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 11,
			"versionNonce": 501770736,
			"isDeleted": false,
			"id": "WLCkcMMGz4m-ZhGwxp__s",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3931.532963965204,
			"y": -697.7311999512079,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 0.4732768699468579,
			"height": 3.312938089626755,
			"seed": 13356816,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.15774932780641393,
					-0.7887935796391048
				],
				[
					0.315527542140444,
					-1.5775907700942184
				],
				[
					0.4732768699468579,
					-2.36638434973338
				],
				[
					0.4732768699468579,
					-3.1551779293725417
				],
				[
					0.4732768699468579,
					-3.312938089626755
				],
				[
					0.4732768699468579,
					-3.312938089626755
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 16,
			"versionNonce": 723889136,
			"isDeleted": false,
			"id": "BANEgnifun15uGdnR2lZE",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3931.2174364230636,
			"y": -714.9269274295426,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 6.310348637113293,
			"height": 0.9465537398933748,
			"seed": 1654615312,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15774932780641393,
					0
				],
				[
					-0.31549865561282786,
					0
				],
				[
					-0.4732768699468579,
					0
				],
				[
					-0.788775525559231,
					0
				],
				[
					-1.262052395506089,
					0
				],
				[
					-1.893107479786977,
					0
				],
				[
					-2.839661219680238,
					-0.15776377107016515
				],
				[
					-4.101713615186327,
					-0.31552754214038714
				],
				[
					-5.363794897219577,
					-0.6310406410168525
				],
				[
					-6.310348637113293,
					-0.9465537398933748
				],
				[
					-6.310348637113293,
					-0.9465537398933748
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 20,
			"versionNonce": 1667935728,
			"isDeleted": false,
			"id": "Z4qo-jjRQgLzJft5Cwqkq",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3915.1260228448764,
			"y": -718.5553930613097,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 28.86988906674742,
			"height": 0.7888044120869608,
			"seed": 1146047248,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.262052395506089,
					0
				],
				[
					-2.681883005346208,
					0
				],
				[
					-4.417241157326316,
					0
				],
				[
					-7.09915304920014,
					0.157763771070222
				],
				[
					-10.254312924492751,
					0.3155275421403303
				],
				[
					-13.25175235850702,
					0.3155275421403303
				],
				[
					-16.722439775940074,
					0.3155275421403303
				],
				[
					-20.19312719337313,
					0.157763771070222
				],
				[
					-23.348315955193357,
					-0.15774932780630024
				],
				[
					-25.71470030492719,
					-0.31551309887652224
				],
				[
					-27.29228024257327,
					-0.47327686994663054
				],
				[
					-28.23883398246653,
					-0.47327686994663054
				],
				[
					-28.71211085241339,
					-0.47327686994663054
				],
				[
					-28.86988906674742,
					-0.47327686994663054
				],
				[
					-28.86988906674742,
					-0.47327686994663054
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 20,
			"versionNonce": 264204272,
			"isDeleted": false,
			"id": "6tUqgIsn-0DH56PadkoKi",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3796.175779160453,
			"y": -723.2881617607765,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 17.195716645886932,
			"height": 2.05085680759305,
			"seed": 1616079120,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.315527542140444,
					0
				],
				[
					-0.4732768699468579,
					0
				],
				[
					-0.9465537398932611,
					-0.1577493278063571
				],
				[
					-1.8931074797865222,
					-0.1577493278063571
				],
				[
					-3.628465631767085,
					-0.4732768699467442
				],
				[
					-5.837071767166435,
					-0.7887899688232096
				],
				[
					-8.203456116899815,
					-1.262066838769897
				],
				[
					-10.412091138826781,
					-1.5775799376464192
				],
				[
					-11.989671076473314,
					-1.7353437087165844
				],
				[
					-13.725029228453877,
					-1.8931074797867495
				],
				[
					-14.671582968347138,
					-2.05085680759305
				],
				[
					-15.775886036046813,
					-2.05085680759305
				],
				[
					-16.880217990274105,
					-2.05085680759305
				],
				[
					-17.195716645886932,
					-2.05085680759305
				],
				[
					-17.195716645886932,
					-2.05085680759305
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 18,
			"versionNonce": 405533168,
			"isDeleted": false,
			"id": "QquXjbv7bZzpr8-MZfPoO",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3757.3670758248254,
			"y": -725.023505469493,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 5.206045569413618,
			"height": 0.4732768699466874,
			"seed": 1646511888,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.6310261977532718,
					0
				],
				[
					-0.9465537398932611,
					0
				],
				[
					-1.577579937646533,
					-0.15776377107016515
				],
				[
					-1.735358151980563,
					-0.15776377107016515
				],
				[
					-1.893107479786977,
					-0.15776377107016515
				],
				[
					-2.050856807592936,
					-0.15776377107016515
				],
				[
					-2.36638434973338,
					-0.3155130988764654
				],
				[
					-2.681911891873824,
					-0.3155130988764654
				],
				[
					-2.997410547486652,
					-0.3155130988764654
				],
				[
					-3.786214959573499,
					-0.4732768699466874
				],
				[
					-4.890518027273174,
					-0.4732768699466874
				],
				[
					-5.206045569413618,
					-0.4732768699466874
				],
				[
					-5.206045569413618,
					-0.4732768699466874
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 45,
			"versionNonce": 599274480,
			"isDeleted": false,
			"id": "q39E5eAx7ewN6GN8GVMTR",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3733.8609816552976,
			"y": -727.07437672035,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 2.8396612196797832,
			"height": 9.781064941073964,
			"seed": 1178101008,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.15774932780641393,
					0
				],
				[
					-0.47327686994640317,
					0
				],
				[
					-0.6310261977528171,
					0.157763771070222
				],
				[
					-0.9465537398932611,
					0.3155275421403303
				],
				[
					-0.9465537398932611,
					0.4732768699466874
				],
				[
					-1.104303067699675,
					0.4732768699466874
				],
				[
					-1.262066838769897,
					0.4732768699466874
				],
				[
					-1.419830609840119,
					0.4732768699466874
				],
				[
					-1.577579937646533,
					0.4732768699466874
				],
				[
					-1.7353437087163002,
					0.4732768699466874
				],
				[
					-1.8931074797865222,
					0.4732768699466874
				],
				[
					-1.8931074797865222,
					0.6310406410168525
				],
				[
					-2.050856807592936,
					0.7888044120870745
				],
				[
					-2.050856807592936,
					0.9465537398933748
				],
				[
					-2.36638434973338,
					1.262081282033705
				],
				[
					-2.524133677539794,
					1.5775943809102273
				],
				[
					-2.524133677539794,
					2.0508712508569147
				],
				[
					-2.681897448610016,
					2.681911891873767
				],
				[
					-2.8396612196797832,
					3.1551887618204546
				],
				[
					-2.8396612196797832,
					3.9439787306436074
				],
				[
					-2.8396612196797832,
					4.417255600590352
				],
				[
					-2.8396612196797832,
					5.206045569413504
				],
				[
					-2.8396612196797832,
					5.837086210430357
				],
				[
					-2.8396612196797832,
					6.310363080377044
				],
				[
					-2.8396612196797832,
					6.783639950323732
				],
				[
					-2.8396612196797832,
					7.099153049200254
				],
				[
					-2.8396612196797832,
					7.5724299191468845
				],
				[
					-2.8396612196797832,
					7.887957461287272
				],
				[
					-2.8396612196797832,
					8.045706789093629
				],
				[
					-2.8396612196797832,
					8.203470560163737
				],
				[
					-2.8396612196797832,
					8.51898365904026
				],
				[
					-2.8396612196797832,
					8.676747430110481
				],
				[
					-2.8396612196797832,
					8.83451120118059
				],
				[
					-2.8396612196797832,
					8.992260528986947
				],
				[
					-2.8396612196797832,
					9.150024300057112
				],
				[
					-2.8396612196797832,
					9.307788071127334
				],
				[
					-2.8396612196797832,
					9.465537398933634
				],
				[
					-2.8396612196797832,
					9.623301170003856
				],
				[
					-2.8396612196797832,
					9.781064941073964
				],
				[
					-2.8396612196797832,
					9.781064941073964
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 37,
			"versionNonce": 946615792,
			"isDeleted": false,
			"id": "hJFAXoCphsgzYZnKuYs5x",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3730.548043565671,
			"y": -697.7312107836557,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 2.36638434973338,
			"height": 15.775900479310621,
			"seed": 973685520,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.3155275421403303
				],
				[
					0,
					0.47327686994663054
				],
				[
					0.157763771070222,
					1.104317510963483
				],
				[
					0.157763771070222,
					1.8931074797866927
				],
				[
					0.315527542140444,
					2.5241481208035452
				],
				[
					0.315527542140444,
					3.47070186069692
				],
				[
					0.4732768699468579,
					4.25949182952013
				],
				[
					0.7888044120868472,
					5.2060455694134475
				],
				[
					0.9465537398932611,
					6.3103630803769875
				],
				[
					1.104317510963483,
					7.5724299191468845
				],
				[
					1.262081282033705,
					8.51898365904026
				],
				[
					1.419830609840119,
					9.30778807112722
				],
				[
					1.419830609840119,
					9.781064941073964
				],
				[
					1.419830609840119,
					10.254341811020595
				],
				[
					1.419830609840119,
					10.727618680967339
				],
				[
					1.419830609840119,
					10.88536800877364
				],
				[
					1.419830609840119,
					11.20089555091397
				],
				[
					1.419830609840119,
					11.674172420860657
				],
				[
					1.577594380910341,
					11.831921748667014
				],
				[
					1.577594380910341,
					12.305198618613645
				],
				[
					1.577594380910341,
					12.620726160754032
				],
				[
					1.7353581519801082,
					13.25175235850702
				],
				[
					1.8931074797865222,
					13.725029228453707
				],
				[
					2.050871250856744,
					14.198306098400394
				],
				[
					2.208635021926966,
					14.671582968347082
				],
				[
					2.208635021926966,
					14.987110510487469
				],
				[
					2.36638434973338,
					15.302623609363934
				],
				[
					2.36638434973338,
					15.4603873804341
				],
				[
					2.36638434973338,
					15.6181367082404
				],
				[
					2.208635021926966,
					15.6181367082404
				],
				[
					2.208635021926966,
					15.775900479310621
				],
				[
					2.208635021926966,
					15.775900479310621
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 302,
			"versionNonce": 1531967472,
			"isDeleted": false,
			"id": "Hz3__N5ZmeQmJ_cSXSg_8",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3776.1925950042914,
			"y": -610.2980203131505,
			"strokeColor": "#e03131",
			"backgroundColor": "transparent",
			"width": 4.209068505558207,
			"height": 5.227390528621811,
			"seed": 2081317136,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.06789020665246426,
					-0.06789020665235057
				],
				[
					0.13578041330492852,
					-0.13578041330470114
				],
				[
					0.13578041330492852,
					-0.2036644046127094
				],
				[
					0.20366440461293678,
					-0.27155461126506
				],
				[
					0.20366440461293678,
					-0.33944481791741055
				],
				[
					0.2715546112649463,
					-0.33944481791741055
				],
				[
					0.33944481791741055,
					-0.33944481791741055
				],
				[
					0.4073288092254188,
					-0.33944481791741055
				],
				[
					0.5431092225303473,
					-0.33944481791741055
				],
				[
					0.6109932138383556,
					-0.33944481791741055
				],
				[
					0.7467736271428294,
					-0.27155461126506
				],
				[
					0.8146576184508376,
					-0.2036644046127094
				],
				[
					1.0183220230633196,
					-0.13578041330470114
				],
				[
					1.1541024363682482,
					0.06788399130795142
				],
				[
					1.2219864276762564,
					0.2036644046127094
				],
				[
					1.3577668409807302,
					0.2715483959206608
				],
				[
					1.4256508322887385,
					0.4752128005333702
				],
				[
					1.4935410389412027,
					0.5431030071857208
				],
				[
					1.561431245593667,
					0.6788772051460228
				],
				[
					1.561431245593667,
					0.8825416097587322
				],
				[
					1.6293152369016752,
					1.0862060143713848
				],
				[
					1.6972054435536847,
					1.2898704189840942
				],
				[
					1.6972054435536847,
					1.5614250302490973
				],
				[
					1.765095650206149,
					1.8329796415141573
				],
				[
					1.8329796415141573,
					2.0366440461268667
				],
				[
					1.8329796415141573,
					2.2403084507395192
				],
				[
					1.8329796415141573,
					2.4439728553522286
				],
				[
					1.8329796415141573,
					2.5797470533125306
				],
				[
					1.8329796415141573,
					2.78341145792524
				],
				[
					1.8329796415141573,
					2.919185655885599
				],
				[
					1.8329796415141573,
					3.1228500604982514
				],
				[
					1.8329796415141573,
					3.190740267150602
				],
				[
					1.8329796415141573,
					3.3944046717633114
				],
				[
					1.6972054435536847,
					3.5301788697236134
				],
				[
					1.6293152369016752,
					3.598069076375964
				],
				[
					1.561431245593667,
					3.8017334809886734
				],
				[
					1.4256508322887385,
					4.005397885601326
				],
				[
					1.3577668409807302,
					4.073288092253733
				],
				[
					1.2219864276762564,
					4.209062290214035
				],
				[
					1.1541024363682482,
					4.344836488174337
				],
				[
					1.086212229715784,
					4.412726694826688
				],
				[
					0.9504380317557661,
					4.480616901479095
				],
				[
					0.8825478251033019,
					4.548500892787047
				],
				[
					0.7467736271428294,
					4.616391099439397
				],
				[
					0.6788834204903651,
					4.616391099439397
				],
				[
					0.6109932138383556,
					4.616391099439397
				],
				[
					0.47521901587788307,
					4.616391099439397
				],
				[
					0.2715546112649463,
					4.616391099439397
				],
				[
					0.20366440461293678,
					4.684281306091748
				],
				[
					0.06789020665246426,
					4.684281306091748
				],
				[
					0,
					4.684281306091748
				],
				[
					-0.06788399130800826,
					4.684281306091748
				],
				[
					-0.20366440461248203,
					4.684281306091748
				],
				[
					-0.2715483959204903,
					4.684281306091748
				],
				[
					-0.33943860257295455,
					4.684281306091748
				],
				[
					-0.4073288092254188,
					4.684281306091748
				],
				[
					-0.5431030071854366,
					4.684281306091748
				],
				[
					-0.6788772051459091,
					4.616391099439397
				],
				[
					-0.7467674117983734,
					4.480616901479095
				],
				[
					-0.8146576184508376,
					4.480616901479095
				],
				[
					-1.0183220230633196,
					4.344836488174337
				],
				[
					-1.1540962210237922,
					4.209062290214035
				],
				[
					-1.2219864276758017,
					4.073288092253733
				],
				[
					-1.28987041898381,
					3.9375076789489754
				],
				[
					-1.3577606256362742,
					3.8017334809886734
				],
				[
					-1.3577606256362742,
					3.6659592830283145
				],
				[
					-1.4256508322887385,
					3.598069076375964
				],
				[
					-1.4935348235967467,
					3.462294878415662
				],
				[
					-1.4935348235967467,
					3.326514465110961
				],
				[
					-1.4935348235967467,
					3.2586304738029526
				],
				[
					-1.4935348235967467,
					3.0549660691903
				],
				[
					-1.4935348235967467,
					2.919185655885599
				],
				[
					-1.561425030249211,
					2.7155212512728895
				],
				[
					-1.561425030249211,
					2.51185684666018
				],
				[
					-1.6293152369012205,
					2.3081924420475275
				],
				[
					-1.6293152369012205,
					2.104528037434818
				],
				[
					-1.6293152369012205,
					1.968753839474516
				],
				[
					-1.6293152369012205,
					1.8329796415141573
				],
				[
					-1.6293152369012205,
					1.6971992282094561
				],
				[
					-1.6293152369012205,
					1.5614250302490973
				],
				[
					-1.561425030249211,
					1.3577606256364447
				],
				[
					-1.561425030249211,
					1.2898704189840942
				],
				[
					-1.4935348235967467,
					1.0862060143713848
				],
				[
					-1.4256508322887385,
					0.8825416097587322
				],
				[
					-1.3577606256362742,
					0.8146576184507239
				],
				[
					-1.28987041898381,
					0.6109932138380714
				],
				[
					-1.2219864276758017,
					0.4752128005333702
				],
				[
					-1.1540962210237922,
					0.3394386025730114
				],
				[
					-1.086206014371328,
					0.2036644046127094
				],
				[
					-1.0183220230633196,
					0.06788399130795142
				],
				[
					-0.9504318164108554,
					0
				],
				[
					-0.8825416097588459,
					-0.2036644046127094
				],
				[
					-0.8146576184508376,
					-0.27155461126506
				],
				[
					-0.7467674117983734,
					-0.27155461126506
				],
				[
					-0.6109932138379008,
					-0.33944481791741055
				],
				[
					-0.5431030071854366,
					-0.40732880922536197
				],
				[
					-0.4073288092254188,
					-0.40732880922536197
				],
				[
					-0.33943860257295455,
					-0.47521901587771254
				],
				[
					-0.20366440461248203,
					-0.47521901587771254
				],
				[
					0,
					-0.47521901587771254
				],
				[
					0.06789020665246426,
					-0.47521901587771254
				],
				[
					0.2715546112649463,
					-0.5431092225300631
				],
				[
					0.4073288092254188,
					-0.5431092225300631
				],
				[
					0.5431092225303473,
					-0.5431092225300631
				],
				[
					0.6788834204903651,
					-0.5431092225300631
				],
				[
					0.8146576184508376,
					-0.5431092225300631
				],
				[
					0.8825478251033019,
					-0.5431092225300631
				],
				[
					0.9504380317557661,
					-0.5431092225300631
				],
				[
					1.086212229715784,
					-0.5431092225300631
				],
				[
					1.1541024363682482,
					-0.47521901587771254
				],
				[
					1.2898766343287207,
					-0.40732880922536197
				],
				[
					1.4256508322887385,
					-0.33944481791741055
				],
				[
					1.561431245593667,
					-0.2036644046127094
				],
				[
					1.765095650206149,
					-0.06789020665235057
				],
				[
					1.9687600548190858,
					0.06788399130795142
				],
				[
					2.1045342527791036,
					0.2036644046127094
				],
				[
					2.240308450739576,
					0.3394386025730114
				],
				[
					2.3760888640445046,
					0.5431030071857208
				],
				[
					2.3760888640445046,
					0.6109932138380714
				],
				[
					2.443972855352513,
					0.7467674117983734
				],
				[
					2.5118630620045224,
					0.8146576184507239
				],
				[
					2.5118630620045224,
					0.8825416097587322
				],
				[
					2.5118630620045224,
					0.9504318164110828
				],
				[
					2.5797532686569866,
					0.9504318164110828
				],
				[
					2.5797532686569866,
					1.0183220230634333
				],
				[
					2.5797532686569866,
					1.0862060143713848
				],
				[
					2.5797532686569866,
					1.1540962210237353
				],
				[
					2.5797532686569866,
					1.2219864276761427
				],
				[
					2.5797532686569866,
					1.2898704189840942
				],
				[
					2.5797532686569866,
					1.4256508322887953
				],
				[
					2.5797532686569866,
					1.4935348235967467
				],
				[
					2.5797532686569866,
					1.6293152369015047
				],
				[
					2.5797532686569866,
					1.6971992282094561
				],
				[
					2.5797532686569866,
					1.7650894348618067
				],
				[
					2.5797532686569866,
					1.8329796415141573
				],
				[
					2.5797532686569866,
					1.968753839474516
				],
				[
					2.5797532686569866,
					2.0366440461268667
				],
				[
					2.5797532686569866,
					2.104528037434818
				],
				[
					2.5797532686569866,
					2.1724182440871687
				],
				[
					2.5797532686569866,
					2.2403084507395192
				],
				[
					2.5797532686569866,
					2.3081924420475275
				],
				[
					2.5797532686569866,
					2.3081924420475275
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 222,
			"versionNonce": 812349936,
			"isDeleted": false,
			"id": "BFoxYtJ6",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3744.1448176858726,
			"y": -622.5312345325591,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 46.781005859375,
			"height": 5.992721317360295,
			"seed": 1002422032,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"fontSize": 4.993934431133579,
			"fontFamily": 3,
			"text": "Proximity Sensor",
			"rawText": "Proximity Sensor",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Proximity Sensor",
			"lineHeight": 1.2,
			"baseline": 5
		},
		{
			"type": "freedraw",
			"version": 1014,
			"versionNonce": 449231856,
			"isDeleted": false,
			"id": "IAuzoHm6rbuplpHwSZJ6s",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3795.070661854087,
			"y": -607.8786079464934,
			"strokeColor": "#e9ecef",
			"backgroundColor": "transparent",
			"width": 37.59505779346546,
			"height": 48.126772238935075,
			"seed": 2039831824,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.12765526773159763
				],
				[
					0,
					0.2553163791467341
				],
				[
					0,
					0.5744574703174408
				],
				[
					0,
					0.8297738494641749
				],
				[
					0,
					1.1489149406349384
				],
				[
					0,
					1.5318865875132133
				],
				[
					0.06382471202368833,
					1.9786887900991132
				],
				[
					0.1276611114149091,
					2.29782988126982
				],
				[
					0.1276611114149091,
					2.6808015281481516
				],
				[
					0.19148582343905218,
					2.9999426193188583
				],
				[
					0.19148582343905218,
					3.38291426619719
				],
				[
					0.19148582343905218,
					3.765885913075465
				],
				[
					0.19148582343905218,
					4.021202292222199
				],
				[
					0.19148582343905218,
					4.468004494808099
				],
				[
					0.2553105354627405,
					4.850976141686431
				],
				[
					0.2553105354627405,
					5.170117232857137
				],
				[
					0.2553105354627405,
					5.68074414746701
				],
				[
					0.19148582343905218,
					5.936060526613744
				],
				[
					0.1276611114149091,
					6.319032173492076
				],
				[
					0.1276611114149091,
					6.702003820370351
				],
				[
					0.1276611114149091,
					7.148806022956251
				],
				[
					0.1276611114149091,
					7.531777669834526
				],
				[
					0.1276611114149091,
					7.978574028736887
				],
				[
					0.1276611114149091,
					8.489206787030355
				],
				[
					0.1276611114149091,
					8.936003145932602
				],
				[
					0.19148582343905218,
					9.44663590422607
				],
				[
					0.2553105354627405,
					9.957262818836
				],
				[
					0.2553105354627405,
					10.404065021421843
				],
				[
					0.3191469348539613,
					10.850861380324147
				],
				[
					0.3191469348539613,
					11.297663582910047
				],
				[
					0.3191469348539613,
					11.744465785495947
				],
				[
					0.3191469348539613,
					12.127437432374222
				],
				[
					0.3191469348539613,
					12.574233791276527
				],
				[
					0.3191469348539613,
					13.021035993862426
				],
				[
					0.3191469348539613,
					13.404007640740758
				],
				[
					0.3191469348539613,
					13.850809843326601
				],
				[
					0.3191469348539613,
					14.297606202228906
				],
				[
					0.2553105354627405,
					14.744408404814806
				],
				[
					0.2553105354627405,
					15.318865875132246
				],
				[
					0.2553105354627405,
					15.765668077718146
				],
				[
					0.2553105354627405,
					16.27629499232802
				],
				[
					0.2553105354627405,
					16.78692190693795
				],
				[
					0.2553105354627405,
					17.29755466523136
				],
				[
					0.2553105354627405,
					17.744351024133664
				],
				[
					0.2553105354627405,
					18.191153226719564
				],
				[
					0.2553105354627405,
					18.637955429305464
				],
				[
					0.2553105354627405,
					19.084751788207768
				],
				[
					0.1276611114149091,
					19.40389872306207
				],
				[
					0.06382471202368833,
					19.786870369940345
				],
				[
					-0.06382471202414308,
					20.169842016818677
				],
				[
					-0.12766111141536385,
					20.61663837572098
				],
				[
					-0.19148582343950693,
					20.935785310575284
				],
				[
					-0.25531053546319527,
					21.382581669477588
				],
				[
					-0.25531053546319527,
					21.76555331635592
				],
				[
					-0.31914693485441603,
					22.276186074649388
				],
				[
					-0.31914693485441603,
					22.595327165820095
				],
				[
					-0.31914693485441603,
					23.105954080429967
				],
				[
					-0.31914693485441603,
					23.552756283015867
				],
				[
					-0.31914693485441603,
					23.999558485601767
				],
				[
					-0.31914693485441603,
					24.382530132480042
				],
				[
					-0.31914693485441603,
					24.765501779358374
				],
				[
					-0.3829716468785591,
					25.14847342623665
				],
				[
					-0.4467963589027022,
					25.53144507311498
				],
				[
					-0.4467963589027022,
					25.850586164285687
				],
				[
					-0.5106327582934682,
					26.16972725545645
				],
				[
					-0.5744574703176113,
					26.488874190310753
				],
				[
					-0.6382821823417544,
					26.80801528148146
				],
				[
					-0.6382821823417544,
					27.127156372652223
				],
				[
					-0.7021185817329751,
					27.510128019530498
				],
				[
					-0.7021185817329751,
					27.89309966640883
				],
				[
					-0.7659432937566635,
					28.212246601263132
				],
				[
					-0.7659432937566635,
					28.53138769243384
				],
				[
					-0.7659432937566635,
					28.91435933931217
				],
				[
					-0.7659432937566635,
					29.297330986190445
				],
				[
					-0.7659432937566635,
					29.680302633068777
				],
				[
					-0.7659432937566635,
					29.999443724239484
				],
				[
					-0.7659432937566635,
					30.382415371117816
				],
				[
					-0.7659432937566635,
					30.76538701799609
				],
				[
					-0.7659432937566635,
					31.020703397142825
				],
				[
					-0.7659432937566635,
					31.403675044021156
				],
				[
					-0.8297680057808066,
					31.722816135191863
				],
				[
					-0.8297680057808066,
					32.105787782070195
				],
				[
					-0.8936044051720273,
					32.4249347169245
				],
				[
					-0.8936044051720273,
					32.744075808095204
				],
				[
					-0.8936044051720273,
					33.06321689926597
				],
				[
					-0.8936044051720273,
					33.38236383412027
				],
				[
					-0.8936044051720273,
					33.63767436958341
				],
				[
					-0.8936044051720273,
					34.148307127876876
				],
				[
					-0.8297680057808066,
					34.403617663340015
				],
				[
					-0.8297680057808066,
					34.786589310218346
				],
				[
					-0.8297680057808066,
					35.10573624507265
				],
				[
					-0.8297680057808066,
					35.424877336243355
				],
				[
					-0.7659432937566635,
					35.74401842741412
				],
				[
					-0.7659432937566635,
					36.06316536226842
				],
				[
					-0.7659432937566635,
					36.31847589773156
				],
				[
					-0.7659432937566635,
					36.573792276878294
				],
				[
					-0.7659432937566635,
					36.82910865602503
				],
				[
					-0.7659432937566635,
					37.02059447946414
				],
				[
					-0.7659432937566635,
					37.2120803029033
				],
				[
					-0.7021185817329751,
					37.27590501492733
				],
				[
					-0.7021185817329751,
					37.4673908383665
				],
				[
					-0.6382821823417544,
					37.595051949781634
				],
				[
					-0.6382821823417544,
					37.72270721751323
				],
				[
					-0.5744574703176113,
					37.978023596659966
				],
				[
					-0.5106327582934682,
					38.10567886439151
				],
				[
					-0.5106327582934682,
					38.29716468783067
				],
				[
					-0.4467963589027022,
					38.424819955562214
				],
				[
					-0.4467963589027022,
					38.61630577900138
				],
				[
					-0.3829716468785591,
					38.807791602440545
				],
				[
					-0.3829716468785591,
					38.99927742587971
				],
				[
					-0.31914693485441603,
					39.19076324931888
				],
				[
					-0.25531053546319527,
					39.44608547214915
				],
				[
					-0.19148582343950693,
					39.57373489619715
				],
				[
					-0.12766111141536385,
					39.82905711902748
				],
				[
					-0.06382471202414308,
					39.956706543075484
				],
				[
					0,
					40.14819236651459
				],
				[
					0.1276611114149091,
					40.33967818995376
				],
				[
					0.19148582343905218,
					40.467339301368895
				],
				[
					0.3191469348539613,
					40.65882512480806
				],
				[
					0.38297164687810437,
					40.786486236223254
				],
				[
					0.5106327582934682,
					40.97797205966236
				],
				[
					0.7021185817325204,
					41.16945788310153
				],
				[
					0.7659432937562087,
					41.360943706540695
				],
				[
					0.8936044051715726,
					41.55242952997986
				],
				[
					1.0850902286106248,
					41.74391535341903
				],
				[
					1.404225476097963,
					41.999225888882165
				],
				[
					1.5318865875128722,
					42.1268870002973
				],
				[
					1.8510335223672882,
					42.44602224778447
				],
				[
					2.1701687698546266,
					42.637508071223635
				],
				[
					2.553140416732731,
					42.89283029405391
				],
				[
					2.93611206361129,
					43.084316117493074
				],
				[
					3.2552589984652514,
					43.27580194093224
				],
				[
					3.5744059333196674,
					43.53111247639538
				],
				[
					3.9573775801982265,
					43.65877358781057
				],
				[
					4.27651282768511,
					43.85025941124968
				],
				[
					4.595659762539526,
					44.04174523468885
				],
				[
					4.9786314094176305,
					44.10556994671282
				],
				[
					5.36160305629619,
					44.297055770151985
				],
				[
					5.808399415198437,
					44.42471688156712
				],
				[
					6.255207461467762,
					44.55236630561518
				],
				[
					6.765828532394153,
					44.74385212905429
				],
				[
					7.340286002711764,
					44.935337952493455
				],
				[
					8.042404584444284,
					45.12682377593262
				],
				[
					8.744523166176805,
					45.31830959937173
				],
				[
					9.382805348518104,
					45.509795422810896
				],
				[
					10.08492393025108,
					45.70128124625006
				],
				[
					10.914691936031431,
					45.8289423576652
				],
				[
					11.552974118373186,
					45.89276706968923
				],
				[
					12.191267988081563,
					46.020428181104364
				],
				[
					12.765725458399174,
					46.084252893128394
				],
				[
					13.404007640740474,
					46.1480892925195
				],
				[
					13.850803999642721,
					46.21191400454353
				],
				[
					14.36143675793619,
					46.27573871656756
				],
				[
					14.808233116838437,
					46.33957511595867
				],
				[
					15.318865875131905,
					46.403399827982696
				],
				[
					15.701837522010464,
					46.53106093939783
				],
				[
					16.148633880912712,
					46.59488565142186
				],
				[
					16.595441927182037,
					46.658710363445834
				],
				[
					17.042238286084284,
					46.78637147486097
				],
				[
					17.489034644986532,
					46.914032586276164
				],
				[
					17.87200629186509,
					46.97785729830014
				],
				[
					18.446463762182702,
					47.04168201032411
				],
				[
					18.765610697036664,
					47.1693431217393
				],
				[
					19.21240705593891,
					47.233167833763275
				],
				[
					19.59537870281747,
					47.233167833763275
				],
				[
					19.978350349695575,
					47.36082894517847
				],
				[
					20.361321996574134,
					47.36082894517847
				],
				[
					20.616644219404407,
					47.42465365720244
				],
				[
					20.93577946689129,
					47.488490056593605
				],
				[
					21.127265290330797,
					47.488490056593605
				],
				[
					21.38258751316107,
					47.55231476861758
				],
				[
					21.637898048624265,
					47.61613948064161
				],
				[
					21.957044983478227,
					47.61613948064161
				],
				[
					22.148530806917734,
					47.67997588003277
				],
				[
					22.531502453795838,
					47.67997588003277
				],
				[
					22.914474100674397,
					47.74380059205674
				],
				[
					23.23360934816128,
					47.80762530408077
				],
				[
					23.552756283015697,
					47.87146170347188
				],
				[
					23.9357279298938,
					47.93528641549591
				],
				[
					24.31869957677236,
					47.99911112751994
				],
				[
					24.637846511626776,
					47.99911112751994
				],
				[
					24.893157047089517,
					48.062947526911046
				],
				[
					25.212303981943933,
					48.062947526911046
				],
				[
					25.33995340599222,
					48.062947526911046
				],
				[
					25.53143922943127,
					48.062947526911046
				],
				[
					25.65910034084618,
					48.062947526911046
				],
				[
					25.786761452261544,
					48.126772238935075
				],
				[
					25.914410876309375,
					48.126772238935075
				],
				[
					26.105896699748882,
					48.126772238935075
				],
				[
					26.361218922579155,
					48.126772238935075
				],
				[
					26.68035417006604,
					48.126772238935075
				],
				[
					26.935676392896312,
					48.126772238935075
				],
				[
					27.31864803977487,
					48.126772238935075
				],
				[
					27.701619686652975,
					47.99911112751994
				],
				[
					28.020754934140314,
					47.93528641549591
				],
				[
					28.339901868994275,
					47.80762530408077
				],
				[
					28.531387692433782,
					47.67997588003277
				],
				[
					28.786698227896977,
					47.488490056593605
				],
				[
					28.850534627287743,
					47.29700423315444
				],
				[
					28.97818405133603,
					47.233167833763275
				],
				[
					29.10584516275094,
					46.97785729830014
				],
				[
					29.233506274166302,
					46.722546762837
				],
				[
					29.361155698214134,
					46.46722454000667
				],
				[
					29.488816809629498,
					46.1480892925195
				],
				[
					29.68030263306855,
					45.8289423576652
				],
				[
					29.871788456507602,
					45.509795422810896
				],
				[
					30.127098991970797,
					45.25448488734776
				],
				[
					30.38242121480107,
					44.935337952493455
				],
				[
					30.637731750264265,
					44.55236630561518
				],
				[
					30.89304228572746,
					44.23323105812801
				],
				[
					31.212189220581877,
					43.97790883529768
				],
				[
					31.40367504402093,
					43.59493718841935
				],
				[
					31.59516086745998,
					43.27580194093224
				],
				[
					31.786646690899033,
					42.89283029405391
				],
				[
					31.97813251433854,
					42.50985864717563
				],
				[
					32.10579362575345,
					42.1268870002973
				],
				[
					32.2972794491925,
					41.68007895402786
				],
				[
					32.42492887324079,
					41.360943706540695
				],
				[
					32.5525899846557,
					40.85031094824723
				],
				[
					32.61641469667984,
					40.40351458934492
				],
				[
					32.80790052011889,
					39.892881831051454
				],
				[
					32.935561631534256,
					39.44608547214915
				],
				[
					32.9993863435584,
					38.93545271385568
				],
				[
					33.19087216699745,
					38.424819955562214
				],
				[
					33.31853327841236,
					37.91419304095234
				],
				[
					33.446194389827724,
					37.40356612634247
				],
				[
					33.637680213266776,
					36.892933368049
				],
				[
					33.82916603670583,
					36.38230645343913
				],
				[
					33.89299074872997,
					35.871679538829255
				],
				[
					33.956815460754115,
					35.29722206851176
				],
				[
					33.956815460754115,
					34.72276459819432
				],
				[
					34.02065186014488,
					34.212131839900906
				],
				[
					34.02065186014488,
					33.63767436958341
				],
				[
					34.02065186014488,
					32.99939218724194
				],
				[
					34.02065186014488,
					32.48875942894847
				],
				[
					34.02065186014488,
					31.91430195863103
				],
				[
					34.02065186014488,
					31.403675044021156
				],
				[
					34.02065186014488,
					30.893048129411284
				],
				[
					34.02065186014488,
					30.382415371117816
				],
				[
					34.02065186014488,
					29.93561901221551
				],
				[
					34.084476572169024,
					29.55264736533718
				],
				[
					34.084476572169024,
					29.105845162751336
				],
				[
					34.14830128419317,
					28.722873515873005
				],
				[
					34.21213768358439,
					28.339901868994673
				],
				[
					34.21213768358439,
					27.956930222116398
				],
				[
					34.21213768358439,
					27.573958575238066
				],
				[
					34.275962395608076,
					27.25481748406736
				],
				[
					34.275962395608076,
					26.935670549213057
				],
				[
					34.275962395608076,
					26.552698902334726
				],
				[
					34.275962395608076,
					26.23355781116402
				],
				[
					34.275962395608076,
					25.978241432017285
				],
				[
					34.275962395608076,
					25.53144507311498
				],
				[
					34.33978710763222,
					25.212298138260678
				],
				[
					34.40362350702344,
					24.765501779358374
				],
				[
					34.46744821904758,
					24.382530132480042
				],
				[
					34.59510933046249,
					23.9357279298942
				],
				[
					34.72275875451032,
					23.4889257273083
				],
				[
					34.72275875451032,
					22.97829881269837
				],
				[
					34.85041986592569,
					22.595327165820095
				],
				[
					34.97808097734105,
					22.21235551894182
				],
				[
					35.04190568936474,
					21.76555331635592
				],
				[
					35.1695668007801,
					21.382581669477588
				],
				[
					35.1695668007801,
					20.999610022599256
				],
				[
					35.297216224827935,
					20.55281366369701
				],
				[
					35.361052624219155,
					20.169842016818677
				],
				[
					35.4248773362433,
					19.786870369940345
				],
				[
					35.48870204826699,
					19.467723435086043
				],
				[
					35.61636315968235,
					19.148582343915336
				],
				[
					35.680187871706494,
					18.76561069703706
				],
				[
					35.74402427109726,
					18.510294317890327
				],
				[
					35.8078489831214,
					18.191153226719564
				],
				[
					35.93551009453677,
					17.808181579841232
				],
				[
					35.999334806560455,
					17.425209932962957
				],
				[
					36.0631595185846,
					17.042238286084682
				],
				[
					36.12699591797582,
					16.72309719491392
				],
				[
					36.19082062999996,
					16.340125548035587
				],
				[
					36.25464534202365,
					15.957153901157312
				],
				[
					36.31848174141487,
					15.63800696630301
				],
				[
					36.31848174141487,
					15.382696430839871
				],
				[
					36.31848174141487,
					15.127380051693137
				],
				[
					36.382306453439014,
					14.935894228253972
				],
				[
					36.382306453439014,
					14.744408404814806
				],
				[
					36.44613116546316,
					14.489092025668072
				],
				[
					36.44613116546316,
					14.361436757936474
				],
				[
					36.50996756485392,
					14.233781490204933
				],
				[
					36.50996756485392,
					14.10612037878974
				],
				[
					36.50996756485392,
					13.91463455535063
				],
				[
					36.573792276878066,
					13.723148731911465
				],
				[
					36.573792276878066,
					13.659324019887492
				],
				[
					36.573792276878066,
					13.467838196448326
				],
				[
					36.573792276878066,
					13.340177085033133
				],
				[
					36.573792276878066,
					13.212521817301592
				],
				[
					36.63761698890221,
					13.021035993862426
				],
				[
					36.63761698890221,
					12.957205438154858
				],
				[
					36.70145338829343,
					12.765719614715692
				],
				[
					36.70145338829343,
					12.638064346984095
				],
				[
					36.70145338829343,
					12.574233791276527
				],
				[
					36.70145338829343,
					12.446578523544986
				],
				[
					36.70145338829343,
					12.38274796783736
				],
				[
					36.70145338829343,
					12.318923255813388
				],
				[
					36.70145338829343,
					12.38274796783736
				],
				[
					36.70145338829343,
					12.510409079252554
				],
				[
					36.63761698890221,
					12.638064346984095
				],
				[
					36.573792276878066,
					12.82955017042326
				],
				[
					36.44613116546316,
					12.957205438154858
				],
				[
					36.382306453439014,
					13.021035993862426
				],
				[
					36.25464534202365,
					13.148691261594024
				],
				[
					36.12699591797582,
					13.27635237300916
				],
				[
					35.999334806560455,
					13.340177085033133
				],
				[
					35.871673695145546,
					13.404007640740758
				],
				[
					35.680187871706494,
					13.467838196448326
				],
				[
					35.48870204826699,
					13.595493464179867
				],
				[
					35.297216224827935,
					13.595493464179867
				],
				[
					34.91424457794983,
					13.659324019887492
				],
				[
					34.59510933046249,
					13.786979287619033
				],
				[
					34.21213768358439,
					13.91463455535063
				],
				[
					33.70150492529092,
					14.042295666765767
				],
				[
					33.25470856638867,
					14.042295666765767
				],
				[
					32.68025109607106,
					14.233781490204933
				],
				[
					32.10579362575345,
					14.361436757936474
				],
				[
					31.531336155436293,
					14.489092025668072
				],
				[
					30.95687868511868,
					14.489092025668072
				],
				[
					30.38242121480107,
					14.616753137083208
				],
				[
					29.935613168531745,
					14.616753137083208
				],
				[
					29.488816809629498,
					14.616753137083208
				],
				[
					29.10584516275094,
					14.616753137083208
				],
				[
					28.786698227896977,
					14.616753137083208
				],
				[
					28.46756298040964,
					14.616753137083208
				],
				[
					28.276077156970587,
					14.616753137083208
				],
				[
					27.95693022211617,
					14.616753137083208
				],
				[
					27.637783287261755,
					14.616753137083208
				],
				[
					27.25481164038365,
					14.616753137083208
				],
				[
					26.808015281481403,
					14.55292258137564
				],
				[
					26.361218922579155,
					14.55292258137564
				],
				[
					25.914410876309375,
					14.489092025668072
				],
				[
					25.403789805382985,
					14.425267313644042
				],
				[
					24.82933233506583,
					14.361436757936474
				],
				[
					24.38252428879605,
					14.233781490204933
				],
				[
					23.74424210645475,
					14.169950934497365
				],
				[
					23.23360934816128,
					14.10612037878974
				],
				[
					22.65915187784367,
					13.978465111058199
				],
				[
					22.148530806917734,
					13.91463455535063
				],
				[
					21.637898048624265,
					13.786979287619033
				],
				[
					21.191101689722018,
					13.723148731911465
				],
				[
					20.80813004284346,
					13.595493464179867
				],
				[
					20.361321996574134,
					13.531662908472299
				],
				[
					20.042186749086795,
					13.404007640740758
				],
				[
					19.59537870281747,
					13.27635237300916
				],
				[
					19.21240705593891,
					13.148691261594024
				],
				[
					18.701785985012975,
					13.021035993862426
				],
				[
					18.191153226719507,
					12.82955017042326
				],
				[
					17.616695756401896,
					12.574233791276527
				],
				[
					17.042238286084284,
					12.38274796783736
				],
				[
					16.403956103742985,
					12.25509270010582
				],
				[
					15.829498633425374,
					11.999776320959086
				],
				[
					15.318865875131905,
					11.80829049751992
				],
				[
					14.872069516229658,
					11.744465785495947
				],
				[
					14.489097869351554,
					11.616804674080754
				],
				[
					14.169950934497137,
					11.425318850641645
				],
				[
					13.850803999642721,
					11.361494138617616
				],
				[
					13.467832352764617,
					11.297663582910047
				],
				[
					13.148697105277279,
					11.106177759470881
				],
				[
					12.829550170422863,
					10.97852249173934
				],
				[
					12.382753811520615,
					10.850861380324147
				],
				[
					11.999782164642511,
					10.659375556884982
				],
				[
					11.4253246943249,
					10.467889733445872
				],
				[
					10.850867224007743,
					10.276403910006707
				],
				[
					10.212573354298911,
					10.021093374543568
				],
				[
					9.6381158839813,
					9.765776995396834
				],
				[
					8.99983370164,
					9.5104606162501
				],
				[
					8.425376231322389,
					9.255150080786962
				],
				[
					7.978579872420141,
					8.999833701640227
				],
				[
					7.595608225542037,
					8.87217843390863
				],
				[
					7.148800179272257,
					8.680692610469464
				],
				[
					6.957314355833205,
					8.489206787030355
				],
				[
					6.765828532394153,
					8.42537623132273
				],
				[
					6.5743427089551005,
					8.297720963591189
				],
				[
					6.382856885516048,
					8.170059852175996
				],
				[
					6.255207461467762,
					8.042404584444455
				],
				[
					5.999885238637489,
					7.914749316712857
				],
				[
					5.808399415198437,
					7.787088205297721
				],
				[
					5.553088879735242,
					7.595602381858555
				],
				[
					5.2977783442720465,
					7.404116558419389
				],
				[
					5.106292520832994,
					7.212630734980223
				],
				[
					4.914806697393942,
					7.021144911541114
				],
				[
					4.659484474563669,
					6.893489643809517
				],
				[
					4.467998651124162,
					6.702003820370351
				],
				[
					4.27651282768511,
					6.510517996931242
				],
				[
					4.148863403637279,
					6.319032173492076
				],
				[
					4.021202292221915,
					6.12754635005291
				],
				[
					3.8935411808070057,
					5.999891082321312
				],
				[
					3.7658917567587196,
					5.808405258882146
				],
				[
					3.702055357367499,
					5.68074414746701
				],
				[
					3.5105695339284466,
					5.4254336120038715
				],
				[
					3.3190837104893944,
					5.297772500588735
				],
				[
					3.191434286441563,
					5.04246196512554
				],
				[
					2.93611206361129,
					4.850976141686431
				],
				[
					2.808462639563004,
					4.659490318247265
				],
				[
					2.6169768161239517,
					4.531829206832128
				],
				[
					2.489315704708588,
					4.212688115661365
				],
				[
					2.3616545932936788,
					4.148857559953797
				],
				[
					2.2340051692458474,
					3.957371736514631
				],
				[
					2.1701687698546266,
					3.82971646878309
				],
				[
					2.1063440578304835,
					3.765885913075465
				],
				[
					2.0425193458063404,
					3.638230645343924
				],
				[
					1.9786829464151197,
					3.5105753776123265
				],
				[
					1.8510335223672882,
					3.4467448219047583
				],
				[
					1.8510335223672882,
					3.3190895541731606
				],
				[
					1.7871971229760675,
					3.191428442758024
				],
				[
					1.7233724109523791,
					3.0637731750264834
				],
				[
					1.659547698928236,
					2.9361179072948858
				],
				[
					1.5957112995370153,
					2.8084567958797493
				],
				[
					1.4680618754891839,
					2.6808015281481516
				],
				[
					1.4680618754891839,
					2.553146260416554
				],
				[
					1.34040076407382,
					2.4254851490014175
				],
				[
					1.276576052049677,
					2.361660436977388
				],
				[
					1.276576052049677,
					2.29782988126982
				],
				[
					1.212739652658911,
					2.2339993255622517
				],
				[
					1.1489149406347678,
					2.170174613538279
				],
				[
					1.1489149406347678,
					2.106344057830711
				],
				[
					1.1489149406347678,
					2.042513502123086
				],
				[
					1.0850902286106248,
					2.042513502123086
				],
				[
					1.0850902286106248,
					1.9786887900991132
				],
				[
					1.0850902286106248,
					1.914858234391545
				],
				[
					1.021253829219404,
					1.8510276786839768
				],
				[
					1.021253829219404,
					1.7233724109523791
				],
				[
					0.9574291171957157,
					1.7233724109523791
				],
				[
					0.9574291171957157,
					1.659541855244811
				],
				[
					0.8936044051715726,
					1.5957171432207815
				],
				[
					0.8936044051715726,
					1.7872029666599474
				],
				[
					0.8936044051715726,
					1.9786887900991132
				],
				[
					0.9574291171957157,
					2.4254851490014175
				],
				[
					1.021253829219404,
					2.9361179072948858
				],
				[
					1.1489149406347678,
					3.38291426619719
				],
				[
					1.276576052049677,
					3.8935470244906583
				],
				[
					1.34040076407382,
					4.404173939100531
				],
				[
					1.404225476097963,
					4.914800853710403
				],
				[
					1.404225476097963,
					5.361603056296303
				],
				[
					1.4680618754891839,
					5.872229970906176
				],
				[
					1.5318865875128722,
					6.255201617784508
				],
				[
					1.5318865875128722,
					6.829659088101948
				],
				[
					1.5957112995370153,
					7.3402918463954165
				],
				[
					1.5957112995370153,
					7.850918761005289
				],
				[
					1.7233724109523791,
					8.42537623132273
				],
				[
					1.8510335223672882,
					9.191319525079336
				],
				[
					2.0425193458063404,
					9.957262818836
				],
				[
					2.3616545932936788,
					10.787036668300175
				],
				[
					2.553140416732731,
					11.680635229788379
				],
				[
					2.744626240171783,
					12.510409079252554
				],
				[
					2.93611206361129,
					13.27635237300916
				],
				[
					2.93611206361129,
					14.10612037878974
				],
				[
					2.999948463002056,
					14.808238960522374
				],
				[
					2.999948463002056,
					15.510351698571412
				],
				[
					2.999948463002056,
					16.020978613181285
				],
				[
					2.999948463002056,
					16.595436083498782
				],
				[
					2.999948463002056,
					17.10606884179225
				],
				[
					2.999948463002056,
					17.68052631210969
				],
				[
					2.93611206361129,
					18.191153226719564
				],
				[
					2.872287351587147,
					18.893265964768602
				],
				[
					2.808462639563004,
					19.595384546501236
				],
				[
					2.744626240171783,
					20.361327840257843
				],
				[
					2.744626240171783,
					21.12727113401445
				],
				[
					2.680801528148095,
					22.084700251210222
				],
				[
					2.680801528148095,
					22.9144682569908
				],
				[
					2.6169768161239517,
					23.871897374186574
				],
				[
					2.6169768161239517,
					24.70167122365075
				],
				[
					2.6169768161239517,
					25.595269785138953
				],
				[
					2.553140416732731,
					26.36121307889556
				],
				[
					2.4254909926848995,
					27.19098692835979
				],
				[
					2.3616545932936788,
					27.89309966640883
				],
				[
					2.2340051692458474,
					28.595218248141407
				],
				[
					2.1701687698546266,
					29.169675718458905
				],
				[
					2.0425193458063404,
					29.680302633068777
				],
				[
					1.9786829464151197,
					30.382415371117816
				],
				[
					1.9148582343914313,
					30.829217573703716
				],
				[
					1.9148582343914313,
					31.403675044021156
				],
				[
					1.8510335223672882,
					31.91430195863103
				],
				[
					1.8510335223672882,
					32.4249347169245
				],
				[
					1.8510335223672882,
					32.99939218724194
				],
				[
					1.7871971229760675,
					33.44618854614424
				],
				[
					1.7871971229760675,
					33.95682130443771
				],
				[
					1.7871971229760675,
					34.53127877475521
				],
				[
					1.7871971229760675,
					34.978075133657455
				],
				[
					1.7233724109523791,
					35.424877336243355
				],
				[
					1.659547698928236,
					35.74401842741412
				],
				[
					1.659547698928236,
					36.126990074292394
				],
				[
					1.659547698928236,
					36.38230645343913
				],
				[
					1.659547698928236,
					36.509961721170725
				],
				[
					1.659547698928236,
					36.76527810031746
				],
				[
					1.7233724109523791,
					36.892933368049
				],
				[
					1.7871971229760675,
					37.084419191488166
				],
				[
					1.9148582343914313,
					37.2120803029033
				],
				[
					2.1063440578304835,
					37.4673908383665
				],
				[
					2.1701687698546266,
					37.658876661805664
				],
				[
					2.3616545932936788,
					37.978023596659966
				],
				[
					2.489315704708588,
					38.233334132123105
				],
				[
					2.744626240171783,
					38.55248106697741
				],
				[
					2.93611206361129,
					38.871622158148114
				],
				[
					3.2552589984652514,
					39.19076324931888
				],
				[
					3.4467448219047583,
					39.637571295588316
				],
				[
					3.702055357367499,
					39.892881831051454
				],
				[
					4.021202292221915,
					40.14819236651459
				],
				[
					4.340349227076331,
					40.40351458934492
				],
				[
					4.659484474563669,
					40.72264983683209
				],
				[
					5.106292520832994,
					40.97797205966236
				],
				[
					5.680749991150606,
					41.23328259512556
				],
				[
					6.382856885516048,
					41.424768418564724
				],
				[
					7.212636578663478,
					41.74391535341903
				],
				[
					8.233890407883337,
					41.999225888882165
				],
				[
					9.446630060542248,
					42.254536424345304
				],
				[
					10.467895577129184,
					42.44602224778447
				],
				[
					11.489149406349043,
					42.70134447061474
				],
				[
					12.574239634960122,
					42.89283029405391
				],
				[
					13.72315457559489,
					43.02047971810191
				],
				[
					14.744408404814749,
					43.148140829517104
				],
				[
					15.829498633425374,
					43.33962665295621
				],
				[
					16.723091351230323,
					43.467287764371406
				],
				[
					17.808181579840948,
					43.722598299834544
				],
				[
					18.829435409060807,
					43.85025941124968
				],
				[
					19.786864526256522,
					43.97790883529768
				],
				[
					20.68046893142855,
					44.04174523468885
				],
				[
					21.637898048624265,
					44.10556994671282
				],
				[
					22.531502453795838,
					44.10556994671282
				],
				[
					23.552756283015697,
					44.16939465873685
				],
				[
					24.38252428879605,
					44.16939465873685
				],
				[
					25.212303981943933,
					44.16939465873685
				],
				[
					25.978247275700596,
					44.16939465873685
				],
				[
					26.616529458041896,
					44.16939465873685
				],
				[
					27.127162216335364,
					44.16939465873685
				],
				[
					27.701619686652975,
					44.23323105812801
				],
				[
					28.148416045555223,
					44.297055770151985
				],
				[
					28.65904880384869,
					44.360880482176015
				],
				[
					29.04202045072725,
					44.360880482176015
				],
				[
					29.361155698214134,
					44.42471688156712
				],
				[
					29.744127345092693,
					44.42471688156712
				],
				[
					29.935613168531745,
					44.48854159359115
				],
				[
					30.190935391362018,
					44.48854159359115
				],
				[
					30.31858481540985,
					44.48854159359115
				],
				[
					30.573907038240122,
					44.42471688156712
				],
				[
					30.70155646228841,
					44.23323105812801
				],
				[
					30.89304228572746,
					44.16939465873685
				],
				[
					31.020703397142825,
					43.85025941124968
				],
				[
					31.148364508557734,
					43.59493718841935
				],
				[
					31.339850331996786,
					43.27580194093224
				],
				[
					31.40367504402093,
					42.76516918263877
				],
				[
					31.59516086745998,
					42.254536424345304
				],
				[
					31.786646690899033,
					41.68007895402786
				],
				[
					31.914307802314397,
					41.16945788310153
				],
				[
					31.97813251433854,
					40.531164013392925
				],
				[
					32.10579362575345,
					39.76522071963632
				],
				[
					32.2972794491925,
					38.93545271385568
				],
				[
					32.42492887324079,
					38.233334132123105
				],
				[
					32.48876527263201,
					37.3397355706349
				],
				[
					32.5525899846557,
					36.38230645343913
				],
				[
					32.5525899846557,
					35.488707891950924
				],
				[
					32.61641469667984,
					34.46744821904758
				],
				[
					32.61641469667984,
					33.51001910185181
				],
				[
					32.5525899846557,
					32.48875942894847
				],
				[
					32.48876527263201,
					31.531330311752697
				],
				[
					32.48876527263201,
					30.510076482532952
				],
				[
					32.42492887324079,
					29.55264736533718
				],
				[
					32.42492887324079,
					28.722873515873005
				],
				[
					32.42492887324079,
					27.8292749543848
				],
				[
					32.42492887324079,
					27.19098692835979
				],
				[
					32.48876527263201,
					26.297388366871587
				],
				[
					32.5525899846557,
					25.53144507311498
				],
				[
					32.61641469667984,
					24.893157047089915
				],
				[
					32.61641469667984,
					24.191044309040876
				],
				[
					32.61641469667984,
					23.3612704595767
				],
				[
					32.61641469667984,
					22.659157721527663
				],
				[
					32.61641469667984,
					21.829383872063488
				],
				[
					32.61641469667984,
					21.191095846038422
				],
				[
					32.61641469667984,
					20.361327840257843
				],
				[
					32.5525899846557,
					19.595384546501236
				],
				[
					32.48876527263201,
					19.02092707618374
				],
				[
					32.361104161216645,
					18.127322671011996
				],
				[
					32.233443049801735,
					17.489040488670526
				],
				[
					32.233443049801735,
					16.978407730377057
				],
				[
					32.233443049801735,
					16.65926663920635
				],
				[
					32.233443049801735,
					16.467780815767185
				],
				[
					32.233443049801735,
					16.340125548035587
				],
				[
					32.233443049801735,
					16.27629499232802
				],
				[
					32.16961833777759,
					16.27629499232802
				],
				[
					31.914307802314397,
					16.27629499232802
				],
				[
					31.59516086745998,
					16.27629499232802
				],
				[
					31.148364508557734,
					16.27629499232802
				],
				[
					30.510070638849356,
					16.27629499232802
				],
				[
					29.744127345092693,
					16.21246443662045
				],
				[
					28.786698227896977,
					16.21246443662045
				],
				[
					27.829269110700807,
					16.21246443662045
				],
				[
					26.808015281481403,
					16.21246443662045
				],
				[
					25.850586164285687,
					16.27629499232802
				],
				[
					25.02081815850488,
					16.403950260059617
				],
				[
					23.871903217870113,
					16.595436083498782
				],
				[
					22.850637701283176,
					16.72309719491392
				],
				[
					22.02086969550237,
					16.850752462645517
				],
				[
					20.93577946689129,
					16.914583018353085
				],
				[
					19.914525637671886,
					16.978407730377057
				],
				[
					18.765610697036664,
					16.978407730377057
				],
				[
					17.616695756401896,
					16.978407730377057
				],
				[
					16.403956103742985,
					16.978407730377057
				],
				[
					15.127380051692853,
					16.78692190693795
				],
				[
					13.850803999642721,
					16.595436083498782
				],
				[
					12.63806434698381,
					16.403950260059617
				],
				[
					11.4253246943249,
					16.148639724596478
				],
				[
					10.404059177737963,
					15.957153901157312
				],
				[
					9.446630060542248,
					15.765668077718146
				],
				[
					8.616862054761896,
					15.510351698571412
				],
				[
					7.914743473028921,
					15.318865875132246
				],
				[
					7.212636578663478,
					15.06354949598557
				],
				[
					6.5743427089551005,
					14.872063672546403
				],
				[
					6.06372163802871,
					14.616753137083208
				],
				[
					5.425427768319878,
					14.297606202228906
				],
				[
					4.723320873954435,
					14.042295666765767
				],
				[
					4.148863403637279,
					13.723148731911465
				],
				[
					3.5105695339284466,
					13.404007640740758
				],
				[
					2.872287351587147,
					13.021035993862426
				],
				[
					2.4254909926848995,
					12.765719614715692
				],
				[
					1.9786829464151197,
					12.446578523544986
				],
				[
					1.659547698928236,
					12.191262144398252
				],
				[
					1.404225476097963,
					11.999776320959086
				],
				[
					1.212739652658911,
					11.80829049751992
				],
				[
					1.0850902286106248,
					11.744465785495947
				],
				[
					1.021253829219404,
					11.680635229788379
				],
				[
					1.021253829219404,
					11.872121053227488
				],
				[
					1.021253829219404,
					12.318923255813388
				],
				[
					0.9574291171957157,
					12.893380726130829
				],
				[
					0.9574291171957157,
					13.659324019887492
				],
				[
					1.021253829219404,
					14.616753137083208
				],
				[
					1.1489149406347678,
					15.63800696630301
				],
				[
					1.276576052049677,
					16.72309719491392
				],
				[
					1.404225476097963,
					17.93583684757283
				],
				[
					1.5957112995370153,
					19.148582343915336
				],
				[
					1.659547698928236,
					20.425152552281816
				],
				[
					1.7871971229760675,
					21.637898048624322
				],
				[
					1.7871971229760675,
					22.78681298925926
				],
				[
					1.8510335223672882,
					23.999558485601767
				],
				[
					1.8510335223672882,
					25.212298138260678
				],
				[
					1.9786829464151197,
					26.488874190310753
				],
				[
					1.9786829464151197,
					27.8292749543848
				],
				[
					2.0425193458063404,
					29.105845162751336
				],
				[
					2.0425193458063404,
					30.446245926825384
				],
				[
					2.1063440578304835,
					31.78664669089943
				],
				[
					2.1063440578304835,
					32.93556163153437
				],
				[
					2.2978298812695357,
					34.403617663340015
				],
				[
					2.4254909926848995,
					35.61636315968252
				],
				[
					2.6169768161239517,
					36.701447544609834
				],
				[
					2.680801528148095,
					37.85036248524477
				],
				[
					2.744626240171783,
					38.61630577900138
				],
				[
					2.744626240171783,
					39.254599648709984
				],
				[
					2.808462639563004,
					39.82905711902748
				],
				[
					2.808462639563004,
					40.21202876590576
				],
				[
					2.808462639563004,
					40.531164013392925
				],
				[
					2.872287351587147,
					40.85031094824723
				],
				[
					2.872287351587147,
					41.04179677168639
				],
				[
					2.999948463002056,
					41.29710730714953
				],
				[
					3.1275978870503423,
					41.55242952997986
				],
				[
					3.2552589984652514,
					41.807740065443
				],
				[
					3.5105695339284466,
					42.06305060090614
				],
				[
					3.8297164687828626,
					42.254536424345304
				],
				[
					4.340349227076331,
					42.70134447061474
				],
				[
					4.850970298002721,
					42.89283029405391
				],
				[
					5.616913591759385,
					43.148140829517104
				],
				[
					6.5743427089551005,
					43.33962665295621
				],
				[
					7.787094048981089,
					43.59493718841935
				],
				[
					9.127494813055364,
					43.722598299834544
				],
				[
					10.659381400568236,
					43.78642301185852
				],
				[
					12.318917412129395,
					43.85025941124968
				],
				[
					13.978465111058085,
					43.85025941124968
				],
				[
					15.701837522010464,
					43.85025941124968
				],
				[
					17.3613852209387,
					43.85025941124968
				],
				[
					18.95709652047617,
					43.78642301185852
				],
				[
					20.488983107989043,
					43.53111247639538
				],
				[
					21.957044983478227,
					43.40345136498024
				],
				[
					23.2974457475525,
					43.27580194093224
				],
				[
					24.574010112235555,
					43.211965541541076
				],
				[
					25.914410876309375,
					43.211965541541076
				],
				[
					26.935676392896312,
					43.211965541541076
				],
				[
					28.276077156970587,
					43.211965541541076
				],
				[
					29.488816809629498,
					43.211965541541076
				],
				[
					30.637731750264265,
					43.27580194093224
				],
				[
					31.59516086745998,
					43.27580194093224
				],
				[
					32.48876527263201,
					43.33962665295621
				],
				[
					33.12704745497331,
					43.33962665295621
				],
				[
					33.51001910185141,
					43.33962665295621
				],
				[
					33.76532963731461,
					43.33962665295621
				],
				[
					33.82916603670583,
					43.211965541541076
				],
				[
					33.89299074872997,
					43.148140829517104
				],
				[
					33.956815460754115,
					42.89283029405391
				],
				[
					33.956815460754115,
					42.637508071223635
				],
				[
					33.956815460754115,
					42.254536424345304
				],
				[
					33.956815460754115,
					41.807740065443
				],
				[
					33.956815460754115,
					41.23328259512556
				],
				[
					33.89299074872997,
					40.65882512480806
				],
				[
					33.82916603670583,
					40.08436765449062
				],
				[
					33.637680213266776,
					39.12693853729485
				],
				[
					33.51001910185141,
					38.55248106697741
				],
				[
					33.3823579904365,
					37.72270721751323
				],
				[
					33.25470856638867,
					36.95676392375657
				],
				[
					32.935561631534256,
					36.06316536226842
				],
				[
					32.68025109607106,
					35.10573624507265
				],
				[
					32.2972794491925,
					33.95682130443771
				],
				[
					31.850471402923176,
					32.744075808095204
				],
				[
					31.212189220581877,
					31.403675044021156
				],
				[
					30.637731750264265,
					29.871788456507886
				],
				[
					30.063274279946654,
					28.46755713672627
				],
				[
					29.424992097605355,
					26.74418472577389
				],
				[
					29.04202045072725,
					25.53144507311498
				],
				[
					28.65904880384869,
					24.127213753333308
				],
				[
					28.339901868994275,
					22.9144682569908
				],
				[
					28.148416045555223,
					21.70172860433189
				],
				[
					27.95693022211617,
					20.68046893142855
				],
				[
					27.829269110700807,
					19.723039814232777
				],
				[
					27.701619686652975,
					18.76561069703706
				],
				[
					27.573958575238066,
					17.999667403280398
				],
				[
					27.446297463822702,
					17.29755466523136
				],
				[
					27.25481164038365,
					16.595436083498782
				],
				[
					27.190986928359507,
					16.27629499232802
				],
				[
					27.127162216335364,
					16.084809168888853
				],
				[
					27.127162216335364,
					16.020978613181285
				],
				[
					27.063325816944598,
					16.21246443662045
				],
				[
					26.999501104920455,
					16.65926663920635
				],
				[
					26.935676392896312,
					17.36137937725539
				],
				[
					26.935676392896312,
					18.254983782427132
				],
				[
					26.87183999350509,
					19.212412899622905
				],
				[
					26.87183999350509,
					19.97835619337951
				],
				[
					26.808015281481403,
					20.999610022599256
				],
				[
					26.74419056945726,
					22.531496610112526
				],
				[
					26.68035417006604,
					23.680411550747465
				],
				[
					26.616529458041896,
					25.467614517407412
				],
				[
					26.616529458041896,
					26.871845837189028
				],
				[
					26.552704746018208,
					28.595218248141407
				],
				[
					26.552704746018208,
					30.63773175026455
				],
				[
					26.552704746018208,
					32.4249347169245
				],
				[
					26.552704746018208,
					34.08447657216931
				],
				[
					26.425043634602844,
					35.424877336243355
				],
				[
					26.361218922579155,
					36.701447544609834
				],
				[
					26.23355781116379,
					37.978023596659966
				],
				[
					25.978247275700596,
					38.93545271385568
				],
				[
					25.786761452261544,
					39.57373489619715
				],
				[
					25.595275628822492,
					40.14819236651459
				],
				[
					25.33995340599222,
					40.59500041278409
				],
				[
					25.084642870529024,
					40.914135660271256
				],
				[
					24.893157047089517,
					41.16945788310153
				],
				[
					24.44636068818727,
					41.360943706540695
				],
				[
					24.063389041309165,
					41.55242952997986
				],
				[
					23.552756283015697,
					41.68007895402786
				],
				[
					22.786812989259033,
					41.74391535341903
				],
				[
					22.02086969550237,
					41.807740065443
				],
				[
					21.127265290330797,
					41.935401176858136
				],
				[
					20.425158395965354,
					41.935401176858136
				],
				[
					19.65921510220869,
					41.999225888882165
				],
				[
					19.02092123249986,
					42.06305060090614
				],
				[
					18.254977938743195,
					42.06305060090614
				],
				[
					17.489034644986532,
					41.999225888882165
				],
				[
					16.531605527790816,
					41.807740065443
				],
				[
					15.382690587156048,
					41.424768418564724
				],
				[
					14.297612045912501,
					40.914135660271256
				],
				[
					13.02103599386237,
					40.33967818995376
				],
				[
					11.680635229788095,
					39.50991018417318
				],
				[
					10.404059177737963,
					38.68013633470895
				],
				[
					9.127494813055364,
					37.658876661805664
				],
				[
					8.106229296468427,
					36.701447544609834
				],
				[
					7.084975467248569,
					35.61636315968252
				],
				[
					6.319032173491905,
					34.65893404248675
				],
				[
					5.744574703174294,
					33.765335480998544
				],
				[
					5.553088879735242,
					33.254702722705076
				],
				[
					5.489264167711099,
					32.744075808095204
				],
				[
					5.489264167711099,
					32.105787782070195
				],
				[
					5.489264167711099,
					31.403675044021156
				],
				[
					5.680749991150606,
					30.382415371117816
				],
				[
					5.872235814589658,
					29.169675718458905
				],
				[
					6.255207461467762,
					27.701613842969664
				],
				[
					6.70200382037001,
					26.16972725545645
				],
				[
					7.340286002711764,
					24.574015955919208
				],
				[
					8.106229296468427,
					23.105954080429967
				],
				[
					8.99983370164,
					21.70172860433189
				],
				[
					10.021087530859859,
					20.55281366369701
				],
				[
					11.042353047446795,
					19.595384546501236
				],
				[
					12.127431588690342,
					18.76561069703706
				],
				[
					13.276346529325565,
					18.254983782427132
				],
				[
					14.680583692790606,
					17.808181579841232
				],
				[
					15.893323345449517,
					17.744351024133664
				],
				[
					17.29754882154748,
					17.68052631210969
				],
				[
					18.637949585621755,
					17.808181579841232
				],
				[
					19.914525637671886,
					18.063497958987966
				],
				[
					21.063440578306654,
					18.510294317890327
				],
				[
					22.084694407526513,
					18.95709652047617
				],
				[
					22.914474100674397,
					19.595384546501236
				],
				[
					23.552756283015697,
					20.297497284550275
				],
				[
					23.999552641917944,
					20.999610022599256
				],
				[
					24.38252428879605,
					21.957039139795086
				],
				[
					24.893157047089517,
					23.233615191845104
				],
				[
					25.148467582552712,
					24.574015955919208
				],
				[
					25.467614517407128,
					26.23355781116402
				],
				[
					25.595275628822492,
					28.08458548984794
				],
				[
					25.65910034084618,
					30.318590659093786
				],
				[
					25.65910034084618,
					32.48875942894847
				],
				[
					25.65910034084618,
					34.72276459819432
				],
				[
					25.212303981943933,
					36.892933368049
				],
				[
					24.701671223650465,
					38.55248106697741
				],
				[
					23.999552641917944,
					40.14819236651459
				],
				[
					23.04212352472223,
					41.424768418564724
				],
				[
					21.89320858408746,
					42.38219753576044
				],
				[
					20.871954754867602,
					42.76516918263877
				],
				[
					19.65921510220869,
					42.89283029405391
				],
				[
					18.318814338134416,
					42.8289938946628
				],
				[
					16.850752462645232,
					42.44602224778447
				],
				[
					15.44652698654727,
					41.807740065443
				],
				[
					13.978465111058085,
					40.85031094824723
				],
				[
					12.829550170422863,
					39.956706543075484
				],
				[
					11.872121053227147,
					38.871622158148114
				],
				[
					10.978516648055574,
					37.72270721751323
				],
				[
					10.08492393025108,
					36.25465118570759
				],
				[
					9.382805348518104,
					34.53127877475521
				],
				[
					8.744523166176805,
					32.99939218724194
				],
				[
					8.29771511990748,
					31.467505599728725
				],
				[
					8.042404584444284,
					29.93561901221551
				],
				[
					8.042404584444284,
					28.786704071580573
				],
				[
					8.042404584444284,
					27.382472751798957
				],
				[
					8.29771511990748,
					26.16972725545645
				],
				[
					8.808347878200948,
					24.893157047089915
				],
				[
					9.318980636494416,
					23.871897374186574
				],
				[
					10.148748642274768,
					22.78681298925926
				],
				[
					10.72320611259238,
					22.21235551894182
				],
				[
					11.552974118373186,
					21.637898048624322
				],
				[
					12.446578523544758,
					21.318756957453616
				],
				[
					13.276346529325565,
					21.191095846038422
				],
				[
					14.425261469960333,
					21.191095846038422
				],
				[
					15.44652698654727,
					21.25492640174599
				],
				[
					16.723091351230323,
					21.574067492916754
				],
				[
					18.063492115304143,
					22.020869695502654
				],
				[
					19.46772927876964,
					22.659157721527663
				],
				[
					20.68046893142855,
					23.42510101528427
				],
				[
					21.765559160039174,
					24.191044309040876
				],
				[
					22.531502453795838,
					25.14847342623665
				],
				[
					23.10595992411345,
					26.16972725545645
				],
				[
					23.23360934816128,
					26.871845837189028
				],
				[
					23.361270459576644,
					28.020760777823966
				],
				[
					23.2974457475525,
					29.04201460704371
				],
				[
					22.914474100674397,
					30.318590659093786
				],
				[
					22.084694407526513,
					31.531330311752697
				],
				[
					20.871954754867602,
					32.61642054036366
				],
				[
					19.340068167354275,
					33.3185332784127
				],
				[
					17.68052046842604,
					33.765335480998544
				],
				[
					15.5741764105951,
					33.829160193022574
				],
				[
					14.106126222472994,
					33.765335480998544
				],
				[
					12.63806434698381,
					33.38236383412027
				],
				[
					11.361488294933679,
					32.93556163153437
				],
				[
					10.467895577129184,
					32.29727360550936
				],
				[
					9.957262818835716,
					31.467505599728725
				],
				[
					9.574291171957611,
					30.63773175026455
				],
				[
					9.318980636494416,
					29.61647207736121
				],
				[
					9.127494813055364,
					28.46755713672627
				],
				[
					9.127494813055364,
					27.510128019530498
				],
				[
					9.127494813055364,
					26.425043634603128
				],
				[
					9.255144237103195,
					25.403783961699844
				],
				[
					9.510466459933468,
					24.765501779358374
				],
				[
					9.829601707420807,
					24.191044309040876
				],
				[
					10.276409753690132,
					23.616586838723435
				],
				[
					10.850867224007743,
					23.233615191845104
				],
				[
					11.361488294933679,
					22.97829881269837
				],
				[
					12.382753811520615,
					22.85064354496683
				],
				[
					13.404007640740474,
					22.85064354496683
				],
				[
					14.744408404814749,
					23.042129368405995
				],
				[
					16.02098445686488,
					23.3612704595767
				],
				[
					17.3613852209387,
					23.999558485601767
				],
				[
					19.02092123249986,
					24.893157047089915
				],
				[
					20.16983617313508,
					25.722930896554146
				],
				[
					21.44641222518476,
					26.80801528148146
				],
				[
					22.531502453795838,
					28.020760777823966
				],
				[
					23.2974457475525,
					29.297330986190445
				],
				[
					23.74424210645475,
					30.57390119455698
				],
				[
					23.999552641917944,
					31.65899142316789
				],
				[
					24.063389041309165,
					33.06321689926597
				],
				[
					23.808066818478892,
					34.403617663340015
				],
				[
					23.23360934816128,
					35.74401842741412
				],
				[
					22.531502453795838,
					36.82910865602503
				],
				[
					21.31875111376985,
					37.595051949781634
				],
				[
					20.361321996574134,
					38.04184830868394
				],
				[
					19.02092123249986,
					38.169509420099075
				],
				[
					17.489034644986532,
					38.10567886439151
				],
				[
					16.403956103742985,
					37.7865377732208
				],
				[
					15.191204763716996,
					37.084419191488166
				],
				[
					13.914640399033942,
					36.06316536226842
				],
				[
					12.701889059007954,
					34.786589310218346
				],
				[
					11.489149406349043,
					33.190878010681104
				],
				[
					10.404059177737963,
					31.403675044021156
				],
				[
					9.446630060542248,
					29.744133188776345
				],
				[
					8.680686766785584,
					27.956930222116398
				],
				[
					8.170065695859194,
					26.80801528148146
				],
				[
					7.723257649589868,
					25.276128693968246
				],
				[
					7.595608225542037,
					24.318699576772474
				],
				[
					7.467947114126673,
					23.233615191845104
				],
				[
					7.404122402102985,
					22.722982433551635
				],
				[
					7.404122402102985,
					22.020869695502654
				],
				[
					7.404122402102985,
					21.318756957453616
				],
				[
					7.467947114126673,
					20.935785310575284
				],
				[
					7.723257649589868,
					20.55281366369701
				],
				[
					7.978579872420141,
					20.233666728842707
				],
				[
					8.425376231322389,
					20.169842016818677
				],
				[
					9.127494813055364,
					20.10601146111111
				],
				[
					10.08492393025108,
					20.169842016818677
				],
				[
					11.233838870885847,
					20.425152552281816
				],
				[
					12.510403235568901,
					20.999610022599256
				],
				[
					13.914640399033942,
					21.510242780892725
				],
				[
					15.44652698654727,
					22.34001078667336
				],
				[
					16.723091351230323,
					23.042129368405995
				],
				[
					18.127328514695364,
					23.999558485601767
				],
				[
					19.02092123249986,
					24.70167122365075
				],
				[
					19.72303981423238,
					25.467614517407412
				],
				[
					20.16983617313508,
					26.297388366871587
				],
				[
					20.29749728454999,
					26.999501104920625
				],
				[
					20.425158395965354,
					27.63778913094569
				],
				[
					20.425158395965354,
					28.339901868994673
				],
				[
					20.29749728454999,
					28.91435933931217
				],
				[
					19.914525637671886,
					29.424986253922043
				],
				[
					19.59537870281747,
					29.744133188776345
				],
				[
					19.21240705593891,
					29.871788456507886
				],
				[
					18.893271808452027,
					29.999443724239484
				],
				[
					18.57412487359761,
					29.999443724239484
				],
				[
					18.446463762182702,
					29.999443724239484
				],
				[
					18.191153226719507,
					29.93561901221551
				],
				[
					17.87200629186509,
					29.871788456507886
				],
				[
					17.552871044377753,
					29.61647207736121
				],
				[
					17.23372410952379,
					29.36116154189807
				],
				[
					16.403956103742985,
					28.722873515873005
				],
				[
					15.638012809986321,
					28.212246601263132
				],
				[
					14.552922581375242,
					27.382472751798957
				],
				[
					13.276346529325565,
					26.616529458042294
				],
				[
					12.063606876666654,
					25.978241432017285
				],
				[
					11.170002471494627,
					25.53144507311498
				],
				[
					10.595545001177015,
					25.339959249675815
				],
				[
					10.404059177737963,
					25.276128693968246
				],
				[
					10.531720289153327,
					25.276128693968246
				],
				[
					10.914691936031431,
					25.276128693968246
				],
				[
					11.29766358290999,
					25.467614517407412
				],
				[
					11.744459941812238,
					25.53144507311498
				],
				[
					12.382753811520615,
					25.722930896554146
				],
				[
					12.829550170422863,
					25.78675560857812
				],
				[
					13.404007640740474,
					25.850586164285687
				],
				[
					13.850803999642721,
					25.914416719993312
				],
				[
					14.106126222472994,
					25.978241432017285
				],
				[
					14.297612045912501,
					26.10590254343242
				],
				[
					14.425261469960333,
					26.16972725545645
				],
				[
					14.425261469960333,
					26.23355781116402
				],
				[
					14.425261469960333,
					26.488874190310753
				],
				[
					14.297612045912501,
					26.74418472577389
				],
				[
					14.106126222472994,
					26.935670549213057
				],
				[
					13.786979287619033,
					27.19098692835979
				],
				[
					13.276346529325565,
					27.446303307506525
				],
				[
					12.893374882447006,
					27.510128019530498
				],
				[
					12.446578523544758,
					27.573958575238066
				],
				[
					11.999782164642511,
					27.573958575238066
				],
				[
					11.616810517763952,
					27.573958575238066
				],
				[
					11.4253246943249,
					27.510128019530498
				],
				[
					11.233838870885847,
					27.382472751798957
				],
				[
					11.170002471494627,
					27.25481748406736
				],
				[
					11.106177759470484,
					27.063331660628194
				],
				[
					11.042353047446795,
					26.80801528148146
				],
				[
					10.978516648055574,
					26.552698902334726
				],
				[
					10.978516648055574,
					26.36121307889556
				],
				[
					11.042353047446795,
					26.297388366871587
				],
				[
					11.106177759470484,
					26.16972725545645
				],
				[
					11.170002471494627,
					26.10590254343242
				],
				[
					11.233838870885847,
					26.10590254343242
				],
				[
					11.29766358290999,
					26.10590254343242
				],
				[
					11.4253246943249,
					26.10590254343242
				],
				[
					11.489149406349043,
					26.10590254343242
				],
				[
					11.552974118373186,
					26.10590254343242
				],
				[
					11.552974118373186,
					26.042071987724853
				],
				[
					11.552974118373186,
					25.850586164285687
				],
				[
					11.361488294933679,
					25.53144507311498
				],
				[
					11.170002471494627,
					25.14847342623665
				],
				[
					10.978516648055574,
					24.70167122365075
				],
				[
					10.787030824616522,
					24.254869021064906
				],
				[
					10.531720289153327,
					23.680411550747465
				],
				[
					10.212573354298911,
					23.042129368405995
				],
				[
					10.08492393025108,
					22.659157721527663
				],
				[
					9.957262818835716,
					22.34001078667336
				],
				[
					9.829601707420807,
					22.084700251210222
				],
				[
					9.765776995396664,
					21.829383872063488
				],
				[
					9.765776995396664,
					21.70172860433189
				],
				[
					9.6381158839813,
					21.510242780892725
				],
				[
					9.574291171957611,
					21.446412225185156
				],
				[
					9.574291171957611,
					21.382581669477588
				],
				[
					9.510466459933468,
					21.382581669477588
				],
				[
					9.446630060542248,
					21.382581669477588
				],
				[
					9.318980636494416,
					21.318756957453616
				],
				[
					9.255144237103195,
					21.25492640174599
				],
				[
					9.127494813055364,
					21.12727113401445
				],
				[
					8.99983370164,
					21.06344057830688
				],
				[
					8.872172590224636,
					20.871954754867716
				],
				[
					8.744523166176805,
					20.68046893142855
				],
				[
					8.616862054761896,
					20.361327840257843
				],
				[
					8.3615515192987,
					19.97835619337951
				],
				[
					8.170065695859194,
					19.53155399079361
				],
				[
					7.914743473028921,
					19.084751788207768
				],
				[
					7.659432937565725,
					18.574124873597896
				],
				[
					7.467947114126673,
					18.127322671011996
				],
				[
					7.212636578663478,
					17.616695756402123
				],
				[
					7.021150755224426,
					17.29755466523136
				],
				[
					6.8296649317853735,
					16.978407730377057
				],
				[
					6.765828532394153,
					16.78692190693795
				],
				[
					6.5743427089551005,
					16.467780815767185
				],
				[
					6.5105179969309575,
					16.340125548035587
				],
				[
					6.446693284906814,
					16.084809168888853
				],
				[
					6.382856885516048,
					16.084809168888853
				],
				[
					6.382856885516048,
					16.084809168888853
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 249,
			"versionNonce": 1550433776,
			"isDeleted": false,
			"id": "IzpqcCFpTiqmjEiSlbdzQ",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3792.4536850379627,
			"y": -570.6027029315661,
			"strokeColor": "#ced4da",
			"backgroundColor": "transparent",
			"width": 37.2120861465869,
			"height": 8.106235140151966,
			"seed": 1728527120,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690849,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.06383639939122077,
					-0.0638247120240294
				],
				[
					0.19148582343905218,
					-0.19148582343916587
				],
				[
					0.25532222283027295,
					-0.19148582343916587
				],
				[
					0.3829716468785591,
					-0.25531053546319527
				],
				[
					0.44680804626932513,
					-0.3191410911707635
				],
				[
					0.5106327582934682,
					-0.4467963589023043
				],
				[
					0.6382938697088321,
					-0.5106269146098725
				],
				[
					0.8297796931478842,
					-0.5744574703174976
				],
				[
					0.9574291171957157,
					-0.5744574703174976
				],
				[
					1.1489149406347678,
					-0.7021127380490384
				],
				[
					1.3404007640742748,
					-0.7659432937566066
				],
				[
					1.5957229869045477,
					-0.8935985614882043
				],
				[
					1.9148582343914313,
					-0.9574291171957725
				],
				[
					2.1701804572217043,
					-1.021253829219745
				],
				[
					2.4254909926848995,
					-1.1489149406349384
				],
				[
					2.8084626395634587,
					-1.2765702083664792
				],
				[
					3.191434286441563,
					-1.4042254760980768
				],
				[
					3.574405933320122,
					-1.5318865875132133
				],
				[
					4.02120229222237,
					-1.659541855244811
				],
				[
					4.531835050515838,
					-1.7233724109523791
				],
				[
					5.042467808809306,
					-1.8510276786839768
				],
				[
					5.6169252791264626,
					-2.0425135021231426
				],
				[
					6.127546350052853,
					-2.1701687698546834
				],
				[
					6.638179108346321,
					-2.2978298812698768
				],
				[
					7.1488118666397895,
					-2.3616545932938493
				],
				[
					7.65943293756618,
					-2.553140416733015
				],
				[
					8.042404584444284,
					-2.6169709724405834
				],
				[
					8.553037342737753,
					-2.744626240172124
				],
				[
					8.936008989616312,
					-2.744626240172124
				],
				[
					9.255155924470728,
					-2.8722873515873175
				],
				[
					9.638127571348832,
					-2.93611206361129
				],
				[
					9.95726281883617,
					-2.9999426193188583
				],
				[
					10.404070865105496,
					-2.9999426193188583
				],
				[
					10.850867224007743,
					-2.9999426193188583
				],
				[
					11.29766358290999,
					-2.9999426193188583
				],
				[
					11.808296341203459,
					-2.9999426193188583
				],
				[
					12.38275381152107,
					-2.9999426193188583
				],
				[
					13.08487239325359,
					-2.9999426193188583
				],
				[
					13.786979287619033,
					-2.93611206361129
				],
				[
					14.489097869351554,
					-2.8722873515873175
				],
				[
					15.255041163108217,
					-2.8084567958797493
				],
				[
					15.893323345449971,
					-2.744626240172124
				],
				[
					16.65926663920618,
					-2.6169709724405834
				],
				[
					17.361385220939155,
					-2.553140416733015
				],
				[
					17.999667403280455,
					-2.553140416733015
				],
				[
					18.510300161573923,
					-2.553140416733015
				],
				[
					19.084757631891534,
					-2.4893157047089858
				],
				[
					19.65921510220869,
					-2.4254851490014175
				],
				[
					20.233672572526302,
					-2.2978298812698768
				],
				[
					20.74430533081977,
					-2.1701687698546834
				],
				[
					21.510248624576434,
					-2.0425135021231426
				],
				[
					22.084706094894045,
					-1.9786829464155744
				],
				[
					22.722988277235345,
					-1.8510276786839768
				],
				[
					23.297445747552956,
					-1.7233724109523791
				],
				[
					23.935727929894256,
					-1.5957112995372427
				],
				[
					24.446360688187724,
					-1.468056031805645
				],
				[
					24.956993446481192,
					-1.4042254760980768
				],
				[
					25.467614517407583,
					-1.2765702083664792
				],
				[
					25.786761452261544,
					-1.1489149406349384
				],
				[
					26.169733099140103,
					-1.0850843849273701
				],
				[
					26.552704746018208,
					-0.9574291171957725
				],
				[
					26.935676392896767,
					-0.7659432937566066
				],
				[
					27.382472751799014,
					-0.6382821823414702
				],
				[
					27.893105510092482,
					-0.4467963589023043
				],
				[
					28.33990186899473,
					-0.19148582343916587
				],
				[
					28.91435933931234,
					0
				],
				[
					29.55265320902072,
					0.2553163791467341
				],
				[
					30.12711067933833,
					0.5106327582934682
				],
				[
					30.76539286167963,
					0.7659432937566066
				],
				[
					31.276025619973097,
					0.9574291171957725
				],
				[
					31.722821978875345,
					1.085090228610909
				],
				[
					32.16961833777805,
					1.2765760520500748
				],
				[
					32.3611041612171,
					1.4042313197816156
				],
				[
					32.61642638404737,
					1.4680618754891839
				],
				[
					32.744075808095204,
					1.5318865875132133
				],
				[
					32.807912207486424,
					1.5318865875132133
				],
				[
					32.935561631534256,
					1.5957171432207815
				],
				[
					32.99939803092548,
					1.6595476989283497
				],
				[
					33.19088385436453,
					1.7872029666599474
				],
				[
					33.382369677804036,
					1.914858234391545
				],
				[
					33.76534132468214,
					2.170180457221818
				],
				[
					34.21213768358439,
					2.361666280660984
				],
				[
					34.722770441877856,
					2.7446379275393156
				],
				[
					35.233391512804246,
					2.999948463002454
				],
				[
					35.68019955907357,
					3.3190953978567563
				],
				[
					36.06317120595213,
					3.510581221295922
				],
				[
					36.25465702939118,
					3.638230645343924
				],
				[
					36.446142852830235,
					3.7658917567590606
				],
				[
					36.50996756485438,
					3.7658917567590606
				],
				[
					36.50996756485438,
					3.82971646878309
				],
				[
					36.50996756485438,
					3.893552868174197
				],
				[
					36.50996756485438,
					4.021202292222199
				],
				[
					36.57379227687852,
					4.148863403637392
				],
				[
					36.70145338829343,
					4.212688115661365
				],
				[
					36.76527810031757,
					4.404173939100531
				],
				[
					36.89293921173248,
					4.468010338491695
				],
				[
					36.89293921173248,
					4.659496161930804
				],
				[
					37.020600323147846,
					4.787145585978806
				],
				[
					37.08442503517199,
					4.85098198536997
				],
				[
					37.14824974719568,
					4.9786314094179716
				],
				[
					37.2120861465869,
					5.0424678088091355
				],
				[
					37.2120861465869,
					5.106292520833108
				],
				[
					37.2120861465869,
					4.9786314094179716
				],
				[
					37.14824974719568,
					4.85098198536997
				],
				[
					37.08442503517199,
					4.659496161930804
				],
				[
					36.956763923756625,
					4.531835050515667
				],
				[
					36.829114499708794,
					4.276524515052529
				],
				[
					36.63762867626929,
					4.085038691613363
				],
				[
					36.50996756485438,
					3.893552868174197
				],
				[
					36.318481741415326,
					3.7658917567590606
				],
				[
					36.19082062999996,
					3.510581221295922
				],
				[
					35.87168538251308,
					3.3190953978567563
				],
				[
					35.616363159682805,
					3.0637731750264265
				],
				[
					35.233391512804246,
					2.8722873515872607
				],
				[
					34.85041986592614,
					2.6169768161241223
				],
				[
					34.46744821904758,
					2.29782988126982
				],
				[
					34.08447657216948,
					2.170180457221818
				],
				[
					33.70150492529092,
					1.914858234391545
				],
				[
					33.25470856638867,
					1.7233724109523791
				],
				[
					32.807912207486424,
					1.5318865875132133
				],
				[
					32.42494056060832,
					1.4042313197816156
				],
				[
					31.914307802314852,
					1.1489149406348815
				],
				[
					31.531336155436293,
					1.0212596729033407
				],
				[
					31.020703397142825,
					0.8936044051717431
				],
				[
					30.510082326216434,
					0.638288026025009
				],
				[
					30.12711067933833,
					0.5744574703174408
				],
				[
					29.74413903245977,
					0.4468022025859
				],
				[
					29.297330986190445,
					0.31914693485430234
				],
				[
					28.91435933931234,
					0.2553163791467341
				],
				[
					28.531387692433782,
					0.19148582343916587
				],
				[
					28.148416045555678,
					0.12766111141513647
				],
				[
					27.76544439867712,
					0.06383055570756824
				],
				[
					27.31864803977487,
					-0.0638247120240294
				],
				[
					26.935676392896767,
					-0.12765526773159763
				],
				[
					26.4250436346033,
					-0.19148582343916587
				],
				[
					26.04207198772474,
					-0.19148582343916587
				],
				[
					25.467614517407583,
					-0.3191410911707635
				],
				[
					25.020818158505335,
					-0.4467963589023043
				],
				[
					24.446360688187724,
					-0.5106269146098725
				],
				[
					23.871903217870113,
					-0.6382821823414702
				],
				[
					23.425106858967865,
					-0.7021127380490384
				],
				[
					22.914474100674397,
					-0.829768005780636
				],
				[
					22.40384134238093,
					-0.8935985614882043
				],
				[
					22.020869695502824,
					-1.021253829219745
				],
				[
					21.574073336600577,
					-1.1489149406349384
				],
				[
					21.25492640174616,
					-1.1489149406349384
				],
				[
					20.871954754867602,
					-1.212739652658911
				],
				[
					20.488983107989498,
					-1.3404007640740474
				],
				[
					20.10601146111094,
					-1.3404007640740474
				],
				[
					19.723039814232834,
					-1.4042254760980768
				],
				[
					19.34006816735473,
					-1.468056031805645
				],
				[
					18.893271808452027,
					-1.468056031805645
				],
				[
					18.38263905015856,
					-1.5318865875132133
				],
				[
					17.872017979232623,
					-1.5957112995372427
				],
				[
					17.361385220939155,
					-1.5957112995372427
				],
				[
					16.850752462645687,
					-1.659541855244811
				],
				[
					16.340131391719297,
					-1.7233724109523791
				],
				[
					15.893323345449971,
					-1.7871971229764085
				],
				[
					15.44652698654727,
					-1.8510276786839768
				],
				[
					14.999730627645022,
					-1.914858234391545
				],
				[
					14.68058369279106,
					-1.9786829464155744
				],
				[
					14.361436757936644,
					-1.9786829464155744
				],
				[
					14.169950934497592,
					-2.0425135021231426
				],
				[
					13.914640399034397,
					-2.0425135021231426
				],
				[
					13.72315457559489,
					-2.0425135021231426
				],
				[
					13.46784404013215,
					-2.0425135021231426
				],
				[
					13.148697105277733,
					-2.0425135021231426
				],
				[
					12.765725458399174,
					-2.0425135021231426
				],
				[
					12.38275381152107,
					-2.0425135021231426
				],
				[
					11.999782164642511,
					-2.0425135021231426
				],
				[
					11.68063522978855,
					-2.0425135021231426
				],
				[
					11.233838870886302,
					-2.0425135021231426
				],
				[
					10.850867224007743,
					-2.0425135021231426
				],
				[
					10.467895577129639,
					-2.0425135021231426
				],
				[
					10.148748642275223,
					-2.0425135021231426
				],
				[
					9.829613394787884,
					-2.0425135021231426
				],
				[
					9.574291171957611,
					-2.0425135021231426
				],
				[
					9.255155924470728,
					-2.0425135021231426
				],
				[
					9.06367010103122,
					-1.9786829464155744
				],
				[
					8.808347878200948,
					-1.914858234391545
				],
				[
					8.616862054761896,
					-1.914858234391545
				],
				[
					8.3615515192987,
					-1.8510276786839768
				],
				[
					8.042404584444284,
					-1.7871971229764085
				],
				[
					7.787094048981544,
					-1.7233724109523791
				],
				[
					7.531783513518349,
					-1.7233724109523791
				],
				[
					7.1488118666397895,
					-1.5957112995372427
				],
				[
					6.893489643809517,
					-1.5318865875132133
				],
				[
					6.574354396322633,
					-1.468056031805645
				],
				[
					6.382868572883126,
					-1.3404007640740474
				],
				[
					6.127546350052853,
					-1.3404007640740474
				],
				[
					5.936060526613801,
					-1.2765702083664792
				],
				[
					5.680749991150606,
					-1.212739652658911
				],
				[
					5.42543945568741,
					-1.0850843849273701
				],
				[
					5.297778344272501,
					-1.021253829219745
				],
				[
					4.978631409418085,
					-1.021253829219745
				],
				[
					4.787145585979033,
					-0.9574291171957725
				],
				[
					4.595659762539526,
					-0.9574291171957725
				],
				[
					4.340349227076786,
					-0.8935985614882043
				],
				[
					4.212688115661422,
					-0.8935985614882043
				],
				[
					4.02120229222237,
					-0.829768005780636
				],
				[
					3.8297164687833174,
					-0.7659432937566066
				],
				[
					3.7658917567591743,
					-0.7659432937566066
				],
				[
					3.7020670447350312,
					-0.7021127380490384
				],
				[
					3.574405933320122,
					-0.6382821823414702
				],
				[
					3.510581221295979,
					-0.6382821823414702
				],
				[
					3.4467448219047583,
					-0.5744574703174976
				],
				[
					3.382920109880615,
					-0.5744574703174976
				],
				[
					3.319095397856927,
					-0.5744574703174976
				],
				[
					3.191434286441563,
					-0.5106269146098725
				],
				[
					3.063773175026654,
					-0.5106269146098725
				],
				[
					2.9361237509783678,
					-0.4467963589023043
				],
				[
					2.7446379275393156,
					-0.38297164687833174
				],
				[
					2.5531521041002634,
					-0.38297164687833174
				],
				[
					2.2978298812699904,
					-0.25531053546319527
				],
				[
					2.1063440578309383,
					-0.25531053546319527
				],
				[
					1.978694633782652,
					-0.19148582343916587
				],
				[
					1.9148582343914313,
					-0.19148582343916587
				],
				[
					1.851033522367743,
					-0.19148582343916587
				],
				[
					1.7872088103436,
					-0.19148582343916587
				],
				[
					1.7233724109523791,
					-0.19148582343916587
				],
				[
					1.659547698928236,
					-0.0638247120240294
				],
				[
					1.5957229869045477,
					-0.0638247120240294
				],
				[
					1.531886587513327,
					0
				],
				[
					1.4042371634654955,
					0.06383055570756824
				],
				[
					1.3404007640742748,
					0.12766111141513647
				],
				[
					1.2765760520501317,
					0.12766111141513647
				],
				[
					1.2127513400259886,
					0.12766111141513647
				],
				[
					1.2127513400259886,
					0.19148582343916587
				],
				[
					1.1489149406347678,
					0.2553163791467341
				],
				[
					1.0850902286110795,
					0.31914693485430234
				],
				[
					0.9574291171957157,
					0.31914693485430234
				],
				[
					0.9574291171957157,
					0.4468022025859
				],
				[
					0.8297796931478842,
					0.5106327582934682
				],
				[
					0.7659432937566635,
					0.5744574703174408
				],
				[
					0.7659432937566635,
					0.638288026025009
				],
				[
					0.7021185817325204,
					0.638288026025009
				],
				[
					0.6382938697088321,
					0.638288026025009
				],
				[
					0.6382938697088321,
					0.7021185817326341
				],
				[
					0.5744574703176113,
					0.7021185817326341
				],
				[
					0.5106327582934682,
					0.7659432937566066
				],
				[
					0.5106327582934682,
					0.8297738494641749
				],
				[
					0.44680804626932513,
					0.8297738494641749
				],
				[
					0.3829716468785591,
					0.8297738494641749
				],
				[
					0.3829716468785591,
					0.8297738494641749
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 19,
			"versionNonce": 912031728,
			"isDeleted": false,
			"id": "qYijNVHx3TVQ2hMCp3uFW",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3783.1985408008595,
			"y": -601.8148921521482,
			"strokeColor": "#fcc2d7",
			"backgroundColor": "transparent",
			"width": 1.8510276786837494,
			"height": 1.7233724109523791,
			"seed": 1183668496,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.12765526773137026,
					0.06383055570756824
				],
				[
					0.25531053546319527,
					0.12766111141513647
				],
				[
					0.31914109117042244,
					0.19148582343916587
				],
				[
					0.5744574703171565,
					0.31914693485430234
				],
				[
					0.7659432937566635,
					0.5106327582934682
				],
				[
					0.9574291171957157,
					0.7021185817326341
				],
				[
					1.1489149406347678,
					0.8936044051717431
				],
				[
					1.34040076407382,
					1.0212596729033407
				],
				[
					1.531886587513327,
					1.2765760520500748
				],
				[
					1.6595418552446972,
					1.4042313197816156
				],
				[
					1.7871971229760675,
					1.5318865875132133
				],
				[
					1.8510276786837494,
					1.6595476989283497
				],
				[
					1.8510276786837494,
					1.7233724109523791
				],
				[
					1.8510276786837494,
					1.7233724109523791
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 23,
			"versionNonce": 145162736,
			"isDeleted": false,
			"id": "_vgg7IUwIQoVTgvtHq5Ip",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3790.3473409801322,
			"y": -595.3043741552168,
			"strokeColor": "#fcc2d7",
			"backgroundColor": "transparent",
			"width": 1.8510335223672882,
			"height": 1.6595476989284066,
			"seed": 1268758288,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.06383639939076602,
					0.06383055570756824
				],
				[
					0.19148582343905218,
					0.12766111141519332
				],
				[
					0.3191469348539613,
					0.31914693485430234
				],
				[
					0.5106327582934682,
					0.5106327582934682
				],
				[
					0.7021185817325204,
					0.6382880260250658
				],
				[
					0.8297796931474295,
					0.8297738494642317
				],
				[
					0.8936044051715726,
					0.8936044051718
				],
				[
					1.0212655165869364,
					0.9574291171957725
				],
				[
					1.1489149406347678,
					1.0850902286109658
				],
				[
					1.2127513400259886,
					1.2127454963425066
				],
				[
					1.2765760520501317,
					1.2765760520500748
				],
				[
					1.4680618754891839,
					1.3404007640741042
				],
				[
					1.5318865875128722,
					1.4042313197816725
				],
				[
					1.595722986904093,
					1.4680618754892407
				],
				[
					1.7233724109523791,
					1.5957171432208384
				],
				[
					1.7872088103436,
					1.5957171432208384
				],
				[
					1.8510335223672882,
					1.6595476989284066
				],
				[
					1.8510335223672882,
					1.6595476989284066
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 24,
			"versionNonce": 1917928432,
			"isDeleted": false,
			"id": "hTj9J3MLCKyyW4o0TQw7W",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3796.411062618161,
			"y": -588.1555681322606,
			"strokeColor": "#fcc2d7",
			"backgroundColor": "transparent",
			"width": 2.680801528148095,
			"height": 2.8084567958797493,
			"seed": 2058769680,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.06383055570756824
				],
				[
					0.06382471202414308,
					0.06383055570756824
				],
				[
					0.12766111141536385,
					0.19148582343916587
				],
				[
					0.19148582343905218,
					0.38297164687833174
				],
				[
					0.31914693485441603,
					0.5106269146099294
				],
				[
					0.44679635890224745,
					0.7659432937566635
				],
				[
					0.6382821823412996,
					0.8935985614882043
				],
				[
					0.8297680057808066,
					1.1489149406349384
				],
				[
					1.0850902286110795,
					1.4042313197816725
				],
				[
					1.404225476097963,
					1.659541855244811
				],
				[
					1.59571129953747,
					1.914858234391545
				],
				[
					1.9148582343914313,
					2.106344057830711
				],
				[
					2.1063440578309383,
					2.2978298812698768
				],
				[
					2.2978298812699904,
					2.4893157047090426
				],
				[
					2.4893157047090426,
					2.6169709724405834
				],
				[
					2.5531404167331857,
					2.6808015281481516
				],
				[
					2.6169768161244065,
					2.74463208385572
				],
				[
					2.680801528148095,
					2.8084567958797493
				],
				[
					2.680801528148095,
					2.8084567958797493
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 37,
			"versionNonce": 1902331376,
			"isDeleted": false,
			"id": "L3WN4TtQuLhGY-DORflmK",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3804.9640999608987,
			"y": -579.5387060774987,
			"strokeColor": "#fcc2d7",
			"backgroundColor": "transparent",
			"width": 4.02120229222237,
			"height": 3.3190895541732175,
			"seed": 155792144,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.06382471202414308,
					0
				],
				[
					0.06382471202414308,
					0.06383055570756824
				],
				[
					0.06382471202414308,
					0.12765526773159763
				],
				[
					0.06382471202414308,
					0.19148582343916587
				],
				[
					0.12764942404828616,
					0.3191410911707635
				],
				[
					0.25531053546319527,
					0.38297164687833174
				],
				[
					0.3829716468785591,
					0.5744574703174976
				],
				[
					0.5744574703176113,
					0.7659432937566635
				],
				[
					0.7659432937566635,
					0.8297738494642317
				],
				[
					0.8935927178049496,
					1.0212596729033976
				],
				[
					1.1489149406352226,
					1.1489149406349384
				],
				[
					1.3404007640742748,
					1.3404007640741042
				],
				[
					1.531886587513327,
					1.468056031805645
				],
				[
					1.7233724109523791,
					1.5957171432208384
				],
				[
					1.914858234391886,
					1.7233724109523791
				],
				[
					2.0425076584397175,
					1.8510276786839768
				],
				[
					2.1063440578309383,
					1.8510276786839768
				],
				[
					2.2339934818787697,
					1.9786887900991132
				],
				[
					2.2978298812699904,
					1.9786887900991132
				],
				[
					2.2978298812699904,
					2.0425135021231426
				],
				[
					2.3616545932941335,
					2.106344057830711
				],
				[
					2.4893157047090426,
					2.2339993255623085
				],
				[
					2.616965128757329,
					2.2978298812698768
				],
				[
					2.808450952196381,
					2.4893157047090426
				],
				[
					3.063773175026654,
					2.6169709724405834
				],
				[
					3.1914225990744853,
					2.7446320838557767
				],
				[
					3.4467448219047583,
					2.999942619318915
				],
				[
					3.638230645344265,
					3.0637731750264834
				],
				[
					3.7658800693920966,
					3.191428442758024
				],
				[
					3.957365892831149,
					3.3190895541732175
				],
				[
					4.02120229222237,
					3.3190895541732175
				],
				[
					4.02120229222237,
					3.3190895541732175
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 32,
			"versionNonce": 48564208,
			"isDeleted": false,
			"id": "UqEXJD9CNTp6Tk6qZHkdp",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3814.2192441980023,
			"y": -571.3686462253228,
			"strokeColor": "#fcc2d7",
			"backgroundColor": "transparent",
			"width": 3.4467448219047583,
			"height": 2.6169768161241223,
			"seed": 1037062416,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.06382471202368833,
					0.06383055570756824
				],
				[
					0.1276611114149091,
					0.06383055570756824
				],
				[
					0.25531053546319527,
					0.19148582343910903
				],
				[
					0.38297164687810437,
					0.2553163791467341
				],
				[
					0.44679635890224745,
					0.31914693485430234
				],
				[
					0.5106327582934682,
					0.44680220258584313
				],
				[
					0.5744574703171565,
					0.44680220258584313
				],
				[
					0.7021185817325204,
					0.5744574703174408
				],
				[
					0.8297680057803518,
					0.7659432937566066
				],
				[
					0.9574291171957157,
					0.8297738494641749
				],
				[
					1.212739652658911,
					0.9574291171957725
				],
				[
					1.404225476097963,
					1.1489149406349384
				],
				[
					1.5957112995370153,
					1.3404007640740474
				],
				[
					1.8510335223672882,
					1.5318865875132133
				],
				[
					2.042519345806795,
					1.5957171432207815
				],
				[
					2.2978298812695357,
					1.7233724109523791
				],
				[
					2.553140416732731,
					1.9148582343914882
				],
				[
					2.680801528148095,
					1.9786887900991132
				],
				[
					2.808462639563004,
					2.106344057830654
				],
				[
					2.999948463002511,
					2.2340051692457905
				],
				[
					3.063773175026199,
					2.29782988126982
				],
				[
					3.1275978870503423,
					2.29782988126982
				],
				[
					3.255258998465706,
					2.361660436977388
				],
				[
					3.3190837104893944,
					2.4893157047089858
				],
				[
					3.382920109880615,
					2.553146260416554
				],
				[
					3.4467448219047583,
					2.6169768161241223
				],
				[
					3.4467448219047583,
					2.6169768161241223
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 29,
			"versionNonce": 1121880560,
			"isDeleted": false,
			"id": "-GzZ6Vnu1T7wduKFQ7ZKt",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3824.1126823048144,
			"y": -563.5815521763415,
			"strokeColor": "#fcc2d7",
			"backgroundColor": "transparent",
			"width": 3.8297164687828626,
			"height": 2.6808015281481516,
			"seed": 1338224400,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.12764942404783142,
					0.12766111141513647
				],
				[
					0.25531053546319527,
					0.19148582343916587
				],
				[
					0.3191352474868836,
					0.31914693485430234
				],
				[
					0.5106210709263905,
					0.38297164687833174
				],
				[
					0.6382821823412996,
					0.5106327582934682
				],
				[
					0.7659432937566635,
					0.6382821823414702
				],
				[
					0.9574291171957157,
					0.7659432937566066
				],
				[
					1.021253829219404,
					0.8936044051718
				],
				[
					1.212739652658911,
					0.9574291171957725
				],
				[
					1.404225476097963,
					1.0850902286109658
				],
				[
					1.4680501881221062,
					1.212739652658911
				],
				[
					1.7233724109523791,
					1.3404007640741042
				],
				[
					1.8510218350002106,
					1.4680618754892407
				],
				[
					2.1063440578304835,
					1.5957112995372427
				],
				[
					2.233993481878315,
					1.6595476989284066
				],
				[
					2.425479305317822,
					1.8510335223675156
				],
				[
					2.553140416732731,
					1.9786829464155744
				],
				[
					2.872287351587147,
					2.106344057830711
				],
				[
					3.063773175026199,
					2.2340051692458474
				],
				[
					3.2552589984652514,
					2.4254909926850132
				],
				[
					3.5105695339284466,
					2.553140416733015
				],
				[
					3.765880069391642,
					2.6808015281481516
				],
				[
					3.8297164687828626,
					2.6808015281481516
				],
				[
					3.8297164687828626,
					2.6808015281481516
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 24,
			"versionNonce": 207080432,
			"isDeleted": false,
			"id": "Fib4TdeYT6Kv8CwiCJrq6",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3833.495487653333,
			"y": -556.688062532532,
			"strokeColor": "#fcc2d7",
			"backgroundColor": "transparent",
			"width": 2.1701687698546266,
			"height": 1.7233724109523791,
			"seed": 1201360144,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.12764942404783142,
					0.19148582343916587
				],
				[
					0.3191352474868836,
					0.25531053546319527
				],
				[
					0.5106210709259358,
					0.38297164687833174
				],
				[
					0.6382821823412996,
					0.5106327582934682
				],
				[
					0.8297680057803518,
					0.7021185817326341
				],
				[
					1.021253829219404,
					0.7659432937566635
				],
				[
					1.085078541243547,
					0.8936044051718
				],
				[
					1.212739652658911,
					0.9574291171957725
				],
				[
					1.2765643646825993,
					1.0850902286109658
				],
				[
					1.34040076407382,
					1.0850902286109658
				],
				[
					1.404225476097963,
					1.1489149406349384
				],
				[
					1.4680501881221062,
					1.212739652658911
				],
				[
					1.5318865875128722,
					1.212739652658911
				],
				[
					1.5957112995370153,
					1.2765760520500748
				],
				[
					1.7233724109523791,
					1.4042254760980768
				],
				[
					1.8510218350002106,
					1.4680618754892407
				],
				[
					2.0425076584392627,
					1.6595476989284066
				],
				[
					2.1701687698546266,
					1.7233724109523791
				],
				[
					2.1701687698546266,
					1.7233724109523791
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 12,
			"versionNonce": 425250288,
			"isDeleted": false,
			"id": "ODpxnS7zZQS0bT3ODYWyc",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3844.793151236243,
			"y": -549.0924543069899,
			"strokeColor": "#fcc2d7",
			"backgroundColor": "transparent",
			"width": 0.19148582343905218,
			"height": 0.19148582343916587,
			"seed": 1590635280,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.06382471202368833,
					0.0638247120240294
				],
				[
					0.12764942404783142,
					0.0638247120240294
				],
				[
					0.19148582343905218,
					0.12764942404800195
				],
				[
					0.19148582343905218,
					0.19148582343916587
				],
				[
					0.19148582343905218,
					0.12764942404800195
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
			"type": "line",
			"version": 63,
			"versionNonce": 585732080,
			"isDeleted": false,
			"id": "fxaTkotJLabeiJBzeeTfy",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3759.172134608198,
			"y": -622.8613406959201,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 157.6965433668256,
			"height": 157.6965433668255,
			"seed": 1607944464,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-157.6965433668256,
					-157.6965433668255
				]
			]
		},
		{
			"type": "freedraw",
			"version": 23,
			"versionNonce": 17961456,
			"isDeleted": false,
			"id": "L9A22j0sO1Is_oQ6jL7lm",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3316.7161539406625,
			"y": -699.8777488690292,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.571471515587518,
			"height": 47.834285510630934,
			"seed": 103524112,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.41474821342808355
				],
				[
					0.13826628062406598,
					-0.9677373932581759
				],
				[
					0.41474821342808355,
					-1.797233820114343
				],
				[
					0.6912554604541583,
					-3.0414784603985368
				],
				[
					0.9677627074802331,
					-4.838724937623908
				],
				[
					1.3825109209083166,
					-7.188960594679372
				],
				[
					2.0737410671404177,
					-10.23045171218888
				],
				[
					2.764996527594576,
					-13.963185633041633
				],
				[
					3.594492954450743,
					-17.972414143809317
				],
				[
					4.838737594734766,
					-23.0876463284593
				],
				[
					5.6682340215909335,
					-27.373382086253116
				],
				[
					6.359489482045092,
					-31.520864220533895
				],
				[
					7.188985908901259,
					-36.08309456824276
				],
				[
					7.88021605513336,
					-40.23057670252348
				],
				[
					8.156723302159435,
					-43.686803376350156
				],
				[
					8.43323054918551,
					-46.590040870346684
				],
				[
					8.571471515587518,
					-47.834285510630934
				],
				[
					8.571471515587518,
					-47.834285510630934
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 23,
			"versionNonce": 1255822320,
			"isDeleted": false,
			"id": "W4uxrCrFn_MeMtnjZtzUc",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3316.02492379443,
			"y": -700.0159898354312,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 23.778889131802316,
			"height": 24.193637345230513,
			"seed": 1581532432,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.13824096640200878,
					0.41474821342808355
				],
				[
					0.27648193280401756,
					0.6912428033431297
				],
				[
					0.5529891798300923,
					1.3824856066862594
				],
				[
					0.8294964268561671,
					2.4884892805685013
				],
				[
					1.5207265730882682,
					3.732733920852752
				],
				[
					2.3502229999444353,
					5.253473151052049
				],
				[
					3.594467640228686,
					7.188960594679372
				],
				[
					5.25346049394102,
					9.539208908845808
				],
				[
					7.603708808107285,
					12.165939155816318
				],
				[
					10.368705335701861,
					14.930935683410837
				],
				[
					13.271942829698446,
					17.55766593038129
				],
				[
					16.45166225649905,
					19.907914244547783
				],
				[
					19.354899750495633,
					21.56690709826006
				],
				[
					21.290399851234042,
					22.94939270494632
				],
				[
					22.6728854579203,
					23.64064816540042
				],
				[
					23.50238188477624,
					24.055396378828505
				],
				[
					23.778889131802316,
					24.193637345230513
				],
				[
					23.778889131802316,
					24.193637345230513
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 24,
			"versionNonce": 1984583152,
			"isDeleted": false,
			"id": "JjC5s06FlSszcMmHo5tfT",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3339.3890647128046,
			"y": -676.0988470801157,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.428666131858108,
			"height": 65.1154695082081,
			"seed": 630792976,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.13824096640200878,
					-0.27649458991504616
				],
				[
					0.27650724702607477,
					-0.6912428033431297
				],
				[
					0.5529891798300923,
					-1.3824982637972312
				],
				[
					0.9677373932581759,
					-2.350235657055407
				],
				[
					1.5207518873103254,
					-3.8709875443656756
				],
				[
					2.2119820335424265,
					-6.082969577908102
				],
				[
					3.0414784603985936,
					-9.124460695417667
				],
				[
					4.1474821342808355,
					-12.718940992757325
				],
				[
					5.253485808163077,
					-17.00467675055114
				],
				[
					6.635971414849337,
					-22.39640352511617
				],
				[
					8.294964268561671,
					-28.479373103024272
				],
				[
					9.67744987524793,
					-34.424101714530366
				],
				[
					11.336442728960265,
					-41.61307496632071
				],
				[
					13.410183796100455,
					-48.24904638116993
				],
				[
					16.17518032369503,
					-55.02325876242122
				],
				[
					17.972414143809374,
					-59.03249993029999
				],
				[
					20.322662457975866,
					-63.04172844106773
				],
				[
					21.428666131858108,
					-65.1154695082081
				],
				[
					21.428666131858108,
					-65.1154695082081
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 22,
			"versionNonce": 2020218864,
			"isDeleted": false,
			"id": "cjFC-wcGdncvfoKq06E5b",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3358.19097528347,
			"y": -744.9470505091766,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.290399851233815,
			"height": 15.345683896838864,
			"seed": 715276560,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.41474821342808355,
					-0.4147482134280267
				],
				[
					-0.6912301462321011,
					-0.8294964268561102
				],
				[
					-1.2442446402842506,
					-1.3824982637972312
				],
				[
					-2.3502229999444353,
					-2.2119946906533983
				],
				[
					-3.594467640228686,
					-3.0414911175095085
				],
				[
					-5.115219527539011,
					-4.285735757793759
				],
				[
					-6.7742123812513455,
					-5.52998039807801
				],
				[
					-8.571446201365688,
					-6.635971414849223
				],
				[
					-10.50694630210387,
					-8.15671064504852
				],
				[
					-12.718928335646297,
					-9.677462532358788
				],
				[
					-14.792669402786714,
					-11.336455386071066
				],
				[
					-17.004676750551198,
					-12.857194616270363
				],
				[
					-18.525403323639466,
					-13.824944666639567
				],
				[
					-20.04615521094979,
					-14.654441093495734
				],
				[
					-20.87565163780573,
					-15.069189306923818
				],
				[
					-21.290399851233815,
					-15.345683896838864
				],
				[
					-21.290399851233815,
					-15.345683896838864
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 22,
			"versionNonce": 1698798064,
			"isDeleted": false,
			"id": "lHPUwMsRnUcyjv0tw_XX5",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3333.1678415113834,
			"y": -765.4079665906655,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 42.71906598309192,
			"height": 32.212107023877024,
			"seed": 752328464,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.41474821342808355,
					-0.27649458991504616
				],
				[
					0.5529891798300923,
					-0.5529891798300923
				],
				[
					1.5207518873103254,
					-1.2442446402842506
				],
				[
					3.0414784603985936,
					-2.4884892805684444
				],
				[
					5.115219527539011,
					-4.009228510767741
				],
				[
					8.018457021535369,
					-6.082969577908102
				],
				[
					11.612949975986112,
					-8.294964268561557
				],
				[
					16.036939357293022,
					-10.921694515532067
				],
				[
					21.152158884831806,
					-14.101439256554613
				],
				[
					26.12913744596881,
					-17.41942496397928
				],
				[
					30.55312682727572,
					-20.875657966361416
				],
				[
					34.83884992795856,
					-23.917142755315467
				],
				[
					38.018594668980995,
					-26.820380249311995
				],
				[
					40.5070839495495,
					-29.447123153393477
				],
				[
					42.16607680326183,
					-31.244363302063334
				],
				[
					42.71906598309192,
					-32.212107023877024
				],
				[
					42.71906598309192,
					-32.212107023877024
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 24,
			"versionNonce": 265870320,
			"isDeleted": false,
			"id": "YeDYuewHrByPLg_Qmnb4r",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3378.2371558086415,
			"y": -801.6293084538657,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 68.01870700220456,
			"height": 26.95864020138052,
			"seed": 1018248464,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.27648193280401756,
					0
				],
				[
					0.6912301462321011,
					0.27650091847053204
				],
				[
					1.797233820114343,
					1.1059973453266991
				],
				[
					3.8709748872545333,
					2.488489280568473
				],
				[
					7.050719628277193,
					4.562230347708834
				],
				[
					11.88943190879013,
					6.912472333319812
				],
				[
					17.6959068967833,
					9.400961613888256
				],
				[
					24.33187831163241,
					12.442446402842307
				],
				[
					31.659105186935903,
					15.483931191796415
				],
				[
					38.98633206223917,
					17.97242047236486
				],
				[
					45.48403719646444,
					20.184415163018258
				],
				[
					51.567019431483686,
					21.981655311688115
				],
				[
					56.68223895902247,
					23.50240087044287
				],
				[
					60.829721093303306,
					24.74664551072712
				],
				[
					63.87122486792373,
					25.714395561096268
				],
				[
					66.35971414849223,
					26.405638364439397
				],
				[
					67.46569250815242,
					26.95864020138052
				],
				[
					68.01870700220456,
					26.95864020138052
				],
				[
					68.01870700220456,
					26.95864020138052
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 26,
			"versionNonce": 708304368,
			"isDeleted": false,
			"id": "Fvme0xxQh_ulQgoLy7cE6",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3358.052734317068,
			"y": -740.9378219984088,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 95.25384812205584,
			"height": 30.691367793677728,
			"seed": 463936272,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5529891798300923,
					-0.27649458991504616
				],
				[
					1.1060036738822419,
					-0.41474821342808355
				],
				[
					2.3502483141664925,
					-1.1059910167712133
				],
				[
					4.285723100682844,
					-2.2119820335424265
				],
				[
					7.327226875303495,
					-3.3179857074246684
				],
				[
					10.506946302104097,
					-4.147482134280779
				],
				[
					15.760432110266947,
					-5.668221364480075
				],
				[
					22.11989627809021,
					-7.188960594679372
				],
				[
					29.86187136682156,
					-9.262701661819733
				],
				[
					38.433342882409306,
					-11.198201762558142
				],
				[
					47.696044544228926,
					-13.686691043126586
				],
				[
					57.09701248667261,
					-16.31342129009704
				],
				[
					66.22147318209045,
					-18.94016419417858
				],
				[
					74.51643745065189,
					-21.843401688175106
				],
				[
					81.84363901173333,
					-24.055396378828505
				],
				[
					87.37363206692226,
					-26.40563203588397
				],
				[
					91.106365987775,
					-27.926371266083265
				],
				[
					93.59485526834351,
					-29.447123153393534
				],
				[
					95.11558184143178,
					-30.41486054665171
				],
				[
					95.25384812205584,
					-30.691367793677728
				],
				[
					95.25384812205584,
					-30.691367793677728
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 20,
			"versionNonce": 1701224432,
			"isDeleted": false,
			"id": "7nKhveGAiRLzgdzm_oQHN",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3362.2002164513488,
			"y": -744.2558077058335,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 30.829608760079736,
			"height": 29.30886952988044,
			"seed": 472987920,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.27650724702607477,
					-0.5529891798300923
				],
				[
					0.6912554604541583,
					-1.2442446402841938
				],
				[
					1.797233820114343,
					-2.626730246970453
				],
				[
					3.594492954450743,
					-4.423976724195768
				],
				[
					6.082982235019244,
					-6.635971414849223
				],
				[
					8.986219729015602,
					-8.98620707190463
				],
				[
					12.30420543644027,
					-11.751190942388178
				],
				[
					15.345683896838864,
					-14.101439256554613
				],
				[
					19.07841781769139,
					-17.14291771695315
				],
				[
					22.258162558714048,
					-19.90791424454767
				],
				[
					25.023133772086567,
					-22.53464449151818
				],
				[
					27.37338208625306,
					-25.023133772086624
				],
				[
					29.447123153393477,
					-27.37338208625306
				],
				[
					30.829608760079736,
					-29.30886952988044
				],
				[
					30.829608760079736,
					-29.30886952988044
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 21,
			"versionNonce": 292364784,
			"isDeleted": false,
			"id": "BaDFbFRo2EtrHu9xmAP6q",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3398.5598182666176,
			"y": -773.5646772357139,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 57.6500016665027,
			"height": 7.6037214652184275,
			"seed": 29857552,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					2.211982033542199,
					0.5530018369411209
				],
				[
					3.0414784603983662,
					0.6912428033431297
				],
				[
					6.08295692079696,
					1.2442446402842506
				],
				[
					9.815690841649712,
					2.0737410671404177
				],
				[
					14.377921189358403,
					3.179732083911574
				],
				[
					19.07841781769139,
					4.009228510767741
				],
				[
					24.33187831163241,
					4.838724937623908
				],
				[
					30.00011233322357,
					5.668221364480075
				],
				[
					35.25359814138642,
					6.359476824934177
				],
				[
					40.645324915951505,
					6.77422503836226
				],
				[
					45.2075552636602,
					7.327214218192353
				],
				[
					49.63151933074505,
					7.46546784170539
				],
				[
					53.22601228519579,
					7.6037214652184275
				],
				[
					56.12924977919238,
					7.6037214652184275
				],
				[
					57.6500016665027,
					7.6037214652184275
				],
				[
					57.6500016665027,
					7.6037214652184275
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 27,
			"versionNonce": 1028875248,
			"isDeleted": false,
			"id": "mHaNJiJdWgKN7QmaVvPgD",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3454.68906804581,
			"y": -767.0669594443779,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.6589928537123342,
			"height": 66.08321955857735,
			"seed": 1625437456,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.1060036738822419
				],
				[
					0,
					1.382498263797288
				],
				[
					0,
					2.6267429040815387
				],
				[
					0,
					4.285735757793816
				],
				[
					-0.13824096640200878,
					6.497730448447214
				],
				[
					-0.13824096640200878,
					9.539208908845808
				],
				[
					-0.13824096640200878,
					13.271942829698503
				],
				[
					-0.13824096640200878,
					17.41942496397928
				],
				[
					-0.13824096640200878,
					22.119908935201124
				],
				[
					-0.27650724702607477,
					27.64988933327919
				],
				[
					-0.27650724702607477,
					32.765108860818145
				],
				[
					-0.5529891798300923,
					39.12458568575232
				],
				[
					-0.6912554604541583,
					44.7928070502324
				],
				[
					-0.9677373932581759,
					50.18453382479743
				],
				[
					-1.3824856066862594,
					54.74676417250623
				],
				[
					-1.6589928537123342,
					58.34125712695692
				],
				[
					-1.6589928537123342,
					61.382735587355455
				],
				[
					-1.6589928537123342,
					63.318235688093864
				],
				[
					-1.6589928537123342,
					64.70072129478012
				],
				[
					-1.6589928537123342,
					65.53021772163629
				],
				[
					-1.6589928537123342,
					66.08321955857735
				],
				[
					-1.6589928537123342,
					66.08321955857735
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 35,
			"versionNonce": 1461806576,
			"isDeleted": false,
			"id": "xsYlXTy-ELOgkAV6LOrNk",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3339.2508237464026,
			"y": -674.1633596364885,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 127.88069070224992,
			"height": 33.8710998775893,
			"seed": 2130252560,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.13824096640200878,
					0
				],
				[
					0.5529891798300923,
					-0.27649458991504616
				],
				[
					1.5207265730882682,
					-0.5529891798300923
				],
				[
					2.903237493996585,
					-1.1059910167712133
				],
				[
					4.562230347708919,
					-1.6589928537123342
				],
				[
					7.05071962827742,
					-2.4884892805684444
				],
				[
					10.230439055078023,
					-3.5944802973396577
				],
				[
					14.37792118935863,
					-4.700471314110814
				],
				[
					19.4931660311197,
					-6.082969577908102
				],
				[
					25.85263019894296,
					-7.46546784170539
				],
				[
					32.903349827220154,
					-9.124460695417724
				],
				[
					41.47482134280767,
					-10.92169451553201
				],
				[
					50.18453382479743,
					-12.718940992757325
				],
				[
					59.1707282395912,
					-14.516187469982697
				],
				[
					68.43345521563288,
					-16.589928537123114
				],
				[
					76.31367127076624,
					-18.525415980750438
				],
				[
					86.26762839304024,
					-21.013905261318882
				],
				[
					94.00957816754953,
					-23.0876463284593
				],
				[
					99.8160531555427,
					-24.884892805684615
				],
				[
					106.03727635696373,
					-26.820380249311995
				],
				[
					111.42900313152882,
					-28.341119479511235
				],
				[
					115.85299251283573,
					-29.86187136682156
				],
				[
					119.3092191866624,
					-30.967862383592774
				],
				[
					122.35072296128283,
					-31.79735881044894
				],
				[
					124.70094596122726,
					-32.62685523730511
				],
				[
					126.22169784853759,
					-33.04160345073319
				],
				[
					127.18943524179576,
					-33.45635166416122
				],
				[
					127.74244973584791,
					-33.8710998775893
				],
				[
					127.88069070224992,
					-33.8710998775893
				],
				[
					127.88069070224992,
					-33.8710998775893
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "text",
			"version": 167,
			"versionNonce": 1272915952,
			"isDeleted": false,
			"id": "WNIfwc9w",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 6.068278342152057,
			"x": 3368.679276218987,
			"y": -732.7090194646656,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 70.48828125,
			"height": 19.261429927591923,
			"seed": 847524112,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"fontSize": 8.025595803163302,
			"fontFamily": 3,
			"text": "Microcontroller\nHome",
			"rawText": "Microcontroller\nHome",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Microcontroller\nHome",
			"lineHeight": 1.2,
			"baseline": 18
		},
		{
			"type": "line",
			"version": 61,
			"versionNonce": 664054256,
			"isDeleted": false,
			"id": "obWg_AcyAoodgcCMEMZHC",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3599.761975490679,
			"y": -780.5334455192877,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 142.39427155279827,
			"height": 38.15443006939029,
			"seed": 1123782416,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-142.39427155279827,
					38.15443006939029
				]
			]
		},
		{
			"type": "line",
			"version": 121,
			"versionNonce": 894036976,
			"isDeleted": false,
			"id": "RBOxcBpkYnIINpc5WYimA",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3329.9369298509187,
			"y": -719.5596674699005,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 717.4924887823704,
			"height": 192.25153294463246,
			"seed": 1222061328,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-717.4924887823704,
					192.25153294463246
				]
			]
		},
		{
			"type": "line",
			"version": 70,
			"versionNonce": 520547824,
			"isDeleted": false,
			"id": "D_l8BFctFzbGomCcMw3HW",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2768.5899369050985,
			"y": -244.4410386295807,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 161.3488293136984,
			"height": 279.464370113084,
			"seed": 227478288,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-161.3488293136984,
					-279.464370113084
				]
			]
		},
		{
			"type": "freedraw",
			"version": 61,
			"versionNonce": 231976944,
			"isDeleted": false,
			"id": "d1-Pbxc6A-RzyWLLXZpek",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2582.7644933423117,
			"y": -641.5545238556477,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 441.9999999999998,
			"height": 132,
			"seed": 1805330704,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
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
					0
				],
				[
					8,
					0
				],
				[
					18,
					-4
				],
				[
					30,
					-10
				],
				[
					32,
					-12
				],
				[
					42,
					-16
				],
				[
					54,
					-22
				],
				[
					82,
					-32
				],
				[
					90,
					-34
				],
				[
					108,
					-38
				],
				[
					140,
					-46
				],
				[
					154,
					-50
				],
				[
					168,
					-52
				],
				[
					212,
					-60
				],
				[
					214,
					-62
				],
				[
					220,
					-64
				],
				[
					242,
					-68
				],
				[
					244,
					-70
				],
				[
					258,
					-74
				],
				[
					264,
					-76
				],
				[
					266,
					-76
				],
				[
					268,
					-78
				],
				[
					278,
					-80
				],
				[
					280,
					-82
				],
				[
					282,
					-82
				],
				[
					290,
					-82
				],
				[
					292,
					-84
				],
				[
					298,
					-84
				],
				[
					302,
					-84
				],
				[
					316,
					-86
				],
				[
					320,
					-86
				],
				[
					342,
					-90
				],
				[
					356,
					-94
				],
				[
					358,
					-94
				],
				[
					363.9999999999998,
					-94
				],
				[
					369.9999999999998,
					-96
				],
				[
					379.9999999999998,
					-100
				],
				[
					385.9999999999998,
					-102
				],
				[
					387.9999999999998,
					-104
				],
				[
					395.9999999999998,
					-108
				],
				[
					399.9999999999998,
					-110
				],
				[
					403.9999999999998,
					-110
				],
				[
					413.9999999999998,
					-116
				],
				[
					423.9999999999998,
					-120
				],
				[
					423.9999999999998,
					-122
				],
				[
					425.9999999999998,
					-122
				],
				[
					429.9999999999998,
					-124
				],
				[
					431.9999999999998,
					-126
				],
				[
					433.9999999999998,
					-126
				],
				[
					437.9999999999998,
					-130
				],
				[
					439.9999999999998,
					-132
				],
				[
					441.9999999999998,
					-132
				],
				[
					441.9999999999998,
					-132
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 198,
			"versionNonce": 1236808176,
			"isDeleted": false,
			"id": "AGyr1RHl85okhqv1yWxgu",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3399.5836828306265,
			"y": -492.8767026600307,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 29.755333647754014,
			"height": 30.00750531809149,
			"seed": 779323152,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.25219475663880075,
					0
				],
				[
					1.0086866813496727,
					0
				],
				[
					1.5129838494217438,
					0
				],
				[
					2.017327190096239,
					0
				],
				[
					3.025967698843033,
					0
				],
				[
					3.5303110395177555,
					0
				],
				[
					4.034654380192478,
					0
				],
				[
					4.538951548264322,
					0
				],
				[
					5.043294888939272,
					0
				],
				[
					5.5476382296139946,
					0
				],
				[
					5.799786813649916,
					0
				],
				[
					6.051935397686066,
					0
				],
				[
					6.3041301543248665,
					0
				],
				[
					6.556278738360561,
					0
				],
				[
					6.80842732239671,
					0
				],
				[
					7.312770663071433,
					0
				],
				[
					7.564919247107355,
					0
				],
				[
					8.069262587782077,
					0
				],
				[
					8.82575451249295,
					0.2521485840359219
				],
				[
					9.330097853167445,
					0.5043202543732832
				],
				[
					10.086589777878316,
					0.7564919247107582
				],
				[
					10.843081702589188,
					1.2608121790840414
				],
				[
					11.851722211335755,
					1.5129838494214027
				],
				[
					12.356065552010477,
					1.7651324334574383
				],
				[
					13.112557476721122,
					2.0173041037947996
				],
				[
					13.364706060757271,
					2.269475774132161
				],
				[
					13.869049401431994,
					2.773796028505444
				],
				[
					14.373346569503838,
					2.773796028505444
				],
				[
					14.625541326142638,
					3.025967698842919
				],
				[
					14.87768991017856,
					3.5302879532162024
				],
				[
					15.12983849421471,
					4.286779877926961
				],
				[
					15.12983849421471,
					4.538951548264322
				],
				[
					15.634181834889205,
					5.29544347297508
				],
				[
					15.886330418925354,
					5.799763727348363
				],
				[
					16.138525175564155,
					6.5562556520591215
				],
				[
					16.390673759600077,
					7.060575906432518
				],
				[
					16.642822343636,
					8.069239501480524
				],
				[
					16.8950171002748,
					8.825731426191282
				],
				[
					17.14716568431095,
					9.58222335090204
				],
				[
					17.14716568431095,
					10.338715275612685
				],
				[
					17.399314268346643,
					11.095207200323443
				],
				[
					17.399314268346643,
					11.851699125034202
				],
				[
					17.399314268346643,
					12.608191049744846
				],
				[
					17.399314268346643,
					13.112511304118243
				],
				[
					17.399314268346643,
					14.121174899166363
				],
				[
					17.399314268346643,
					14.625495153539646
				],
				[
					17.399314268346643,
					15.634158748587765
				],
				[
					17.399314268346643,
					15.886330418925127
				],
				[
					17.399314268346643,
					17.14714259800928
				],
				[
					17.14716568431095,
					17.39931426834653
				],
				[
					16.8950171002748,
					18.155806193057288
				],
				[
					16.8950171002748,
					18.912298117768046
				],
				[
					16.390673759600077,
					19.416618372141443
				],
				[
					16.390673759600077,
					19.920938626514726
				],
				[
					16.390673759600077,
					20.42528196718945
				],
				[
					15.886330418925354,
					20.929602221562845
				],
				[
					15.634181834889205,
					21.43392247593613
				],
				[
					15.38203325085351,
					21.938265816610965
				],
				[
					15.12983849421471,
					22.442586070984248
				],
				[
					14.87768991017856,
					22.69475774132161
				],
				[
					14.373346569503838,
					23.199077995695006
				],
				[
					13.869049401431994,
					23.451249666032368
				],
				[
					13.616854644793193,
					23.955569920405765
				],
				[
					13.112557476721122,
					24.459890174779048
				],
				[
					12.608214136046627,
					24.71206184511641
				],
				[
					12.356065552010477,
					24.71206184511641
				],
				[
					12.103870795371677,
					25.216382099489806
				],
				[
					11.599573627299833,
					25.468553769827167
				],
				[
					11.095230286624883,
					25.72072544016453
				],
				[
					10.590886945950388,
					25.72072544016453
				],
				[
					10.086589777878316,
					25.97287402420045
				],
				[
					9.330097853167445,
					26.225045694537926
				],
				[
					9.077903096528871,
					26.477217364875287
				],
				[
					8.321411171818,
					26.72936594891121
				],
				[
					7.564919247107355,
					26.72936594891121
				],
				[
					6.80842732239671,
					26.98153761924857
				],
				[
					6.3041301543248665,
					27.233709289586045
				],
				[
					5.799786813649916,
					27.485857873621967
				],
				[
					5.043294888939272,
					27.485857873621967
				],
				[
					4.791146304903123,
					27.73802954395933
				],
				[
					4.286802964228627,
					27.73802954395933
				],
				[
					4.034654380192478,
					27.73802954395933
				],
				[
					3.5303110395177555,
					27.73802954395933
				],
				[
					3.2781624554818336,
					27.73802954395933
				],
				[
					2.2694757741323883,
					27.73802954395933
				],
				[
					1.7651786060605446,
					27.73802954395933
				],
				[
					1.2608352653855945,
					27.73802954395933
				],
				[
					0.25219475663880075,
					27.73802954395933
				],
				[
					-0.2521485840356945,
					27.73802954395933
				],
				[
					-1.0086405087465664,
					27.73802954395933
				],
				[
					-1.765132433457211,
					27.73802954395933
				],
				[
					-2.2694757741319336,
					27.73802954395933
				],
				[
					-2.7737729422037773,
					27.73802954395933
				],
				[
					-3.025967698842578,
					27.73802954395933
				],
				[
					-3.2781162828787274,
					27.73802954395933
				],
				[
					-3.5302648669146492,
					27.485857873621967
				],
				[
					-3.78245962355345,
					27.485857873621967
				],
				[
					-3.78245962355345,
					27.233709289586045
				],
				[
					-4.034608207589372,
					27.233709289586045
				],
				[
					-4.034608207589372,
					26.98153761924857
				],
				[
					-4.286756791625521,
					26.98153761924857
				],
				[
					-5.043248716336166,
					26.477217364875287
				],
				[
					-5.547592057010888,
					26.477217364875287
				],
				[
					-6.051935397685611,
					26.225045694537926
				],
				[
					-7.060575906432405,
					25.468553769827167
				],
				[
					-7.5649192471069,
					24.964233515453884
				],
				[
					-8.321411171817772,
					24.459890174779048
				],
				[
					-8.573559755853694,
					23.955569920405765
				],
				[
					-9.077903096528644,
					23.451249666032368
				],
				[
					-9.330051680564338,
					23.199077995695006
				],
				[
					-9.582200264600488,
					22.946906325357645
				],
				[
					-9.834395021239288,
					22.69475774132161
				],
				[
					-9.834395021239288,
					22.190414400646887
				],
				[
					-9.834395021239288,
					21.686094146273604
				],
				[
					-10.08654360527521,
					21.181773891900207
				],
				[
					-10.338692189311132,
					20.677430551225484
				],
				[
					-10.590886945949933,
					20.173110296852087
				],
				[
					-10.590886945949933,
					19.668790042478804
				],
				[
					-10.843035529986082,
					19.164446701803968
				],
				[
					-11.347378870660577,
					18.660126447430684
				],
				[
					-11.347378870660577,
					17.651462852382565
				],
				[
					-11.347378870660577,
					17.14714259800928
				],
				[
					-11.599527454696727,
					16.390650673298524
				],
				[
					-11.851676038732649,
					16.138479002961162
				],
				[
					-11.851676038732649,
					15.381987078250404
				],
				[
					-12.103870795371222,
					14.625495153539646
				],
				[
					-12.103870795371222,
					14.373346569503724
				],
				[
					-12.103870795371222,
					13.869003228829001
				],
				[
					-12.356019379407371,
					13.364682974455604
				],
				[
					-12.356019379407371,
					13.112511304118243
				],
				[
					-12.356019379407371,
					12.860362720082207
				],
				[
					-12.356019379407371,
					12.356019379407485
				],
				[
					-12.356019379407371,
					11.851699125034202
				],
				[
					-12.356019379407371,
					11.59952745469684
				],
				[
					-12.356019379407371,
					10.843035529986082
				],
				[
					-12.356019379407371,
					10.086543605275324
				],
				[
					-12.356019379407371,
					9.58222335090204
				],
				[
					-12.356019379407371,
					9.077903096528644
				],
				[
					-12.103870795371222,
					8.573559755853921
				],
				[
					-12.103870795371222,
					8.069239501480524
				],
				[
					-12.103870795371222,
					7.312747576769766
				],
				[
					-11.851676038732649,
					7.060575906432518
				],
				[
					-11.599527454696727,
					6.5562556520591215
				],
				[
					-11.599527454696727,
					6.051935397685725
				],
				[
					-11.599527454696727,
					5.799763727348363
				],
				[
					-11.599527454696727,
					5.043271802637605
				],
				[
					-11.347378870660577,
					4.538951548264322
				],
				[
					-11.347378870660577,
					4.286779877926961
				],
				[
					-11.095184114021777,
					4.034608207589599
				],
				[
					-10.843035529986082,
					3.5302879532162024
				],
				[
					-10.843035529986082,
					3.278116282878841
				],
				[
					-10.590886945949933,
					2.773796028505444
				],
				[
					-10.338692189311132,
					2.521624358168083
				],
				[
					-10.338692189311132,
					2.269475774132161
				],
				[
					-10.08654360527521,
					1.7651324334574383
				],
				[
					-10.08654360527521,
					1.5129838494214027
				],
				[
					-10.08654360527521,
					1.2608121790840414
				],
				[
					-9.834395021239288,
					1.00864050874668
				],
				[
					-9.834395021239288,
					0.5043202543732832
				],
				[
					-9.582200264600488,
					0.2521485840359219
				],
				[
					-9.330051680564338,
					0.2521485840359219
				],
				[
					-9.077903096528644,
					0
				],
				[
					-8.825708339889843,
					-0.2521716703373613
				],
				[
					-8.573559755853694,
					-0.5043433406747226
				],
				[
					-8.321411171817772,
					-0.7564919247107582
				],
				[
					-8.069216415178971,
					-0.7564919247107582
				],
				[
					-7.817067831143049,
					-1.0086635950481195
				],
				[
					-7.5649192471069,
					-1.0086635950481195
				],
				[
					-7.312724490468099,
					-1.2608352653854809
				],
				[
					-7.312724490468099,
					-1.5129838494214027
				],
				[
					-7.060575906432405,
					-1.5129838494214027
				],
				[
					-6.8084273223962555,
					-1.5129838494214027
				],
				[
					-6.556232565757455,
					-1.5129838494214027
				],
				[
					-6.304083981721533,
					-1.5129838494214027
				],
				[
					-6.051935397685611,
					-1.5129838494214027
				],
				[
					-5.79974064104681,
					-1.5129838494214027
				],
				[
					-5.547592057010888,
					-1.5129838494214027
				],
				[
					-5.043248716336166,
					-1.5129838494214027
				],
				[
					-4.791100132300016,
					-1.5129838494214027
				],
				[
					-4.286756791625521,
					-1.7651555197588777
				],
				[
					-3.78245962355345,
					-1.7651555197588777
				],
				[
					-3.5302648669146492,
					-1.7651555197588777
				],
				[
					-3.2781162828787274,
					-1.7651555197588777
				],
				[
					-3.025967698842578,
					-1.7651555197588777
				],
				[
					-2.7737729422037773,
					-2.017327190096239
				],
				[
					-2.521624358168083,
					-2.017327190096239
				],
				[
					-2.2694757741319336,
					-2.017327190096239
				],
				[
					-2.017281017493133,
					-2.017327190096239
				],
				[
					-1.765132433457211,
					-2.017327190096239
				],
				[
					-1.2607890927824883,
					-2.269475774132161
				],
				[
					-1.0086405087465664,
					-2.269475774132161
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
			"version": 66,
			"versionNonce": 1505522672,
			"isDeleted": false,
			"id": "5H6HJrw7rkO0P7zyQuMag",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3402.8618452861083,
			"y": -463.12136901227643,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 129.61226770956955,
			"height": 124.56901899323316,
			"seed": 1922049296,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.5043433406747226
				],
				[
					0.5042971680718438,
					1.765155519758764
				],
				[
					1.2607890927824883,
					3.530311039517642
				],
				[
					2.01728101749336,
					6.808427322396483
				],
				[
					2.773772942204232,
					8.825754512492722
				],
				[
					3.7824596235536774,
					11.347378870660805
				],
				[
					4.286756791625521,
					14.121197985467688
				],
				[
					5.043248716336166,
					17.399314268346643
				],
				[
					5.799740641047038,
					20.67745363752681
				],
				[
					6.30408398172176,
					24.459913261080487
				],
				[
					7.060575906432405,
					28.746693139007448
				],
				[
					7.564919247107355,
					33.03349610323585
				],
				[
					8.069216415179199,
					38.581088160246736
				],
				[
					8.825708339889843,
					44.12870330355918
				],
				[
					9.330051680564793,
					50.43281037158238
				],
				[
					10.59088694595016,
					57.99772961868962
				],
				[
					11.347378870660805,
					64.55398527074874
				],
				[
					12.860362720082321,
					73.88406003761474
				],
				[
					14.37334656950361,
					81.95329953909527
				],
				[
					15.886330418925127,
					88.76172686149175
				],
				[
					17.651462852382565,
					96.3266461085991
				],
				[
					19.416595285840003,
					103.13507343099559
				],
				[
					20.67743055122537,
					108.93483715834395
				],
				[
					21.938265816610965,
					113.72596037694564
				],
				[
					22.94690632535776,
					117.5084200004992
				],
				[
					23.451249666032254,
					120.28221602900476
				],
				[
					23.955546834104325,
					121.79519987842627
				],
				[
					24.207741590743126,
					123.05603514381164
				],
				[
					24.459890174779048,
					123.56035539818504
				],
				[
					24.459890174779048,
					124.31684732289568
				],
				[
					24.459890174779048,
					124.56901899323316
				],
				[
					24.712038758815197,
					124.56901899323316
				],
				[
					24.712038758815197,
					124.31684732289568
				],
				[
					25.720725440164642,
					123.8125270685224
				],
				[
					26.477217364875287,
					122.80386347347428
				],
				[
					27.738006457657775,
					121.54305129439024
				],
				[
					29.25099030707952,
					120.28221602900476
				],
				[
					31.520466081211453,
					118.0127402548726
				],
				[
					35.30292570476513,
					115.49111589670451
				],
				[
					40.09407200966825,
					111.96080485718676
				],
				[
					46.39815599139001,
					107.67402497925991
				],
				[
					53.45873189782242,
					103.38724510133284
				],
				[
					62.28448641031514,
					98.59612188273127
				],
				[
					71.11024092280786,
					93.30067840975607
				],
				[
					79.9359492626977,
					88.00523493678111
				],
				[
					89.5181956999013,
					82.45761979346867
				],
				[
					97.83960687171907,
					77.41434799083095
				],
				[
					105.90886945950115,
					72.62322477222926
				],
				[
					112.21295344122291,
					68.58861656463978
				],
				[
					117.25624833016172,
					64.8061569410861
				],
				[
					121.29085653775155,
					61.27584590156846
				],
				[
					124.06467565255844,
					58.75422154340026
				],
				[
					125.57765950197972,
					56.9890660236415
				],
				[
					127.34279193543716,
					54.71959024950934
				],
				[
					128.85577578485868,
					52.70228614571454
				],
				[
					129.1079243688946,
					52.45011447537718
				],
				[
					129.1079243688946,
					52.197942805039816
				],
				[
					129.3601191255334,
					52.197942805039816
				],
				[
					129.3601191255334,
					51.94579422100378
				],
				[
					129.61226770956955,
					51.94579422100378
				],
				[
					129.61226770956955,
					51.94579422100378
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 82,
			"versionNonce": 602437104,
			"isDeleted": false,
			"id": "nfqWDgBP7Z8K30u1an-ir",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.023682179613829568,
			"x": 2834.1512317474658,
			"y": -793.8822941995871,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.9743589743589745,
			"height": 16.564102564102566,
			"seed": 90768144,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.8717948717948719
				],
				[
					0,
					1.7435897435897438
				],
				[
					0,
					2.615384615384616
				],
				[
					0,
					3.4871794871794877
				],
				[
					0.8717948717948718,
					3.4871794871794877
				],
				[
					0.8717948717948718,
					4.3589743589743595
				],
				[
					0.8717948717948718,
					5.230769230769232
				],
				[
					1.7435897435897436,
					5.230769230769232
				],
				[
					1.7435897435897436,
					6.102564102564103
				],
				[
					2.6153846153846154,
					6.974358974358975
				],
				[
					2.6153846153846154,
					7.846153846153848
				],
				[
					2.6153846153846154,
					8.717948717948719
				],
				[
					3.4871794871794872,
					10.461538461538463
				],
				[
					4.3589743589743595,
					12.205128205128206
				],
				[
					6.102564102564102,
					13.94871794871795
				],
				[
					6.102564102564102,
					14.820512820512823
				],
				[
					6.9743589743589745,
					15.692307692307695
				],
				[
					6.9743589743589745,
					16.564102564102566
				],
				[
					6.9743589743589745,
					16.564102564102566
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 80,
			"versionNonce": 222574576,
			"isDeleted": false,
			"id": "mtmr-5zLxfhocoaaZMYBH",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.023682179613829568,
			"x": 2850.813787711125,
			"y": -797.8374868378029,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.846153846153847,
			"height": 16.564102564102566,
			"seed": 1165369616,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.8717948717948719
				],
				[
					0,
					1.7435897435897438
				],
				[
					0,
					2.615384615384616
				],
				[
					0.8717948717948718,
					3.4871794871794877
				],
				[
					0.8717948717948718,
					4.3589743589743595
				],
				[
					1.7435897435897436,
					6.102564102564103
				],
				[
					2.6153846153846154,
					7.846153846153848
				],
				[
					3.4871794871794872,
					9.589743589743591
				],
				[
					4.3589743589743595,
					11.333333333333336
				],
				[
					5.230769230769231,
					12.205128205128206
				],
				[
					5.230769230769231,
					13.076923076923078
				],
				[
					6.102564102564102,
					14.820512820512823
				],
				[
					6.9743589743589745,
					14.820512820512823
				],
				[
					7.846153846153847,
					15.692307692307695
				],
				[
					7.846153846153847,
					16.564102564102566
				],
				[
					7.846153846153847,
					16.564102564102566
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 80,
			"versionNonce": 433568240,
			"isDeleted": false,
			"id": "z29SlJJucsSvn2Woqg9S6",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.023682179613829568,
			"x": 2844.144367212257,
			"y": -764.7882586078734,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.948717948717949,
			"height": 1.7435897435897436,
			"seed": 36667152,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.8717948717948718,
					0
				],
				[
					1.7435897435897436,
					0
				],
				[
					2.6153846153846154,
					0
				],
				[
					3.4871794871794872,
					0
				],
				[
					4.3589743589743595,
					0
				],
				[
					5.230769230769231,
					0
				],
				[
					6.102564102564102,
					0
				],
				[
					6.9743589743589745,
					0
				],
				[
					7.846153846153847,
					0
				],
				[
					8.717948717948719,
					-0.8717948717948718
				],
				[
					9.58974358974359,
					-0.8717948717948718
				],
				[
					10.461538461538462,
					-1.7435897435897436
				],
				[
					11.333333333333334,
					-1.7435897435897436
				],
				[
					12.205128205128204,
					-1.7435897435897436
				],
				[
					13.076923076923077,
					-1.7435897435897436
				],
				[
					13.948717948717949,
					-1.7435897435897436
				],
				[
					13.948717948717949,
					-1.7435897435897436
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 18,
			"versionNonce": 212532208,
			"isDeleted": false,
			"id": "H00oZ-uE8dgCHLU-KfwfF",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3530.961129146256,
			"y": -410.16693428252586,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.799786813649916,
			"height": 7.31274757676988,
			"seed": 1544363280,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.2521485840360356
				],
				[
					0.25214858403614926,
					-0.2521485840360356
				],
				[
					0.7564919247108719,
					-0.7564919247107582
				],
				[
					1.2608352653855945,
					-1.5129838494215164
				],
				[
					1.7651324334574383,
					-2.0173041037949133
				],
				[
					2.521624358168083,
					-3.025967698842919
				],
				[
					3.2781162828787274,
					-3.7824596235536774
				],
				[
					4.034608207589827,
					-4.538951548264436
				],
				[
					4.538951548264322,
					-5.547592057011116
				],
				[
					5.295443472975421,
					-6.30408398172176
				],
				[
					5.799786813649916,
					-7.060575906432518
				],
				[
					5.799786813649916,
					-7.31274757676988
				],
				[
					5.799786813649916,
					-7.31274757676988
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 39,
			"versionNonce": 130416112,
			"isDeleted": false,
			"id": "071c3F4IIpdt5g0htkFCp",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3533.7349482610634,
			"y": -420.2534778878013,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 123.81252706852274,
			"height": 50.180638701245016,
			"seed": 612825872,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.2608352653855945,
					-0.5043433406747226
				],
				[
					-2.521670530771189,
					-1.2608352653854809
				],
				[
					-4.538951548264549,
					-2.269475774132161
				],
				[
					-8.069262587782305,
					-3.7824596235535637
				],
				[
					-11.599573627299833,
					-5.547615143312441
				],
				[
					-16.642822343636,
					-8.069262587781964
				],
				[
					-22.190460573249993,
					-10.590886945950047
				],
				[
					-28.746693139007675,
					-13.112534390419569
				],
				[
					-37.068104310825674,
					-16.39067375959985
				],
				[
					-46.14600740735432,
					-20.173133383153527
				],
				[
					-56.23259718523241,
					-23.70342133636973
				],
				[
					-65.5626488657972,
					-27.23370928958593
				],
				[
					-74.3884033782897,
					-30.511848658766212
				],
				[
					-83.97060364289041,
					-34.042136611982414
				],
				[
					-92.03986623067249,
					-37.06810431082533
				],
				[
					-98.84829355306874,
					-39.84192342563233
				],
				[
					-104.64808036671866,
					-42.11139919976449
				],
				[
					-109.94352383969363,
					-44.38087497389665
				],
				[
					-113.7259834632473,
					-46.14600740735398
				],
				[
					-116.75195116209034,
					-47.1546710024021
				],
				[
					-118.51708359554777,
					-48.163334597450216
				],
				[
					-120.03006744496906,
					-48.6676548518235
				],
				[
					-120.78655936967971,
					-49.171975106196896
				],
				[
					-121.29090271035466,
					-49.171975106196896
				],
				[
					-121.7951998784265,
					-49.42414677653426
				],
				[
					-122.0473946350653,
					-49.42414677653426
				],
				[
					-122.29954321910122,
					-49.42414677653426
				],
				[
					-122.55169180313715,
					-49.42414677653426
				],
				[
					-122.80388655977595,
					-49.67631844687162
				],
				[
					-123.0560351438121,
					-49.67631844687162
				],
				[
					-123.56037848448659,
					-49.928467030907655
				],
				[
					-123.81252706852274,
					-49.928467030907655
				],
				[
					-123.81252706852274,
					-50.180638701245016
				],
				[
					-123.81252706852274,
					-50.180638701245016
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 35,
			"versionNonce": 741392368,
			"isDeleted": false,
			"id": "gJKwpJmErgiYVnqXSVEyr",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3387.227663451219,
			"y": -491.11157022657324,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 101.62206649527275,
			"height": 58.502038329912295,
			"seed": 1041570064,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5043433406747226,
					-0.2521485840360356
				],
				[
					-0.7564919247106445,
					-0.7564919247107582
				],
				[
					-1.2608352653855945,
					-1.260812179084155
				],
				[
					-2.269475774132161,
					-2.269475774132161
				],
				[
					-3.530311039517528,
					-3.278116282878841
				],
				[
					-5.0432948889390445,
					-4.7911001323003575
				],
				[
					-7.3127706630712055,
					-7.060575906432518
				],
				[
					-9.834395021239288,
					-9.33005168056468
				],
				[
					-12.608214136046172,
					-11.851699125034202
				],
				[
					-15.381987078250404,
					-14.121174899166363
				],
				[
					-18.155806193057288,
					-16.894982470822583
				],
				[
					-21.433922475936242,
					-19.164458244954744
				],
				[
					-24.459890174779048,
					-21.433934019086905
				],
				[
					-27.738052630260654,
					-23.703409793219066
				],
				[
					-31.01616891313961,
					-25.72072544016453
				],
				[
					-34.54647995265714,
					-27.73802954395933
				],
				[
					-38.07674481957201,
					-29.755345190904904
				],
				[
					-42.36354778380041,
					-32.024820965037065
				],
				[
					-47.15464791610066,
					-34.294296739169226
				],
				[
					-54.21526999513594,
					-37.57242456519873
				],
				[
					-61.023697317532424,
					-40.59839226404165
				],
				[
					-67.8321246399289,
					-43.37219983569787
				],
				[
					-75.64919247107218,
					-47.154659459251434
				],
				[
					-83.21411171817931,
					-50.43278728528105
				],
				[
					-90.0225390405758,
					-53.710926654461275
				],
				[
					-95.57013109758691,
					-56.232562555780135
				],
				[
					-99.10044213710444,
					-57.745546405201594
				],
				[
					-100.86557457056188,
					-58.2498782027256
				],
				[
					-101.62206649527275,
					-58.502038329912295
				],
				[
					-101.62206649527275,
					-58.502038329912295
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 94,
			"versionNonce": 972243440,
			"isDeleted": false,
			"id": "iDFTCZtKxKJQdv6axQFZu",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.023682179613829568,
			"x": 2844.237265540416,
			"y": -764.7871585390122,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.948717948717949,
			"height": 9.58974358974359,
			"seed": 2083485456,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.8717948717948718
				],
				[
					0,
					-1.7435897435897436
				],
				[
					0,
					-3.4871794871794872
				],
				[
					0,
					-4.3589743589743595
				],
				[
					0,
					-5.230769230769231
				],
				[
					0,
					-6.102564102564102
				],
				[
					0.8717948717948718,
					-6.102564102564102
				],
				[
					0.8717948717948718,
					-6.9743589743589745
				],
				[
					1.7435897435897436,
					-6.9743589743589745
				],
				[
					2.6153846153846154,
					-7.846153846153847
				],
				[
					3.4871794871794872,
					-7.846153846153847
				],
				[
					3.4871794871794872,
					-8.717948717948719
				],
				[
					4.3589743589743595,
					-8.717948717948719
				],
				[
					5.230769230769231,
					-9.58974358974359
				],
				[
					6.102564102564102,
					-9.58974358974359
				],
				[
					6.9743589743589745,
					-9.58974358974359
				],
				[
					7.846153846153847,
					-9.58974358974359
				],
				[
					9.58974358974359,
					-9.58974358974359
				],
				[
					10.461538461538462,
					-9.58974358974359
				],
				[
					11.333333333333334,
					-8.717948717948719
				],
				[
					11.333333333333334,
					-7.846153846153847
				],
				[
					12.205128205128204,
					-6.9743589743589745
				],
				[
					12.205128205128204,
					-6.102564102564102
				],
				[
					13.076923076923077,
					-6.102564102564102
				],
				[
					13.076923076923077,
					-5.230769230769231
				],
				[
					13.076923076923077,
					-4.3589743589743595
				],
				[
					13.948717948717949,
					-4.3589743589743595
				],
				[
					13.948717948717949,
					-3.4871794871794872
				],
				[
					13.948717948717949,
					-2.6153846153846154
				],
				[
					13.948717948717949,
					-1.7435897435897436
				],
				[
					13.948717948717949,
					-1.7435897435897436
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 37,
			"versionNonce": 806716400,
			"isDeleted": false,
			"id": "UKbCe8zJEfFeMOYsgzzw7",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3285.6055969559466,
			"y": -549.6136085564855,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 100.10908264585146,
			"height": 20.677442094376147,
			"seed": 55448848,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.2521601271866416
				],
				[
					0.5042971680720711,
					-0.2521601271866416
				],
				[
					0.7564919247108719,
					-0.5043317975240598
				],
				[
					1.5129838494215164,
					-0.7564919247107014
				],
				[
					2.269475774132161,
					-0.7564919247107014
				],
				[
					3.5302648669148766,
					-1.2608237222347611
				],
				[
					5.043248716336393,
					-1.7651439766081012
				],
				[
					7.312724490468554,
					-2.269475774132161
				],
				[
					10.086543605275438,
					-3.0259676988428623
				],
				[
					14.62549515353976,
					-3.7824596235536205
				],
				[
					20.42528196718945,
					-5.295443472975023
				],
				[
					27.48585787362208,
					-6.304095524872423
				],
				[
					35.55512046140393,
					-7.817079374293883
				],
				[
					43.87653163322193,
					-9.330063223715342
				],
				[
					51.94574804840113,
					-11.095218743474163
				],
				[
					58.75417537079761,
					-12.608202592895566
				],
				[
					66.06694603386882,
					-13.869014771979664
				],
				[
					72.62322477222938,
					-15.381998621401124
				],
				[
					78.67516016991522,
					-16.642822343635885
				],
				[
					84.47490081096225,
					-17.903646065870646
				],
				[
					88.76170377519043,
					-18.660137990581347
				],
				[
					92.5441633987441,
					-19.416629915292106
				],
				[
					95.82227968162283,
					-20.173121840002807
				],
				[
					96.8309663629725,
					-20.173121840002807
				],
				[
					98.09175545575522,
					-20.425281967189505
				],
				[
					98.84824738046586,
					-20.425281967189505
				],
				[
					99.35259072114059,
					-20.425281967189505
				],
				[
					99.35259072114059,
					-20.677442094376147
				],
				[
					99.60473930517651,
					-20.677442094376147
				],
				[
					99.85693406181531,
					-20.677442094376147
				],
				[
					100.10908264585146,
					-20.677442094376147
				],
				[
					100.10908264585146,
					-20.677442094376147
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 40,
			"versionNonce": 1822393840,
			"isDeleted": false,
			"id": "9IKf3Tabg_HL9HhzvhJjf",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3387.4798120352552,
			"y": -570.0388905236749,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.112557476720895,
			"height": 74.64054041917484,
			"seed": 686355216,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.7564919247107582
				],
				[
					0,
					1.260823722234818
				],
				[
					0.2521947566385734,
					2.7738075716562207
				],
				[
					0.5043433406744953,
					4.28679142107768
				],
				[
					0.7564919247106445,
					6.0519353976857815
				],
				[
					1.512983849421289,
					8.57357129900464
				],
				[
					1.7651786060600898,
					11.095218743474163
				],
				[
					2.0173271900960117,
					14.121186442317082
				],
				[
					2.5216705307707343,
					17.399314268346643
				],
				[
					3.025967698842578,
					21.433934019086905
				],
				[
					3.78245962355345,
					25.972885567351227
				],
				[
					4.538951548264322,
					30.76400878595291
				],
				[
					5.295443472974966,
					34.798628536693286
				],
				[
					6.8084273223962555,
					39.33758008495761
				],
				[
					7.817114003745701,
					43.37219983569787
				],
				[
					8.825754512492495,
					47.154659459251434
				],
				[
					9.834395021239288,
					50.68495895561841
				],
				[
					10.590886945949933,
					53.96308678164792
				],
				[
					10.843081702588734,
					56.73689435330414
				],
				[
					11.347378870660577,
					59.258530254623
				],
				[
					11.851722211335527,
					61.78017769909252
				],
				[
					12.103870795371222,
					63.79748180288732
				],
				[
					12.356065552010023,
					66.06695757701948
				],
				[
					12.356065552010023,
					67.83211309677836
				],
				[
					12.608214136046172,
					69.34509694619976
				],
				[
					12.608214136046172,
					70.85808079562116
				],
				[
					12.608214136046172,
					71.61457272033192
				],
				[
					12.860362720082094,
					72.37106464504268
				],
				[
					12.860362720082094,
					73.12755656975332
				],
				[
					12.860362720082094,
					73.3797282400908
				],
				[
					13.112557476720895,
					73.88404849446408
				],
				[
					13.112557476720895,
					74.13622016480144
				],
				[
					13.112557476720895,
					74.38836874883737
				],
				[
					13.112557476720895,
					74.64054041917484
				],
				[
					13.112557476720895,
					74.64054041917484
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 255,
			"versionNonce": 1285113840,
			"isDeleted": false,
			"id": "V_3aVJ4nVvNS3kg1Zba0o",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.023682179613829568,
			"x": 2813.123467701286,
			"y": -801.6058059069297,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 68,
			"height": 67.12820512820512,
			"seed": 1400377616,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.8717948717948717
				],
				[
					0,
					1.7435897435897434
				],
				[
					0,
					2.615384615384615
				],
				[
					0,
					3.487179487179487
				],
				[
					0,
					4.358974358974359
				],
				[
					0,
					5.23076923076923
				],
				[
					0,
					6.102564102564102
				],
				[
					0,
					6.974358974358974
				],
				[
					0.8717948717948718,
					6.974358974358974
				],
				[
					0.8717948717948718,
					7.846153846153845
				],
				[
					0.8717948717948718,
					8.717948717948717
				],
				[
					1.7435897435897436,
					9.58974358974359
				],
				[
					2.6153846153846154,
					10.46153846153846
				],
				[
					2.6153846153846154,
					11.333333333333332
				],
				[
					4.3589743589743595,
					15.69230769230769
				],
				[
					4.3589743589743595,
					16.564102564102562
				],
				[
					4.3589743589743595,
					17.435897435897434
				],
				[
					6.102564102564102,
					20.92307692307692
				],
				[
					6.9743589743589745,
					21.794871794871792
				],
				[
					8.717948717948719,
					26.15384615384615
				],
				[
					8.717948717948719,
					27.025641025641022
				],
				[
					8.717948717948719,
					27.897435897435894
				],
				[
					9.58974358974359,
					31.38461538461538
				],
				[
					10.461538461538462,
					33.99999999999999
				],
				[
					10.461538461538462,
					34.87179487179487
				],
				[
					11.333333333333334,
					37.48717948717948
				],
				[
					11.333333333333334,
					40.102564102564095
				],
				[
					12.205128205128204,
					42.717948717948715
				],
				[
					12.205128205128204,
					43.589743589743584
				],
				[
					13.076923076923077,
					44.46153846153846
				],
				[
					13.076923076923077,
					45.33333333333333
				],
				[
					13.076923076923077,
					46.2051282051282
				],
				[
					13.076923076923077,
					47.07692307692307
				],
				[
					13.076923076923077,
					47.94871794871794
				],
				[
					13.076923076923077,
					48.82051282051282
				],
				[
					13.076923076923077,
					49.692307692307686
				],
				[
					13.948717948717949,
					50.564102564102555
				],
				[
					13.948717948717949,
					51.43589743589743
				],
				[
					13.948717948717949,
					52.3076923076923
				],
				[
					13.948717948717949,
					53.179487179487175
				],
				[
					14.820512820512821,
					53.179487179487175
				],
				[
					15.692307692307693,
					53.179487179487175
				],
				[
					16.564102564102566,
					53.179487179487175
				],
				[
					17.435897435897438,
					53.179487179487175
				],
				[
					17.435897435897438,
					54.051282051282044
				],
				[
					18.307692307692307,
					54.051282051282044
				],
				[
					19.17948717948718,
					54.051282051282044
				],
				[
					20.05128205128205,
					54.051282051282044
				],
				[
					21.794871794871796,
					54.051282051282044
				],
				[
					23.53846153846154,
					54.051282051282044
				],
				[
					24.41025641025641,
					54.051282051282044
				],
				[
					27.897435897435898,
					54.051282051282044
				],
				[
					28.76923076923077,
					54.051282051282044
				],
				[
					29.641025641025642,
					54.051282051282044
				],
				[
					31.384615384615387,
					54.051282051282044
				],
				[
					32.256410256410255,
					54.051282051282044
				],
				[
					34,
					54.051282051282044
				],
				[
					37.48717948717949,
					52.3076923076923
				],
				[
					38.35897435897436,
					52.3076923076923
				],
				[
					39.23076923076923,
					52.3076923076923
				],
				[
					40.1025641025641,
					52.3076923076923
				],
				[
					40.97435897435898,
					51.43589743589743
				],
				[
					41.84615384615385,
					51.43589743589743
				],
				[
					42.717948717948715,
					51.43589743589743
				],
				[
					43.58974358974359,
					50.564102564102555
				],
				[
					44.46153846153846,
					50.564102564102555
				],
				[
					45.333333333333336,
					50.564102564102555
				],
				[
					46.205128205128204,
					50.564102564102555
				],
				[
					46.205128205128204,
					49.692307692307686
				],
				[
					47.94871794871795,
					48.82051282051282
				],
				[
					48.82051282051282,
					47.94871794871794
				],
				[
					49.69230769230769,
					47.94871794871794
				],
				[
					50.56410256410256,
					47.94871794871794
				],
				[
					51.43589743589744,
					47.07692307692307
				],
				[
					52.30769230769231,
					47.07692307692307
				],
				[
					53.17948717948718,
					47.07692307692307
				],
				[
					54.05128205128205,
					46.2051282051282
				],
				[
					54.05128205128205,
					45.33333333333333
				],
				[
					54.92307692307693,
					45.33333333333333
				],
				[
					55.794871794871796,
					44.46153846153846
				],
				[
					56.666666666666664,
					44.46153846153846
				],
				[
					58.41025641025641,
					43.589743589743584
				],
				[
					60.15384615384615,
					41.84615384615384
				],
				[
					61.02564102564103,
					41.84615384615384
				],
				[
					62.769230769230774,
					40.97435897435897
				],
				[
					63.64102564102564,
					40.97435897435897
				],
				[
					63.64102564102564,
					40.102564102564095
				],
				[
					63.64102564102564,
					39.230769230769226
				],
				[
					63.64102564102564,
					38.35897435897436
				],
				[
					63.64102564102564,
					37.48717948717948
				],
				[
					63.64102564102564,
					36.61538461538461
				],
				[
					63.64102564102564,
					35.74358974358974
				],
				[
					63.64102564102564,
					33.99999999999999
				],
				[
					63.64102564102564,
					33.128205128205124
				],
				[
					63.64102564102564,
					32.256410256410255
				],
				[
					63.64102564102564,
					31.38461538461538
				],
				[
					63.64102564102564,
					29.64102564102564
				],
				[
					63.64102564102564,
					28.769230769230766
				],
				[
					63.64102564102564,
					27.897435897435894
				],
				[
					63.64102564102564,
					27.025641025641022
				],
				[
					63.64102564102564,
					26.15384615384615
				],
				[
					63.64102564102564,
					24.41025641025641
				],
				[
					63.64102564102564,
					23.538461538461537
				],
				[
					63.64102564102564,
					22.666666666666664
				],
				[
					63.64102564102564,
					20.92307692307692
				],
				[
					63.64102564102564,
					20.051282051282048
				],
				[
					62.769230769230774,
					20.051282051282048
				],
				[
					62.769230769230774,
					19.17948717948718
				],
				[
					62.769230769230774,
					18.307692307692307
				],
				[
					62.769230769230774,
					17.435897435897434
				],
				[
					62.769230769230774,
					16.564102564102562
				],
				[
					62.769230769230774,
					15.69230769230769
				],
				[
					62.769230769230774,
					14.82051282051282
				],
				[
					62.769230769230774,
					13.948717948717947
				],
				[
					61.8974358974359,
					13.076923076923075
				],
				[
					61.8974358974359,
					11.333333333333332
				],
				[
					61.8974358974359,
					10.46153846153846
				],
				[
					61.8974358974359,
					9.58974358974359
				],
				[
					61.02564102564103,
					9.58974358974359
				],
				[
					61.02564102564103,
					8.717948717948717
				],
				[
					61.02564102564103,
					7.846153846153845
				],
				[
					61.02564102564103,
					6.974358974358974
				],
				[
					61.02564102564103,
					6.102564102564102
				],
				[
					60.15384615384615,
					5.23076923076923
				],
				[
					60.15384615384615,
					4.358974358974359
				],
				[
					60.15384615384615,
					3.487179487179487
				],
				[
					59.282051282051285,
					2.615384615384615
				],
				[
					59.282051282051285,
					1.7435897435897434
				],
				[
					59.282051282051285,
					0.8717948717948717
				],
				[
					58.41025641025641,
					0.8717948717948717
				],
				[
					58.41025641025641,
					-0.8717948717948717
				],
				[
					57.53846153846154,
					-2.615384615384615
				],
				[
					57.53846153846154,
					-4.358974358974359
				],
				[
					57.53846153846154,
					-6.102564102564102
				],
				[
					56.666666666666664,
					-7.846153846153845
				],
				[
					56.666666666666664,
					-9.58974358974359
				],
				[
					55.794871794871796,
					-10.46153846153846
				],
				[
					55.794871794871796,
					-11.333333333333332
				],
				[
					55.794871794871796,
					-12.205128205128204
				],
				[
					54.92307692307693,
					-12.205128205128204
				],
				[
					54.92307692307693,
					-13.076923076923075
				],
				[
					54.05128205128205,
					-13.076923076923075
				],
				[
					53.17948717948718,
					-13.076923076923075
				],
				[
					52.30769230769231,
					-13.076923076923075
				],
				[
					51.43589743589744,
					-13.076923076923075
				],
				[
					49.69230769230769,
					-13.076923076923075
				],
				[
					47.94871794871795,
					-13.076923076923075
				],
				[
					45.333333333333336,
					-13.076923076923075
				],
				[
					40.1025641025641,
					-11.333333333333332
				],
				[
					38.35897435897436,
					-10.46153846153846
				],
				[
					37.48717948717949,
					-10.46153846153846
				],
				[
					36.61538461538461,
					-10.46153846153846
				],
				[
					35.743589743589745,
					-10.46153846153846
				],
				[
					33.12820512820513,
					-9.58974358974359
				],
				[
					32.256410256410255,
					-9.58974358974359
				],
				[
					31.384615384615387,
					-8.717948717948717
				],
				[
					30.512820512820515,
					-8.717948717948717
				],
				[
					29.641025641025642,
					-8.717948717948717
				],
				[
					28.76923076923077,
					-8.717948717948717
				],
				[
					27.897435897435898,
					-7.846153846153845
				],
				[
					27.025641025641026,
					-7.846153846153845
				],
				[
					27.025641025641026,
					-6.974358974358974
				],
				[
					23.53846153846154,
					-6.974358974358974
				],
				[
					22.666666666666668,
					-6.102564102564102
				],
				[
					17.435897435897438,
					-4.358974358974359
				],
				[
					16.564102564102566,
					-4.358974358974359
				],
				[
					15.692307692307693,
					-4.358974358974359
				],
				[
					14.820512820512821,
					-4.358974358974359
				],
				[
					13.948717948717949,
					-4.358974358974359
				],
				[
					13.076923076923077,
					-4.358974358974359
				],
				[
					12.205128205128204,
					-4.358974358974359
				],
				[
					10.461538461538462,
					-4.358974358974359
				],
				[
					9.58974358974359,
					-4.358974358974359
				],
				[
					9.58974358974359,
					-3.487179487179487
				],
				[
					8.717948717948719,
					-3.487179487179487
				],
				[
					7.846153846153847,
					-3.487179487179487
				],
				[
					6.9743589743589745,
					-3.487179487179487
				],
				[
					6.102564102564102,
					-3.487179487179487
				],
				[
					4.3589743589743595,
					-3.487179487179487
				],
				[
					3.4871794871794872,
					-3.487179487179487
				],
				[
					2.6153846153846154,
					-2.615384615384615
				],
				[
					0.8717948717948718,
					-2.615384615384615
				],
				[
					0.8717948717948718,
					-1.7435897435897434
				],
				[
					0,
					-1.7435897435897434
				],
				[
					-0.8717948717948718,
					-0.8717948717948717
				],
				[
					-1.7435897435897436,
					-0.8717948717948717
				],
				[
					-2.6153846153846154,
					-0.8717948717948717
				],
				[
					-2.6153846153846154,
					0
				],
				[
					-3.4871794871794872,
					0
				],
				[
					-4.3589743589743595,
					0
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
			"version": 114,
			"versionNonce": 1275775472,
			"isDeleted": false,
			"id": "tWNJyDfDK1M5Ih0z_RdCc",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3284.344761690561,
			"y": -548.8571166317746,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 101.87426125191132,
			"height": 63.79748180288732,
			"seed": 1517514512,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.5043317975240598
				],
				[
					0,
					1.260823722234818
				],
				[
					0,
					2.269475774132161
				],
				[
					0,
					3.2781278260296176
				],
				[
					0.2521485840359219,
					4.79111167545102
				],
				[
					0.5043433406747226,
					6.556267195209841
				],
				[
					0.5043433406747226,
					7.8170793742939395
				],
				[
					0.5043433406747226,
					9.582234894052704
				],
				[
					0.7564919247106445,
					11.09521874347422
				],
				[
					0.7564919247106445,
					12.608202592895623
				],
				[
					1.0086405087465664,
					13.364694517606381
				],
				[
					1.0086405087465664,
					13.869014771979664
				],
				[
					1.2608352653853672,
					13.869014771979664
				],
				[
					1.512983849421289,
					13.869014771979664
				],
				[
					1.7651324334574383,
					13.869014771979664
				],
				[
					2.017327190096239,
					13.869014771979664
				],
				[
					2.269475774132161,
					13.869014771979664
				],
				[
					2.521624358168083,
					13.869014771979664
				],
				[
					2.7738191148068836,
					13.869014771979664
				],
				[
					3.0259676988428055,
					13.869014771979664
				],
				[
					3.530311039517528,
					13.869014771979664
				],
				[
					3.7824596235536774,
					13.869014771979664
				],
				[
					4.2868029642284,
					13.869014771979664
				],
				[
					4.791100132300244,
					13.869014771979664
				],
				[
					5.295443472974966,
					14.373346569503724
				],
				[
					6.30408398172176,
					14.625506696690422
				],
				[
					7.3127706630712055,
					14.877678367027784
				],
				[
					8.321411171818,
					15.381998621401067
				],
				[
					9.077903096528644,
					15.634170291738542
				],
				[
					10.338738361914238,
					16.390662216449186
				],
				[
					11.599527454696727,
					16.894982470822583
				],
				[
					12.860362720082321,
					17.65147439553334
				],
				[
					13.869003228828888,
					18.1558061930574
				],
				[
					15.381987078250404,
					19.164458244954744
				],
				[
					16.894970927671693,
					19.668790042478804
				],
				[
					18.40795477709321,
					20.67744209437626
				],
				[
					20.42528196718945,
					21.433934019086905
				],
				[
					22.190414400646887,
					22.442597614135025
				],
				[
					24.207741590743126,
					23.451249666032368
				],
				[
					26.477217364875287,
					24.712073388267186
				],
				[
					28.746693139007448,
					25.46856531297783
				],
				[
					30.76402032910346,
					26.729377492061985
				],
				[
					33.03349610323585,
					27.485869416772744
				],
				[
					35.05077712072921,
					28.49453301182075
				],
				[
					36.5637609701505,
					29.251024936531508
				],
				[
					38.328939576210814,
					30.25967698842885
				],
				[
					39.84192342563233,
					30.76400878595291
				],
				[
					41.35490727505362,
					31.772660837850367
				],
				[
					43.12003970851106,
					32.52915276256101
				],
				[
					45.1373668986073,
					33.53780481445847
				],
				[
					47.15464791610066,
					34.04213661198253
				],
				[
					48.919826522160974,
					35.302960334217346
				],
				[
					50.937107539654335,
					36.05945225892799
				],
				[
					53.458778070425296,
					36.81594418363875
				],
				[
					55.72825384455746,
					37.82459623553609
				],
				[
					58.24987820272554,
					38.83324828743355
				],
				[
					60.5193539768577,
					39.58974021214419
				],
				[
					62.53668116695394,
					40.34623213685495
				],
				[
					64.8061569410861,
					41.35489573190307
				],
				[
					66.57128937454354,
					42.11138765661383
				],
				[
					68.58861656463978,
					42.86787958132447
				],
				[
					70.10160041406107,
					43.62437150603523
				],
				[
					71.36238950684378,
					44.128691760408515
				],
				[
					72.62322477222915,
					44.633023557932574
				],
				[
					73.63186528097594,
					45.38951548264333
				],
				[
					74.64055196232539,
					45.89384728016739
				],
				[
					75.39704388703626,
					46.398167534540676
				],
				[
					76.1535358117469,
					47.154659459251434
				],
				[
					77.16217632049347,
					47.406831129588795
				],
				[
					77.91866824520434,
					48.16332305429955
				],
				[
					79.17950351058971,
					48.66764330867284
				],
				[
					80.69248736001123,
					49.676306903720956
				],
				[
					81.7011278687578,
					50.432798828431714
				],
				[
					82.96196313414339,
					51.18929075314247
				],
				[
					84.4749469835649,
					51.94578267785312
				],
				[
					86.24007941702212,
					52.450102932226514
				],
				[
					87.50091468240771,
					53.45876652727463
				],
				[
					88.5095551911545,
					53.96308678164792
				],
				[
					90.0225390405758,
					54.971750376696036
				],
				[
					91.03117954932259,
					55.2239220470334
				],
				[
					91.78767147403323,
					55.980413971744156
				],
				[
					92.54416339874388,
					56.48473422611744
				],
				[
					93.30065532345475,
					56.736905896454914
				],
				[
					94.3093420048042,
					57.49339782116556
				],
				[
					94.56149058884012,
					57.745546405201594
				],
				[
					95.31798251355076,
					58.24988974587632
				],
				[
					95.57013109758691,
					58.50203832991224
				],
				[
					96.07447443826163,
					58.7542100002496
				],
				[
					96.07447443826163,
					59.258530254623
				],
				[
					96.32662302229755,
					59.258530254623
				],
				[
					96.57881777893635,
					59.51070192496036
				],
				[
					96.57881777893635,
					59.76287359529772
				],
				[
					96.8309663629725,
					59.76287359529772
				],
				[
					97.0831149470082,
					59.76287359529772
				],
				[
					97.0831149470082,
					60.015022179333755
				],
				[
					97.335309703647,
					60.015022179333755
				],
				[
					97.58745828768315,
					60.267193849671116
				],
				[
					97.58745828768315,
					60.51936552000848
				],
				[
					97.83960687171907,
					61.02368577438176
				],
				[
					98.34395021239379,
					61.02368577438176
				],
				[
					98.84829355306852,
					61.52800602875516
				],
				[
					99.35259072114059,
					62.03234936942988
				],
				[
					99.85693406181508,
					62.53666962380328
				],
				[
					100.36127740249003,
					62.78884129414064
				],
				[
					100.86557457056188,
					63.29316154851392
				],
				[
					101.36991791123683,
					63.29316154851392
				],
				[
					101.62206649527252,
					63.79748180288732
				],
				[
					101.87426125191132,
					63.79748180288732
				],
				[
					101.87426125191132,
					63.79748180288732
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 134,
			"versionNonce": 637275120,
			"isDeleted": false,
			"id": "_RntBX9SE_rX9YDNKGoT5",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3426.3130949521405,
			"y": -338.0480297646699,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 26.729412121514088,
			"height": 123.30818372784756,
			"seed": 1716718864,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.5043433406744953,
					0
				],
				[
					-0.7564919247106445,
					0
				],
				[
					-1.2608352653853672,
					0
				],
				[
					-1.7651786060600898,
					0
				],
				[
					-2.2694757741319336,
					0.2521716703373613
				],
				[
					-2.7738191148068836,
					0.2521716703373613
				],
				[
					-3.2781624554816062,
					0.5043202543732832
				],
				[
					-4.034654380192251,
					0.5043202543732832
				],
				[
					-4.286802964228173,
					0.5043202543732832
				],
				[
					-5.043294888938817,
					0.5043202543732832
				],
				[
					-5.547638229613767,
					0.5043202543732832
				],
				[
					-5.799786813649689,
					0.2521716703373613
				],
				[
					-6.051935397685611,
					0.2521716703373613
				],
				[
					-6.051935397685611,
					0
				],
				[
					-6.304130154324412,
					0
				],
				[
					-6.556278738360561,
					0
				],
				[
					-7.060622079035056,
					-0.2521716703373613
				],
				[
					-7.3127706630712055,
					-0.5043202543732832
				],
				[
					-7.564919247107127,
					-0.7564919247107582
				],
				[
					-8.06926258778185,
					-1.0086635950480058
				],
				[
					-8.573605928456573,
					-1.5129838494214027
				],
				[
					-8.825754512492495,
					-2.0173041037947996
				],
				[
					-9.330097853167445,
					-2.773796028505444
				],
				[
					-9.834395021239288,
					-3.025967698842919
				],
				[
					-10.086589777878089,
					-4.034631293891039
				],
				[
					-10.338738361914011,
					-4.791123218601683
				],
				[
					-10.590886945949933,
					-5.547615143312328
				],
				[
					-10.843081702588734,
					-6.3041070680232
				],
				[
					-11.347378870660577,
					-7.564919247107241
				],
				[
					-11.599573627299378,
					-8.57358284215536
				],
				[
					-11.851722211335527,
					-9.582223350901927
				],
				[
					-12.10387079537145,
					-10.590886945950047
				],
				[
					-12.608214136046172,
					-12.103870795371563
				],
				[
					-12.860362720082094,
					-13.112534390419682
				],
				[
					-13.364706060756816,
					-14.625518239841085
				],
				[
					-13.616854644792966,
					-15.886330418925127
				],
				[
					-14.121197985467461,
					-17.39931426834653
				],
				[
					-14.37334656950361,
					-18.912298117768046
				],
				[
					-14.625541326142411,
					-20.42528196718945
				],
				[
					-14.625541326142411,
					-21.686094146273604
				],
				[
					-14.625541326142411,
					-23.199077995694893
				],
				[
					-14.625541326142411,
					-24.459913261080487
				],
				[
					-14.625541326142411,
					-25.97289711050189
				],
				[
					-14.877689910178333,
					-27.485880959923293
				],
				[
					-15.129838494214255,
					-29.25101339338073
				],
				[
					-15.382033250853056,
					-31.016168913139495
				],
				[
					-15.634181834889205,
					-32.78132443289837
				],
				[
					-16.1385251755637,
					-34.79862853669317
				],
				[
					-16.64282234363577,
					-37.06810431082533
				],
				[
					-17.147165684310494,
					-39.08540841462013
				],
				[
					-17.651509024985216,
					-41.10273560471626
				],
				[
					-18.155806193057288,
					-42.8678680381737
				],
				[
					-18.66014953373201,
					-45.13734381230586
				],
				[
					-18.912298117767932,
					-46.902499332064735
				],
				[
					-19.164492874406733,
					-48.66765485182361
				],
				[
					-19.668790042478577,
					-50.43278728528094
				],
				[
					-19.668790042478577,
					-51.94577113470234
				],
				[
					-19.920984799117377,
					-53.45875498412386
				],
				[
					-20.173133383153527,
					-54.97173883354537
				],
				[
					-20.42528196718922,
					-56.48472268296666
				],
				[
					-20.677476723828022,
					-57.49338627801478
				],
				[
					-20.677476723828022,
					-59.25854179777366
				],
				[
					-20.92962530786417,
					-60.26718230652034
				],
				[
					-21.181773891900093,
					-61.52801757190582
				],
				[
					-21.433968648538894,
					-62.78882975098986
				],
				[
					-21.686117232574816,
					-64.04964193007402
				],
				[
					-21.938265816610965,
					-65.31047719545938
				],
				[
					-22.190460573249766,
					-66.31911770420618
				],
				[
					-22.190460573249766,
					-67.57995296959155
				],
				[
					-22.190460573249766,
					-68.58859347833834
				],
				[
					-22.190460573249766,
					-69.8494287437237
				],
				[
					-22.44260915728546,
					-71.11024092280786
				],
				[
					-22.44260915728546,
					-72.11890451785587
				],
				[
					-22.69475774132161,
					-73.37971669694002
				],
				[
					-22.69475774132161,
					-74.64052887602406
				],
				[
					-22.69475774132161,
					-75.90136414140954
				],
				[
					-22.69475774132161,
					-77.16217632049359
				],
				[
					-22.69475774132161,
					-78.42298849957763
				],
				[
					-22.69475774132161,
					-79.68382376496311
				],
				[
					-22.94695249796041,
					-80.94463594404726
				],
				[
					-22.94695249796041,
					-82.70979146380603
				],
				[
					-23.199101081996332,
					-84.22277531322754
				],
				[
					-23.199101081996332,
					-85.48358749231159
				],
				[
					-23.199101081996332,
					-87.24874301207035
				],
				[
					-23.703444422671055,
					-88.50955519115439
				],
				[
					-23.703444422671055,
					-90.02253904057591
				],
				[
					-23.703444422671055,
					-91.28335121965995
				],
				[
					-23.703444422671055,
					-92.54418648504543
				],
				[
					-23.955593006706977,
					-94.30931891850287
				],
				[
					-23.955593006706977,
					-95.06581084321351
				],
				[
					-23.955593006706977,
					-96.326646108599
				],
				[
					-24.2077415907429,
					-97.33528661734567
				],
				[
					-24.2077415907429,
					-98.34395021239379
				],
				[
					-24.4599363473817,
					-99.35261380744191
				],
				[
					-24.4599363473817,
					-100.86559765686332
				],
				[
					-24.4599363473817,
					-101.62208958157407
				],
				[
					-24.71208493141785,
					-102.88290176065811
				],
				[
					-24.71208493141785,
					-103.89156535570623
				],
				[
					-24.964233515453543,
					-105.65669778916367
				],
				[
					-25.216428272092344,
					-106.41318971387443
				],
				[
					-25.216428272092344,
					-107.92617356329583
				],
				[
					-25.216428272092344,
					-108.93483715834395
				],
				[
					-25.216428272092344,
					-109.94350075339196
				],
				[
					-25.468576856128493,
					-110.95214126213875
				],
				[
					-25.468576856128493,
					-111.96080485718687
				],
				[
					-25.468576856128493,
					-112.96946845223488
				],
				[
					-25.720725440164415,
					-113.72596037694564
				],
				[
					-25.720725440164415,
					-114.4824523016564
				],
				[
					-25.720725440164415,
					-114.73460088569232
				],
				[
					-25.720725440164415,
					-115.49109281040307
				],
				[
					-25.972920196803216,
					-116.24758473511372
				],
				[
					-25.972920196803216,
					-116.75192807578856
				],
				[
					-26.225068780839138,
					-117.5084200004992
				],
				[
					-26.225068780839138,
					-118.0127402548726
				],
				[
					-26.225068780839138,
					-118.76923217958335
				],
				[
					-26.477217364875287,
					-119.02140384992072
				],
				[
					-26.477217364875287,
					-119.27355243395664
				],
				[
					-26.729412121514088,
					-119.77789577463147
				],
				[
					-26.729412121514088,
					-120.28221602900476
				],
				[
					-26.729412121514088,
					-120.53438769934212
				],
				[
					-26.729412121514088,
					-120.78653628337804
				],
				[
					-26.729412121514088,
					-121.03870795371552
				],
				[
					-26.729412121514088,
					-121.29087962405288
				],
				[
					-26.729412121514088,
					-121.5430282080888
				],
				[
					-26.729412121514088,
					-121.79519987842616
				],
				[
					-26.729412121514088,
					-122.04737154876364
				],
				[
					-26.729412121514088,
					-122.29952013279956
				],
				[
					-26.729412121514088,
					-122.80386347347428
				],
				[
					-26.729412121514088,
					-122.80386347347428
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 52,
			"versionNonce": 1953828336,
			"isDeleted": false,
			"id": "-7kxOFBgRmQUiz3ZnbKhR",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3386.413678208949,
			"y": -469.75815437875656,
			"strokeColor": "#ced4da",
			"backgroundColor": "transparent",
			"width": 2.16315365131436,
			"height": 10.506746306383434,
			"seed": 1351543568,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.20602092052615717
				],
				[
					0,
					0.3090219501876845
				],
				[
					-0.10301989086451613,
					0.6180439003754827
				],
				[
					-0.10301989086451613,
					0.8240648209016399
				],
				[
					-0.10301989086451613,
					1.1330867710894381
				],
				[
					-0.20602092052627086,
					1.4421087212771226
				],
				[
					-0.20602092052627086,
					1.5451097509387637
				],
				[
					-0.20602092052627086,
					1.7511306714649209
				],
				[
					-0.3090219501877982,
					2.0601526216526054
				],
				[
					-0.3090219501877982,
					2.1631536513142464
				],
				[
					-0.3090219501877982,
					2.472175601501931
				],
				[
					-0.3090219501877982,
					2.678196522028088
				],
				[
					-0.41204184105231434,
					3.0902195018774137
				],
				[
					-0.6180439003755964,
					3.399241452065212
				],
				[
					-0.7210637912401126,
					3.811273862516032
				],
				[
					-0.8240648209016399,
					4.326307302628493
				],
				[
					-0.9270658505631673,
					4.738339713079313
				],
				[
					-1.0300857414279108,
					5.3563836134547955
				],
				[
					-1.0300857414279108,
					5.871417053567143
				],
				[
					-1.1330867710894381,
					6.180439003754941
				],
				[
					-1.2360878007509655,
					6.592471414205761
				],
				[
					-1.2360878007509655,
					7.004503824656581
				],
				[
					-1.2360878007509655,
					7.210515314581244
				],
				[
					-1.339107691615709,
					7.4165268045059065
				],
				[
					-1.339107691615709,
					7.622547725032064
				],
				[
					-1.339107691615709,
					7.725548754693705
				],
				[
					-1.4421087212772363,
					7.8285592149567265
				],
				[
					-1.4421087212772363,
					7.931569675219862
				],
				[
					-1.4421087212772363,
					8.03457070488139
				],
				[
					-1.4421087212772363,
					8.240591625407546
				],
				[
					-1.6481296418032798,
					8.343592655069187
				],
				[
					-1.6481296418032798,
					8.549613575595345
				],
				[
					-1.6481296418032798,
					8.755625065520007
				],
				[
					-1.6481296418032798,
					8.85863552578303
				],
				[
					-1.7511306714650345,
					9.064647015707692
				],
				[
					-1.7511306714650345,
					9.270658505632355
				],
				[
					-1.854131701126562,
					9.476679426158626
				],
				[
					-1.957151591991078,
					9.682690916083175
				],
				[
					-1.957151591991078,
					9.78570137634631
				],
				[
					-1.957151591991078,
					9.888702406007951
				],
				[
					-2.0601526216526054,
					9.991712866270973
				],
				[
					-2.0601526216526054,
					10.094723326534108
				],
				[
					-2.0601526216526054,
					10.197724356195636
				],
				[
					-2.16315365131436,
					10.300734816458771
				],
				[
					-2.16315365131436,
					10.403745276721793
				],
				[
					-2.16315365131436,
					10.506746306383434
				],
				[
					-2.16315365131436,
					10.506746306383434
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 127,
			"versionNonce": 1350422512,
			"isDeleted": false,
			"id": "_CGcoO86oVU_BqmDUbxTz",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3380.0272182846675,
			"y": -462.7536505541001,
			"strokeColor": "#ced4da",
			"backgroundColor": "transparent",
			"width": 14.111989817771928,
			"height": 6.695472443867402,
			"seed": 60754192,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.20602092052627086,
					0
				],
				[
					-0.41202297984932557,
					0
				],
				[
					-0.7210449300371238,
					0
				],
				[
					-0.8240648209018673,
					0
				],
				[
					-1.1330867710894381,
					-0.10301046026313543
				],
				[
					-1.2360878007509655,
					-0.10301046026313543
				],
				[
					-1.3390888304127202,
					-0.10301046026313543
				],
				[
					-1.4421087212772363,
					-0.10301046026313543
				],
				[
					-1.5451097509387637,
					-0.10301046026313543
				],
				[
					-1.6481107806005184,
					-0.10301046026313543
				],
				[
					-1.854131701126562,
					-0.10301046026313543
				],
				[
					-1.9571327307880892,
					-0.10301046026313543
				],
				[
					-2.0601526216528327,
					-0.10301046026313543
				],
				[
					-2.16315365131436,
					-0.10301046026313543
				],
				[
					-2.16315365131436,
					0
				],
				[
					-2.2661546809758875,
					0.20601148992466278
				],
				[
					-2.3691745718404036,
					0.20601148992466278
				],
				[
					-2.4721756015021583,
					0.3090219501877982
				],
				[
					-2.4721756015021583,
					0.41202297984932557
				],
				[
					-2.4721756015021583,
					0.515033440112461
				],
				[
					-2.4721756015021583,
					0.7210449300371238
				],
				[
					-2.4721756015021583,
					0.927065850563281
				],
				[
					-2.5751766311636857,
					1.0300668802248083
				],
				[
					-2.5751766311636857,
					1.2360878007509655
				],
				[
					-2.5751766311636857,
					1.4420992906756283
				],
				[
					-2.5751766311636857,
					1.5451097509387637
				],
				[
					-2.5751766311636857,
					1.648110780600291
				],
				[
					-2.5751766311636857,
					1.7511212408634265
				],
				[
					-2.5751766311636857,
					1.8541317011264482
				],
				[
					-2.5751766311636857,
					1.9571327307880892
				],
				[
					-2.2661546809758875,
					2.060143191051111
				],
				[
					-2.0601526216528327,
					2.2661546809757738
				],
				[
					-1.7511306714650345,
					2.369165141238909
				],
				[
					-1.4421087212772363,
					2.575176631163572
				],
				[
					-1.2360878007509655,
					2.781197551689729
				],
				[
					-0.9270658505633946,
					2.987209041614392
				],
				[
					-0.7210449300371238,
					3.1932205315390547
				],
				[
					-0.41202297984932557,
					3.399241452065212
				],
				[
					-0.20602092052627086,
					3.502242481726853
				],
				[
					-0.10300102966152735,
					3.70826340225301
				],
				[
					0.20602092052604348,
					3.914274892177673
				],
				[
					0.41202297984932557,
					4.017285352440695
				],
				[
					0.618043900375369,
					4.017285352440695
				],
				[
					0.9270658505631673,
					4.120286382102336
				],
				[
					1.0300668802246946,
					4.120286382102336
				],
				[
					1.2360878007509655,
					4.223296842365357
				],
				[
					1.5451097509387637,
					4.223296842365357
				],
				[
					1.9571327307880892,
					4.326307302628493
				],
				[
					2.1631536513141327,
					4.326307302628493
				],
				[
					2.3691745718404036,
					4.42930833229002
				],
				[
					2.781197551689729,
					4.532318792553156
				],
				[
					2.8841985813512565,
					4.532318792553156
				],
				[
					3.296240422403571,
					4.635329252816177
				],
				[
					3.502242481726853,
					4.635329252816177
				],
				[
					3.9142843227791673,
					4.841340742740954
				],
				[
					4.223306272966738,
					4.944351203003976
				],
				[
					4.532328223154536,
					5.150362692928638
				],
				[
					5.047352232665389,
					5.253373153191774
				],
				[
					5.150372123530133,
					5.356374182853301
				],
				[
					5.459394073717931,
					5.562395103379458
				],
				[
					5.768416023905502,
					5.665396133041099
				],
				[
					5.974418083228784,
					5.768406593304121
				],
				[
					6.283440033416582,
					5.8714170535672565
				],
				[
					6.489460953942626,
					5.974418083228784
				],
				[
					6.798482904130424,
					6.077428543491919
				],
				[
					7.004503824656467,
					6.077428543491919
				],
				[
					7.3135257748442655,
					6.180439003754941
				],
				[
					7.622547725032064,
					6.180439003754941
				],
				[
					8.03457070488139,
					6.283440033416582
				],
				[
					8.343592655069187,
					6.283440033416582
				],
				[
					8.85863552578303,
					6.386450493679604
				],
				[
					9.167657475970827,
					6.386450493679604
				],
				[
					9.476679426158626,
					6.386450493679604
				],
				[
					9.785701376346196,
					6.489460953942739
				],
				[
					10.197724356195522,
					6.489460953942739
				],
				[
					10.50674630638332,
					6.489460953942739
				],
				[
					10.712767226909591,
					6.592461983604267
				],
				[
					10.918769286232646,
					6.592461983604267
				],
				[
					11.02178917709739,
					6.592461983604267
				],
				[
					11.227791236420444,
					6.592461983604267
				],
				[
					11.33081112728496,
					6.592461983604267
				],
				[
					11.433812156946487,
					6.592461983604267
				],
				[
					11.433812156946487,
					6.489460953942739
				],
				[
					11.536813186608242,
					6.489460953942739
				],
				[
					11.536813186608242,
					6.283440033416582
				],
				[
					11.536813186608242,
					6.180439003754941
				],
				[
					11.536813186608242,
					5.974418083228784
				],
				[
					11.536813186608242,
					5.8714170535672565
				],
				[
					11.536813186608242,
					5.562395103379458
				],
				[
					11.433812156946487,
					5.356374182853301
				],
				[
					11.33081112728496,
					5.150362692928638
				],
				[
					11.227791236420444,
					4.944351203003976
				],
				[
					11.02178917709739,
					4.738330282477818
				],
				[
					10.815768256571118,
					4.42930833229002
				],
				[
					10.712767226909591,
					4.223296842365357
				],
				[
					10.609747336044848,
					4.120286382102336
				],
				[
					10.403745276721793,
					4.017285352440695
				],
				[
					10.300725385857277,
					3.914274892177673
				],
				[
					10.197724356195522,
					3.70826340225301
				],
				[
					10.197724356195522,
					3.6052529419898747
				],
				[
					10.094723326533995,
					3.502242481726853
				],
				[
					9.991703435669478,
					3.502242481726853
				],
				[
					9.888702406007951,
					3.399241452065212
				],
				[
					9.68268148548168,
					3.29623099180219
				],
				[
					9.579680455820153,
					3.1932205315390547
				],
				[
					9.373659535293882,
					3.0902195018775274
				],
				[
					9.064637585106311,
					2.987209041614392
				],
				[
					8.961636555444557,
					2.88419858135137
				],
				[
					8.549613575595231,
					2.88419858135137
				],
				[
					8.343592655069187,
					2.781197551689729
				],
				[
					8.137571734542917,
					2.575176631163572
				],
				[
					7.931569675219862,
					2.575176631163572
				],
				[
					7.828549784355118,
					2.4721756015020446
				],
				[
					7.725548754693591,
					2.4721756015020446
				],
				[
					7.622547725032064,
					2.369165141238909
				],
				[
					7.416526804505793,
					2.369165141238909
				],
				[
					7.3135257748442655,
					2.369165141238909
				],
				[
					7.107504854318222,
					2.2661546809757738
				],
				[
					7.107504854318222,
					2.1631536513142464
				],
				[
					7.004503824656467,
					2.060143191051111
				],
				[
					7.004503824656467,
					1.9571327307880892
				],
				[
					7.004503824656467,
					1.9571327307880892
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 456,
			"versionNonce": 1914589680,
			"isDeleted": false,
			"id": "_z5J-zyS68XxWJ64h2BSF",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3372.8167124006877,
			"y": -462.95967147462613,
			"strokeColor": "#ced4da",
			"backgroundColor": "transparent",
			"width": 26.47286782528181,
			"height": 34.404446931103166,
			"seed": 1526425360,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.20602092052615717
				],
				[
					0,
					0.3090219501877982
				],
				[
					-0.10301989086451613,
					0.7210543606386182
				],
				[
					-0.30902195018757084,
					1.2360878007509655
				],
				[
					-0.41204184105231434,
					1.9571421613895836
				],
				[
					-0.618043900375369,
					2.5751860617650664
				],
				[
					-0.9270658505631673,
					3.5022519123283473
				],
				[
					-1.0300857414276834,
					4.53232822315465
				],
				[
					-1.2360878007509655,
					5.665405563642594
				],
				[
					-1.5451097509385363,
					7.004503824656581
				],
				[
					-2.0601526216526054,
					8.446603115332323
				],
				[
					-2.369174571840176,
					9.991712866270973
				],
				[
					-2.8842174425542453,
					11.536822617209737
				],
				[
					-3.1932393927420435,
					12.978921907885365
				],
				[
					-3.605262372591369,
					14.421030629162601
				],
				[
					-3.91428432277894,
					15.657118429913567
				],
				[
					-4.120305243305211,
					16.79019577040151
				],
				[
					-4.3263073026282655,
					17.92327311088934
				],
				[
					-4.738349143680807,
					18.953349421715757
				],
				[
					-5.047371093868378,
					20.086426762203587
				],
				[
					-5.25337315319166,
					20.70447066257907
				],
				[
					-5.665414994243974,
					21.528535483480823
				],
				[
					-5.871417053567029,
					22.249580413517833
				],
				[
					-5.974436944431773,
					22.867624313893316
				],
				[
					-6.0774379740933,
					23.4856682142688
				],
				[
					-6.180439003754827,
					23.89770062471962
				],
				[
					-6.180439003754827,
					24.41273406483208
				],
				[
					-6.180439003754827,
					24.618754985358237
				],
				[
					-6.180439003754827,
					24.927776935546035
				],
				[
					-6.180439003754827,
					25.133788425470698
				],
				[
					-6.180439003754827,
					25.442810375658382
				],
				[
					-6.180439003754827,
					25.75183232584618
				],
				[
					-6.180439003754827,
					25.854842786109202
				],
				[
					-6.180439003754827,
					26.06085427603398
				],
				[
					-6.180439003754827,
					26.266865765958528
				],
				[
					-6.180439003754827,
					26.369876226221663
				],
				[
					-6.180439003754827,
					26.4728866864848
				],
				[
					-6.180439003754827,
					26.575887716146326
				],
				[
					-6.180439003754827,
					26.67889817640946
				],
				[
					-6.180439003754827,
					26.781908636672483
				],
				[
					-6.180439003754827,
					26.884909666334124
				],
				[
					-6.180439003754827,
					27.19393161652181
				],
				[
					-6.180439003754827,
					27.502953566709607
				],
				[
					-6.180439003754827,
					27.60596402697263
				],
				[
					-6.180439003754827,
					27.914985977160427
				],
				[
					-6.180439003754827,
					28.12099746708509
				],
				[
					-6.0774379740933,
					28.327018387611247
				],
				[
					-5.871417053567029,
					28.430019417272774
				],
				[
					-5.562395103379458,
					28.63604033779893
				],
				[
					-5.150372123529905,
					28.842051827723708
				],
				[
					-4.8413501733423345,
					28.94506228798673
				],
				[
					-4.532328223154536,
					29.151073777911392
				],
				[
					-4.120305243305211,
					29.357085267836055
				],
				[
					-3.8112832931174125,
					29.563106188362212
				],
				[
					-3.399241452065098,
					29.769117678286875
				],
				[
					-2.781197551689729,
					30.078139628474673
				],
				[
					-2.266173542178649,
					30.387161578662358
				],
				[
					-1.6481296418032798,
					30.696183528850156
				],
				[
					-0.9270658505631673,
					30.90219501877482
				],
				[
					-0.20602092052604348,
					31.108215939300976
				],
				[
					0.5150240095110803,
					31.31422742922564
				],
				[
					1.4420898600742476,
					31.5202389191503
				],
				[
					2.369155710637415,
					31.72625983967646
				],
				[
					3.502242481726853,
					31.829260869337986
				],
				[
					4.532309361951775,
					32.03528178986426
				],
				[
					5.8714170535672565,
					32.24129327978892
				],
				[
					6.695463013265908,
					32.34430374005194
				],
				[
					7.622528863829302,
					32.44730476971358
				],
				[
					8.240572764204671,
					32.550315229976604
				],
				[
					8.858616664580268,
					32.550315229976604
				],
				[
					9.270658505632582,
					32.75632671990127
				],
				[
					9.682681485481908,
					32.75632671990127
				],
				[
					9.991703435669706,
					32.8593371801644
				],
				[
					10.403726415519031,
					32.962347640427424
				],
				[
					10.71274836570683,
					33.065348670089065
				],
				[
					11.0217703158944,
					33.16835913035209
				],
				[
					11.330792266082199,
					33.16835913035209
				],
				[
					11.53681318660847,
					33.27136959061522
				],
				[
					11.639814216269997,
					33.27136959061522
				],
				[
					11.742834107134513,
					33.27136959061522
				],
				[
					11.948836166457795,
					33.27136959061522
				],
				[
					12.051856057322311,
					33.27136959061522
				],
				[
					12.154857086983839,
					33.27136959061522
				],
				[
					12.257858116645366,
					33.27136959061522
				],
				[
					12.463879037171637,
					33.27136959061522
				],
				[
					12.669899957697908,
					33.27136959061522
				],
				[
					12.772900987359435,
					33.27136959061522
				],
				[
					12.772900987359435,
					33.16835913035209
				],
				[
					12.875902017020962,
					33.16835913035209
				],
				[
					12.978921907885479,
					32.8593371801644
				],
				[
					13.081922937547006,
					32.550315229976604
				],
				[
					13.390944887734804,
					32.138282819525784
				],
				[
					13.596965808261075,
					31.829260869337986
				],
				[
					13.905987758448873,
					31.31422742922564
				],
				[
					14.215009708636444,
					30.90219501877482
				],
				[
					14.524031658824242,
					30.59317306858702
				],
				[
					14.730033718147524,
					30.078139628474673
				],
				[
					15.039055668335095,
					29.666107218023853
				],
				[
					15.348077618522893,
					29.254084238174528
				],
				[
					15.554098539049164,
					28.739041367460572
				],
				[
					15.760119459575208,
					28.327018387611247
				],
				[
					15.760119459575208,
					27.81197551689729
				],
				[
					16.069141409763006,
					27.19393161652181
				],
				[
					16.172142439424533,
					26.575887716146326
				],
				[
					16.378163359950804,
					25.957843815770843
				],
				[
					16.48116438961233,
					25.33979991539536
				],
				[
					16.58416541927386,
					24.618754985358237
				],
				[
					16.79018633980013,
					23.89770062471962
				],
				[
					16.893187369461657,
					23.176646264081114
				],
				[
					17.099208289987928,
					22.45560133404399
				],
				[
					17.202209319649455,
					21.734546973405486
				],
				[
					17.4082302401755,
					21.11650307302989
				],
				[
					17.61425116070177,
					20.395448712391385
				],
				[
					17.820253220024824,
					19.880415272278924
				],
				[
					17.923273110889568,
					19.15936091164042
				],
				[
					18.129275170212622,
					18.541317011264937
				],
				[
					18.232295061077366,
					18.026283571152476
				],
				[
					18.335296090738893,
					17.511250131040015
				],
				[
					18.43829712040042,
					17.099217720589195
				],
				[
					18.541317011264937,
					16.687185310138375
				],
				[
					18.644318040926464,
					16.172151870026028
				],
				[
					18.74731907058822,
					15.760119459575208
				],
				[
					18.953339991114262,
					15.348096479725882
				],
				[
					19.056341020776017,
					14.833053609011927
				],
				[
					19.056341020776017,
					14.524031658824128
				],
				[
					19.056341020776017,
					14.215009708636444
				],
				[
					19.159360911640533,
					13.905987758448646
				],
				[
					19.26236194130206,
					13.49396477859932
				],
				[
					19.365362970963588,
					13.0819323681485
				],
				[
					19.46838286182833,
					12.772910417960702
				],
				[
					19.57138389148986,
					12.463888467773018
				],
				[
					19.674384921151386,
					12.15486651758522
				],
				[
					19.674384921151386,
					11.845844567397535
				],
				[
					19.674384921151386,
					11.639833077472872
				],
				[
					19.880405841677657,
					11.227800667022052
				],
				[
					19.880405841677657,
					11.02178917709739
				],
				[
					19.983406871339184,
					10.712767226909591
				],
				[
					20.0864267622037,
					10.506746306383434
				],
				[
					20.189427791865228,
					10.094723326534108
				],
				[
					20.189427791865228,
					9.888702406007951
				],
				[
					20.292428821526983,
					9.682690916083288
				],
				[
					20.292428821526983,
					9.476679426158626
				],
				[
					20.292428821526983,
					9.37366896589549
				],
				[
					20.292428821526983,
					9.270658505632468
				],
				[
					20.292428821526983,
					8.96163655544467
				],
				[
					20.292428821526983,
					8.858635525783143
				],
				[
					20.292428821526983,
					8.755625065520007
				],
				[
					20.292428821526983,
					8.446603115332323
				],
				[
					20.292428821526983,
					8.24059162540766
				],
				[
					20.292428821526983,
					7.931569675219862
				],
				[
					20.292428821526983,
					7.82855921495684
				],
				[
					20.292428821526983,
					7.622547725032064
				],
				[
					20.292428821526983,
					7.519537264769042
				],
				[
					20.292428821526983,
					7.313525774844379
				],
				[
					20.292428821526983,
					7.210515314581244
				],
				[
					20.189427791865228,
					7.210515314581244
				],
				[
					19.983406871339184,
					7.210515314581244
				],
				[
					19.674384921151386,
					7.210515314581244
				],
				[
					19.57138389148986,
					7.210515314581244
				],
				[
					19.26236194130206,
					7.210515314581244
				],
				[
					19.159360911640533,
					7.210515314581244
				],
				[
					19.056341020776017,
					7.210515314581244
				],
				[
					18.850338961452735,
					7.210515314581244
				],
				[
					18.541317011264937,
					7.210515314581244
				],
				[
					18.43829712040042,
					7.210515314581244
				],
				[
					18.129275170212622,
					7.210515314581244
				],
				[
					18.026274140551095,
					7.210515314581244
				],
				[
					17.820253220024824,
					7.210515314581244
				],
				[
					17.61425116070177,
					7.210515314581244
				],
				[
					17.30522921051397,
					7.210515314581244
				],
				[
					17.099208289987928,
					7.210515314581244
				],
				[
					16.893187369461657,
					7.210515314581244
				],
				[
					16.687185310138602,
					7.210515314581244
				],
				[
					16.378163359950804,
					7.210515314581244
				],
				[
					16.069141409763006,
					7.210515314581244
				],
				[
					15.863120489236735,
					7.210515314581244
				],
				[
					15.451097509387637,
					7.107504854318222
				],
				[
					14.936054638673568,
					7.004503824656581
				],
				[
					14.62703268848577,
					7.004503824656581
				],
				[
					14.111989817771928,
					6.901493364393559
				],
				[
					13.493945917396559,
					6.901493364393559
				],
				[
					13.081922937547006,
					6.798482904130424
				],
				[
					12.669899957697908,
					6.695481874468896
				],
				[
					12.257858116645366,
					6.489460953942739
				],
				[
					11.84583513679604,
					6.386459924281098
				],
				[
					11.433812156946715,
					6.2834494640180765
				],
				[
					11.124790206759144,
					6.2834494640180765
				],
				[
					10.918769286232873,
					6.180439003754941
				],
				[
					10.815768256571346,
					6.077437974093414
				],
				[
					10.609747336045075,
					5.974427513830278
				],
				[
					10.403726415519031,
					5.974427513830278
				],
				[
					10.300725385857277,
					5.7684160239056155
				],
				[
					9.991703435669706,
					5.7684160239056155
				],
				[
					9.682681485481908,
					5.562395103379458
				],
				[
					9.270658505632582,
					5.3563836134547955
				],
				[
					8.961636555444784,
					5.150372123530133
				],
				[
					8.446593684730942,
					4.944351203003976
				],
				[
					8.034570704881617,
					4.53232822315465
				],
				[
					7.622528863829302,
					4.429317762891515
				],
				[
					7.210505883979977,
					4.12029581270383
				],
				[
					6.9014839337921785,
					3.9142843227791673
				],
				[
					6.695463013265908,
					3.811273862516032
				],
				[
					6.386441063078109,
					3.605262372591369
				],
				[
					6.283440033416582,
					3.399241452065212
				],
				[
					6.180439003755055,
					3.2962404224036845
				],
				[
					6.077419112890539,
					3.193229962140549
				],
				[
					5.76839716270274,
					2.9872184722158863
				],
				[
					5.665396133041213,
					2.781197551689729
				],
				[
					5.459375212514942,
					2.678196522028202
				],
				[
					5.2533731531918875,
					2.472175601501931
				],
				[
					4.944351203004089,
					2.266164111577268
				],
				[
					4.841331312139573,
					2.1631536513142464
				],
				[
					4.532309361951775,
					1.9571421613895836
				],
				[
					4.326307302628493,
					1.8541317011264482
				],
				[
					4.326307302628493,
					1.6481202112017854
				],
				[
					4.223287411763977,
					1.6481202112017854
				],
				[
					4.120286382102449,
					1.5451097509387637
				],
				[
					4.017285352440922,
					1.5451097509387637
				],
				[
					4.017285352440922,
					1.4421087212771226
				],
				[
					3.811264431914651,
					1.2360878007509655
				],
				[
					3.811264431914651,
					1.1330867710894381
				],
				[
					3.708263402253124,
					0.927065850563281
				],
				[
					3.502242481726853,
					0.927065850563281
				],
				[
					3.3992414520653256,
					0.7210543606386182
				],
				[
					3.2962215612008094,
					0.5150428707139554
				],
				[
					3.193220531539282,
					0.41203241045081995
				],
				[
					3.193220531539282,
					0.3090219501877982
				],
				[
					3.0902195018775274,
					0.3090219501877982
				],
				[
					3.0902195018775274,
					0.20602092052615717
				],
				[
					2.9871996110130112,
					0.10301046026302174
				],
				[
					2.884198581351484,
					0
				],
				[
					2.884198581351484,
					-0.10300102966152735
				],
				[
					2.781197551689729,
					-0.3090219501877982
				],
				[
					2.678177660825213,
					-0.41202297984932557
				],
				[
					2.5751766311636857,
					-0.6180439003754827
				],
				[
					2.5751766311636857,
					-0.7210449300371238
				],
				[
					2.4721756015021583,
					-0.8240553903001455
				],
				[
					2.4721756015021583,
					-0.927065850563281
				],
				[
					2.4721756015021583,
					-1.0300668802248083
				],
				[
					2.369155710637415,
					-1.1330773404879437
				],
				[
					2.2661546809758875,
					-0.927065850563281
				],
				[
					2.16315365131436,
					-0.8240553903001455
				],
				[
					2.16315365131436,
					-0.41202297984932557
				],
				[
					2.16315365131436,
					0.10301046026302174
				],
				[
					2.060133760449844,
					0.6180439003754827
				],
				[
					2.060133760449844,
					1.339098261014101
				],
				[
					2.060133760449844,
					1.8541317011264482
				],
				[
					2.060133760449844,
					2.472175601501931
				],
				[
					2.060133760449844,
					3.0902195018775274
				],
				[
					2.060133760449844,
					3.605262372591369
				],
				[
					2.060133760449844,
					4.12029581270383
				],
				[
					1.9571327307880892,
					4.738339713079313
				],
				[
					1.9571327307880892,
					5.25337315319166
				],
				[
					1.9571327307880892,
					5.974427513830278
				],
				[
					1.7511118102620458,
					6.695481874468896
				],
				[
					1.7511118102620458,
					7.519537264769042
				],
				[
					1.6481107806005184,
					8.343592655069187
				],
				[
					1.4420898600742476,
					9.167657475970827
				],
				[
					1.3390888304127202,
					10.197724356195636
				],
				[
					1.2360878007511928,
					11.227800667022052
				],
				[
					1.1330679098864493,
					12.257876977848355
				],
				[
					1.1330679098864493,
					13.287943858073163
				],
				[
					1.030066880224922,
					14.215009708636444
				],
				[
					1.030066880224922,
					15.142075559199611
				],
				[
					0.9270658505633946,
					16.069141409762892
				],
				[
					0.9270658505633946,
					16.79019577040151
				],
				[
					0.9270658505633946,
					17.408239670776993
				],
				[
					0.8240459596986511,
					18.12929403141561
				],
				[
					0.6180439003755964,
					18.64432747152796
				],
				[
					0.41202297984955294,
					19.468382861828104
				],
				[
					0.20600205932328208,
					20.086426762203587
				],
				[
					0.20600205932328208,
					20.807481122842205
				],
				[
					0,
					21.425525023217688
				],
				[
					-0.20602092052604348,
					22.04356892359317
				],
				[
					-0.30902195018757084,
					22.45560133404399
				],
				[
					-0.41204184105231434,
					22.867624313893316
				],
				[
					-0.41204184105231434,
					23.176646264081114
				],
				[
					-0.41204184105231434,
					23.588678674531934
				],
				[
					-0.41204184105231434,
					23.89770062471962
				],
				[
					-0.41204184105231434,
					24.103712114644395
				],
				[
					-0.5150428707138417,
					24.41273406483208
				],
				[
					-0.618043900375369,
					24.618754985358237
				],
				[
					-0.7210637912398852,
					25.133788425470698
				],
				[
					-0.9270658505631673,
					25.442810375658382
				],
				[
					-1.1330867710892107,
					26.06085427603398
				],
				[
					-1.3391076916154816,
					26.4728866864848
				],
				[
					-1.5451097509385363,
					26.987920126597146
				],
				[
					-1.7511306714648072,
					27.502953566709607
				],
				[
					-1.7511306714648072,
					27.914985977160427
				],
				[
					-1.8541317011263345,
					28.22400792734811
				],
				[
					-1.8541317011263345,
					28.327018387611247
				],
				[
					-1.8541317011263345,
					28.430019417272774
				],
				[
					-1.8541317011263345,
					28.53302987753591
				],
				[
					-1.8541317011263345,
					28.63604033779893
				],
				[
					-1.7511306714648072,
					28.739041367460572
				],
				[
					-1.5451097509385363,
					29.048063317648257
				],
				[
					-1.2360878007509655,
					29.254084238174528
				],
				[
					-1.0300857414276834,
					29.666107218023853
				],
				[
					-0.5150428707138417,
					30.181150088737695
				],
				[
					-0.10301989086451613,
					30.490172038925493
				],
				[
					0.41202297984955294,
					30.90219501877482
				],
				[
					1.030066880224922,
					31.211216968962503
				],
				[
					1.9571327307880892,
					31.72625983967646
				],
				[
					2.678177660825213,
					32.03528178986426
				],
				[
					3.6052435113883803,
					32.34430374005194
				],
				[
					4.326307302628493,
					32.44730476971358
				],
				[
					4.944351203004089,
					32.550315229976604
				],
				[
					5.562395103379458,
					32.550315229976604
				],
				[
					6.180439003755055,
					32.550315229976604
				],
				[
					6.59246198360438,
					32.550315229976604
				],
				[
					7.004484963453706,
					32.44730476971358
				],
				[
					7.313506913641504,
					32.34430374005194
				],
				[
					7.828549784355346,
					32.34430374005194
				],
				[
					8.034570704881617,
					32.24129327978892
				],
				[
					8.240572764204671,
					32.138282819525784
				],
				[
					8.54959471439247,
					32.138282819525784
				],
				[
					8.858616664580268,
					32.03528178986426
				],
				[
					9.270658505632582,
					32.03528178986426
				],
				[
					9.682681485481908,
					32.03528178986426
				],
				[
					10.300725385857277,
					32.03528178986426
				],
				[
					10.71274836570683,
					32.03528178986426
				],
				[
					11.0217703158944,
					31.93227132960112
				],
				[
					11.330792266082199,
					31.72625983967646
				],
				[
					11.53681318660847,
					31.5202389191503
				],
				[
					11.639814216269997,
					31.211216968962503
				],
				[
					11.84583513679604,
					30.799193989113178
				],
				[
					12.154857086983839,
					30.284151118399336
				],
				[
					12.257858116645366,
					29.563106188362212
				],
				[
					12.978921907885479,
					26.781908636672483
				],
				[
					13.081922937547006,
					25.545820835921518
				],
				[
					13.287943858073277,
					24.206722574907417
				],
				[
					13.596965808261075,
					22.867624313893316
				],
				[
					13.905987758448873,
					21.425525023217688
				],
				[
					14.111989817771928,
					20.189437222466722
				],
				[
					14.421011767959726,
					18.747337931791094
				],
				[
					14.62703268848577,
					17.20222818085233
				],
				[
					14.936054638673568,
					15.86312991983823
				],
				[
					15.142075559199839,
					14.524031658824128
				],
				[
					15.451097509387637,
					13.0819323681485
				],
				[
					15.657099568710692,
					12.15486651758522
				],
				[
					15.863120489236735,
					11.227800667022052
				],
				[
					16.172142439424533,
					10.197724356195636
				],
				[
					16.378163359950804,
					9.270658505632468
				],
				[
					16.687185310138602,
					8.343592655069187
				],
				[
					16.893187369461657,
					7.725548754693705
				],
				[
					17.099208289987928,
					7.313525774844379
				],
				[
					17.30522921051397,
					6.901493364393559
				],
				[
					17.30522921051397,
					6.695481874468896
				],
				[
					17.30522921051397,
					6.901493364393559
				],
				[
					17.099208289987928,
					7.313525774844379
				],
				[
					16.79018633980013,
					7.82855921495684
				],
				[
					16.58416541927386,
					8.343592655069187
				],
				[
					16.172142439424533,
					9.167657475970827
				],
				[
					15.863120489236735,
					9.991712866270973
				],
				[
					15.245076588861366,
					10.918778716834254
				],
				[
					14.62703268848577,
					12.360878007509882
				],
				[
					13.80296786758413,
					13.802986728787118
				],
				[
					12.978921907885479,
					15.45109750938741
				],
				[
					12.051856057322311,
					17.20222818085233
				],
				[
					11.227791236420671,
					18.953349421715757
				],
				[
					10.19772435619575,
					20.91049158310534
				],
				[
					9.167638614768066,
					22.76462328423179
				],
				[
					8.137571734543144,
					24.309733035170552
				],
				[
					7.313506913641504,
					25.75183232584618
				],
				[
					6.695463013265908,
					26.884909666334124
				],
				[
					6.180439003755055,
					27.708974487235764
				],
				[
					5.8714170535672565,
					28.327018387611247
				],
				[
					5.459375212514942,
					28.842051827723708
				],
				[
					5.356374182853415,
					29.151073777911392
				],
				[
					5.047352232665617,
					29.46009572809919
				],
				[
					4.841331312139573,
					29.666107218023853
				],
				[
					4.738330282477818,
					29.975129168211538
				],
				[
					4.532309361951775,
					30.078139628474673
				],
				[
					4.532309361951775,
					29.975129168211538
				],
				[
					4.429308332290248,
					29.563106188362212
				],
				[
					4.429308332290248,
					28.842051827723708
				],
				[
					4.429308332290248,
					28.01799643742345
				],
				[
					4.326307302628493,
					26.987920126597146
				],
				[
					4.223287411763977,
					25.545820835921518
				],
				[
					4.120286382102449,
					24.309733035170552
				],
				[
					4.120286382102449,
					22.76462328423179
				],
				[
					4.120286382102449,
					21.219513533293025
				],
				[
					4.120286382102449,
					19.777404812015902
				],
				[
					4.326307302628493,
					17.820272081227813
				],
				[
					4.532309361951775,
					15.966140380101365
				],
				[
					5.047352232665617,
					13.905987758448646
				],
				[
					5.459375212514942,
					12.15486651758522
				],
				[
					5.76839716270274,
					10.197724356195636
				],
				[
					6.180439003755055,
					8.549613575595345
				],
				[
					6.489460953942853,
					7.107504854318222
				],
				[
					6.798482904130651,
					6.180439003754941
				],
				[
					7.004484963453706,
					5.459394073717931
				],
				[
					7.107504854318449,
					5.047361663267111
				],
				[
					7.210505883979977,
					4.8413501733423345
				],
				[
					7.313506913641504,
					4.8413501733423345
				],
				[
					7.5195278341675476,
					4.8413501733423345
				],
				[
					7.828549784355346,
					5.047361663267111
				],
				[
					8.240572764204671,
					5.3563836134547955
				],
				[
					8.54959471439247,
					5.7684160239056155
				],
				[
					8.961636555444784,
					6.2834494640180765
				],
				[
					9.270658505632582,
					6.798482904130424
				],
				[
					9.57968045582038,
					7.313525774844379
				],
				[
					9.682681485481908,
					7.931569675219862
				],
				[
					9.888702406008179,
					8.755625065520007
				],
				[
					10.094704465331233,
					9.78570137634631
				],
				[
					10.403726415519031,
					11.433812156946715
				],
				[
					10.609747336045075,
					12.875920878223837
				],
				[
					10.815768256571346,
					14.730052579350286
				],
				[
					10.918769286232873,
					16.79019577040151
				],
				[
					11.124790206759144,
					18.747337931791094
				],
				[
					11.124790206759144,
					20.189437222466722
				],
				[
					11.124790206759144,
					21.425525023217688
				],
				[
					11.124790206759144,
					21.94055846333015
				],
				[
					11.124790206759144,
					22.146579383856306
				],
				[
					11.124790206759144,
					21.94055846333015
				],
				[
					11.124790206759144,
					21.425525023217688
				],
				[
					11.124790206759144,
					20.91049158310534
				],
				[
					11.124790206759144,
					20.189437222466722
				],
				[
					11.124790206759144,
					19.365381832166577
				],
				[
					11.124790206759144,
					18.64432747152796
				],
				[
					11.124790206759144,
					17.92327311088934
				],
				[
					11.227791236420671,
					17.099217720589195
				],
				[
					11.433812156946715,
					16.481173820213712
				],
				[
					11.53681318660847,
					15.760119459575208
				],
				[
					11.742834107134513,
					15.039074529538084
				],
				[
					11.948836166457795,
					14.421030629162601
				],
				[
					12.154857086983839,
					13.802986728787118
				],
				[
					12.36087800751011,
					13.287943858073163
				],
				[
					12.463879037171637,
					12.875920878223837
				],
				[
					12.669899957697908,
					12.66989995769768
				],
				[
					12.669899957697908,
					12.56689892803604
				],
				[
					12.36087800751011,
					12.56689892803604
				],
				[
					11.948836166457795,
					12.56689892803604
				],
				[
					11.53681318660847,
					12.772910417960702
				],
				[
					11.227791236420671,
					13.287943858073163
				],
				[
					10.71274836570683,
					13.905987758448646
				],
				[
					10.19772435619575,
					14.524031658824128
				],
				[
					9.682681485481908,
					15.348096479725882
				],
				[
					9.064637585106311,
					16.27516233028905
				],
				[
					8.54959471439247,
					17.099217720589195
				],
				[
					8.240572764204671,
					17.717261620964678
				],
				[
					8.137571734543144,
					18.026283571152476
				],
				[
					7.9315508140171005,
					18.12929403141561
				],
				[
					7.828549784355346,
					18.12929403141561
				],
				[
					7.828549784355346,
					18.026283571152476
				],
				[
					8.034570704881617,
					17.717261620964678
				],
				[
					8.137571734543144,
					17.099217720589195
				],
				[
					8.240572764204671,
					16.584184280476848
				],
				[
					8.240572764204671,
					15.966140380101365
				],
				[
					8.240572764204671,
					15.245086019462747
				],
				[
					8.240572764204671,
					15.245086019462747
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 126,
			"versionNonce": 1348375536,
			"isDeleted": false,
			"id": "BCXK4MU-5G3XcJDnMRiSn",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3388.782833919586,
			"y": -433.19055379633926,
			"strokeColor": "#868e96",
			"backgroundColor": "transparent",
			"width": 21.940558463330262,
			"height": 4.429317762891515,
			"seed": 52167952,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.10300102966175473,
					0
				],
				[
					-0.3090219501877982,
					0
				],
				[
					-0.41202297984932557,
					0
				],
				[
					-0.5150240095108529,
					0
				],
				[
					-0.7210449300371238,
					0
				],
				[
					-0.8240459596986511,
					0
				],
				[
					-1.1330679098864493,
					-0.10301046026302174
				],
				[
					-1.4420898600742476,
					-0.20601148992466278
				],
				[
					-1.854131701126562,
					-0.5150334401123473
				],
				[
					-2.2661546809758875,
					-0.6180439003754827
				],
				[
					-2.678177660825213,
					-0.8240553903001455
				],
				[
					-3.1932205315390547,
					-1.1330773404879437
				],
				[
					-3.708263402253124,
					-1.2360878007509655
				],
				[
					-4.120286382102449,
					-1.4420992906756283
				],
				[
					-4.738330282477818,
					-1.6481202112017854
				],
				[
					-5.150353262327144,
					-1.8541317011264482
				],
				[
					-5.562395103379458,
					-1.9571421613895836
				],
				[
					-6.077419112890311,
					-2.060143191051111
				],
				[
					-6.695463013265908,
					-2.266164111577268
				],
				[
					-7.313506913641504,
					-2.369165141238909
				],
				[
					-7.931550814016873,
					-2.472175601501931
				],
				[
					-8.755615634918513,
					-2.781197551689729
				],
				[
					-9.476660564955637,
					-2.884208011952751
				],
				[
					-10.19772435619575,
					-3.193229962140549
				],
				[
					-10.918769286232873,
					-3.399241452065212
				],
				[
					-11.639814216269997,
					-3.399241452065212
				],
				[
					-12.154857086983839,
					-3.6052529419898747
				],
				[
					-12.772900987359208,
					-3.7082634022528964
				],
				[
					-12.978921907885479,
					-3.811273862516032
				],
				[
					-13.493945917396331,
					-3.914274892177673
				],
				[
					-13.80296786758413,
					-4.017285352440695
				],
				[
					-14.215009708636444,
					-4.017285352440695
				],
				[
					-14.421011767959726,
					-4.017285352440695
				],
				[
					-14.730033718147297,
					-4.12029581270383
				],
				[
					-15.039055668335095,
					-4.223296842365357
				],
				[
					-15.348077618522893,
					-4.223296842365357
				],
				[
					-15.760119459575208,
					-4.223296842365357
				],
				[
					-16.172142439424533,
					-4.326307302628493
				],
				[
					-16.58416541927386,
					-4.326307302628493
				],
				[
					-16.893187369461657,
					-4.326307302628493
				],
				[
					-17.30522921051397,
					-4.326307302628493
				],
				[
					-17.717252190363297,
					-4.326307302628493
				],
				[
					-18.026274140551095,
					-4.326307302628493
				],
				[
					-18.335296090738666,
					-4.429317762891515
				],
				[
					-18.43829712040042,
					-4.429317762891515
				],
				[
					-18.74731907058822,
					-4.429317762891515
				],
				[
					-18.850338961452735,
					-4.429317762891515
				],
				[
					-18.953339991114262,
					-4.429317762891515
				],
				[
					-19.159360911640533,
					-4.429317762891515
				],
				[
					-19.26236194130206,
					-4.429317762891515
				],
				[
					-19.365362970963588,
					-4.429317762891515
				],
				[
					-19.57138389148986,
					-4.429317762891515
				],
				[
					-19.674384921151386,
					-4.429317762891515
				],
				[
					-19.88040584167743,
					-4.429317762891515
				],
				[
					-20.0864267622037,
					-4.429317762891515
				],
				[
					-20.3954487123915,
					-4.326307302628493
				],
				[
					-20.601450771714553,
					-4.326307302628493
				],
				[
					-20.807471692240824,
					-4.223296842365357
				],
				[
					-21.013492612766868,
					-4.223296842365357
				],
				[
					-21.116493642428395,
					-4.12029581270383
				],
				[
					-21.21949467209015,
					-4.12029581270383
				],
				[
					-21.322514562954666,
					-4.12029581270383
				],
				[
					-21.425515592616193,
					-4.017285352440695
				],
				[
					-21.528516622277948,
					-3.914274892177673
				],
				[
					-21.631536513142464,
					-3.914274892177673
				],
				[
					-21.83753857246552,
					-3.811273862516032
				],
				[
					-21.940558463330262,
					-3.811273862516032
				],
				[
					-21.940558463330262,
					-3.7082634022528964
				],
				[
					-21.73453754280399,
					-3.7082634022528964
				],
				[
					-21.631536513142464,
					-3.7082634022528964
				],
				[
					-21.425515592616193,
					-3.811273862516032
				],
				[
					-21.322514562954666,
					-3.914274892177673
				],
				[
					-21.013492612766868,
					-3.914274892177673
				],
				[
					-20.807471692240824,
					-4.017285352440695
				],
				[
					-20.601450771714553,
					-4.12029581270383
				],
				[
					-20.189427791865228,
					-4.12029581270383
				],
				[
					-20.0864267622037,
					-4.223296842365357
				],
				[
					-19.777404812015902,
					-4.223296842365357
				],
				[
					-19.674384921151386,
					-4.223296842365357
				],
				[
					-19.26236194130206,
					-4.326307302628493
				],
				[
					-18.953339991114262,
					-4.326307302628493
				],
				[
					-18.541317011264937,
					-4.326307302628493
				],
				[
					-18.129275170212622,
					-4.326307302628493
				],
				[
					-17.30522921051397,
					-4.326307302628493
				],
				[
					-16.58416541927386,
					-4.326307302628493
				],
				[
					-16.48116438961233,
					-4.326307302628493
				],
				[
					-13.18492396720876,
					-4.326307302628493
				],
				[
					-13.081922937547006,
					-4.326307302628493
				],
				[
					-12.978921907885479,
					-4.326307302628493
				],
				[
					-12.051856057322311,
					-4.223296842365357
				],
				[
					-11.330792266082199,
					-4.12029581270383
				],
				[
					-10.712748365706602,
					-4.017285352440695
				],
				[
					-10.094704465331233,
					-3.914274892177673
				],
				[
					-9.682681485481908,
					-3.914274892177673
				],
				[
					-9.270658505632582,
					-3.7082634022528964
				],
				[
					-8.961636555444784,
					-3.7082634022528964
				],
				[
					-8.652614605256986,
					-3.5022519123283473
				],
				[
					-8.343592655069187,
					-3.5022519123283473
				],
				[
					-7.931550814016873,
					-3.399241452065212
				],
				[
					-7.622528863829075,
					-3.2962309918020765
				],
				[
					-7.210505883979749,
					-3.0902195018774137
				],
				[
					-6.9014839337921785,
					-2.884208011952751
				],
				[
					-6.489460953942853,
					-2.884208011952751
				],
				[
					-5.974418083228784,
					-2.6781870914265937
				],
				[
					-5.665396133041213,
					-2.472175601501931
				],
				[
					-5.356374182853415,
					-2.266164111577268
				],
				[
					-4.944351203004089,
					-2.266164111577268
				],
				[
					-4.532309361951775,
					-2.060143191051111
				],
				[
					-4.223287411763977,
					-1.9571421613895836
				],
				[
					-3.811264431914651,
					-1.7511212408634265
				],
				[
					-3.502242481726853,
					-1.7511212408634265
				],
				[
					-3.1932205315390547,
					-1.6481202112017854
				],
				[
					-2.9871996110130112,
					-1.5451097509387637
				],
				[
					-2.884198581351484,
					-1.5451097509387637
				],
				[
					-2.884198581351484,
					-1.4420992906756283
				],
				[
					-2.781197551689729,
					-1.339098261014101
				],
				[
					-2.678177660825213,
					-1.339098261014101
				],
				[
					-2.5751766311636857,
					-1.2360878007509655
				],
				[
					-2.369155710637415,
					-1.1330773404879437
				],
				[
					-2.2661546809758875,
					-1.1330773404879437
				],
				[
					-2.2661546809758875,
					-1.1330773404879437
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 32,
			"versionNonce": 1095144944,
			"isDeleted": false,
			"id": "-IA23rllWFpfYZ4NfBiC6",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3370.6526305624484,
			"y": -467.2980801637617,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 8.697631918653997,
			"height": 33.72006573162355,
			"seed": 1501094672,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.06690080877410765,
					0.3345224198479855
				],
				[
					-0.13381386819992258,
					0.46833628804779437
				],
				[
					-0.8697595166697738,
					3.9473866053790516
				],
				[
					-1.2711888706178343,
					5.620010955270573
				],
				[
					-1.6057174157915597,
					7.493349982136124
				],
				[
					-2.2747622554875306,
					9.901926105823463
				],
				[
					-2.943819345835209,
					12.377403038285024
				],
				[
					-3.61286418553118,
					15.053600773046242
				],
				[
					-4.415722893426846,
					17.863606250681528
				],
				[
					-5.285482410096847,
					20.874326405290844
				],
				[
					-6.021440309218406,
					23.55052414005206
				],
				[
					-6.757398208340192,
					26.15981494071343
				],
				[
					-7.29262917983624,
					28.233862519227046
				],
				[
					-7.760971593209888,
					29.973393803218414
				],
				[
					-8.095487887732133,
					31.110774930962293
				],
				[
					-8.229301755931829,
					32.11434831583199
				],
				[
					-8.296202564705936,
					32.71649234675385
				],
				[
					-8.363115624131751,
					33.05101476660184
				],
				[
					-8.363115624131751,
					33.318636377675716
				],
				[
					-8.363115624131751,
					33.385543311775564
				],
				[
					-8.430016432905859,
					33.45244412054967
				],
				[
					-8.496917241679967,
					33.45244412054967
				],
				[
					-8.563830301105781,
					33.51935105464963
				],
				[
					-8.63073110987989,
					33.586257988749594
				],
				[
					-8.697631918653997,
					33.6531587975237
				],
				[
					-8.697631918653997,
					33.72006573162355
				],
				[
					-8.697631918653997,
					33.72006573162355
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 33,
			"versionNonce": 434001904,
			"isDeleted": false,
			"id": "o5Ueww_3j6VlRM98Eq7lE",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3396.0095806699405,
			"y": -451.77614310266756,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.215008216453043,
			"height": 21.409563502112633,
			"seed": 1284112656,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.06690080877399396
				],
				[
					0,
					0.535237096821902
				],
				[
					0,
					1.1373811277437653
				],
				[
					0,
					1.8733329015395839
				],
				[
					0,
					3.010720154609203
				],
				[
					-0.1338016175482153,
					4.281909025226923
				],
				[
					-0.26761548574813787,
					5.48619708707065
				],
				[
					-0.5352309714962757,
					7.025013694088216
				],
				[
					-0.8028587078958935,
					8.764538852753844
				],
				[
					-1.137375002418139,
					10.370256268545404
				],
				[
					-1.5388043563659721,
					12.176688361310994
				],
				[
					-1.9402337103138052,
					13.648598034228485
				],
				[
					-2.274762255487758,
					15.321216258794266
				],
				[
					-2.5423777412356685,
					16.458603511863885
				],
				[
					-2.876906286409394,
					17.39526996263362
				],
				[
					-3.144521772157532,
					18.064320927655444
				],
				[
					-3.345236449131562,
					18.666464958577308
				],
				[
					-3.4790503173312572,
					19.13479512129925
				],
				[
					-3.6797649943052875,
					19.536224475247195
				],
				[
					-3.81357886250521,
					19.93765382919503
				],
				[
					-3.8804796712793177,
					20.339083183142975
				],
				[
					-4.01429353947924,
					20.606704794216853
				],
				[
					-4.0811943482531206,
					20.87432640529073
				],
				[
					-4.148095157027228,
					21.141941891038755
				],
				[
					-4.215008216453043,
					21.275755759238564
				],
				[
					-4.215008216453043,
					21.34265656801267
				],
				[
					-4.215008216453043,
					21.409563502112633
				],
				[
					-4.215008216453043,
					21.409563502112633
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 62,
			"versionNonce": 1311627760,
			"isDeleted": false,
			"id": "Zx2XTlXsiFGLsT-QlwKc7",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3362.3564279977427,
			"y": -431.8384892734724,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 29.170528969996667,
			"height": 8.229301755931942,
			"seed": 1002921744,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.20071467697380285,
					0.3345285451738391
				],
				[
					0.2676154857479105,
					0.46833628804790806
				],
				[
					0.4683301627219407,
					0.7359578991217859
				],
				[
					0.8697595166697738,
					1.271194995943688
				],
				[
					1.070474193643804,
					1.6057174157916734
				],
				[
					1.3380896793917145,
					1.9402459609653988
				],
				[
					1.739519033339775,
					2.2747683808133843
				],
				[
					2.0740475785135004,
					2.8100054776352863
				],
				[
					2.408576123687226,
					3.1445340228091254
				],
				[
					2.7430924182094714,
					3.479056442657111
				],
				[
					3.1445217721573044,
					3.8135788625050964
				],
				[
					3.6128641855309525,
					4.2150082164529294
				],
				[
					4.0811943482531206,
					4.549536761626769
				],
				[
					4.549524510975061,
					4.884059181474754
				],
				[
					5.218581601322512,
					5.151680792548632
				],
				[
					6.021440309218406,
					5.486203212396617
				],
				[
					7.025013694088102,
					5.820725632244603
				],
				[
					8.162388696506014,
					6.222154986192436
				],
				[
					9.634304494749586,
					6.690497399566198
				],
				[
					11.17310885111533,
					7.091926753514031
				],
				[
					12.578111589933087,
					7.292641430487947
				],
				[
					14.183829005724647,
					7.627157725010079
				],
				[
					15.722645612742099,
					7.8947854614098105
				],
				[
					17.127648351559856,
					8.028587078958026
				],
				[
					18.599551899151493,
					8.09550013838384
				],
				[
					19.937653829195142,
					8.229301755931942
				],
				[
					21.07504108226476,
					8.229301755931942
				],
				[
					22.078614467134457,
					8.229301755931942
				],
				[
					22.94837398380423,
					8.229301755931942
				],
				[
					23.818133500474232,
					8.229301755931942
				],
				[
					24.420277531396096,
					8.162400947157835
				],
				[
					24.95552075354385,
					8.09550013838384
				],
				[
					25.423850916265792,
					7.8947854614098105
				],
				[
					25.758379461439517,
					7.760971593210002
				],
				[
					26.09290800661347,
					7.694070784435894
				],
				[
					26.36052349236138,
					7.4933561074619774
				],
				[
					26.62813897810952,
					7.359542239262055
				],
				[
					26.962667523283244,
					7.225728371062246
				],
				[
					27.163382200257274,
					7.091926753514031
				],
				[
					27.364096877231077,
					6.891212076540114
				],
				[
					27.631712362979215,
					6.824299017114299
				],
				[
					27.765526231179138,
					6.623584340140383
				],
				[
					28.033141716927048,
					6.489782722592167
				],
				[
					28.23385639390108,
					6.3559688543923585
				],
				[
					28.367670262101,
					6.289061920292397
				],
				[
					28.43457107087511,
					6.088347243318481
				],
				[
					28.568384939074804,
					6.021440309218519
				],
				[
					28.63528574784891,
					5.820725632244603
				],
				[
					28.702198807274726,
					5.686917889370534
				],
				[
					28.769099616048834,
					5.553110146496579
				],
				[
					28.83600042482294,
					5.419296278296656
				],
				[
					28.969814293022864,
					5.285488535422701
				],
				[
					29.036715101796972,
					5.151680792548632
				],
				[
					29.036715101796972,
					5.017866924348823
				],
				[
					29.10362816122256,
					4.950966115574715
				],
				[
					29.170528969996667,
					4.884059181474754
				],
				[
					29.170528969996667,
					4.884059181474754
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 26,
			"versionNonce": 289217520,
			"isDeleted": false,
			"id": "v-QIAefWZHwwPThaUptsI",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3370.079170137507,
			"y": -467.91633006094173,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 11.771845571677659,
			"height": 2.2851246047720224,
			"seed": 1470692624,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.06924197369198737,
					0
				],
				[
					0.20773860043391323,
					0
				],
				[
					0.6924577749934997,
					0
				],
				[
					1.8003927508545985,
					0.2769869138047625
				],
				[
					2.0081313512882843,
					0.2769869138047625
				],
				[
					2.5621051788978093,
					0.484725514238562
				],
				[
					3.393059580633235,
					0.6924641146724753
				],
				[
					4.29325595606042,
					0.8309544017353119
				],
				[
					5.193465010845557,
					1.0386930021691114
				],
				[
					6.2321580130146685,
					1.246431602602911
				],
				[
					7.063112414749867,
					1.3849282293448368
				],
				[
					8.171047390610966,
					1.5926668297786364
				],
				[
					8.79426319191225,
					1.6619088034706238
				],
				[
					9.625217593647676,
					1.800405430212436
				],
				[
					10.109936768207263,
					1.800405430212436
				],
				[
					10.663910595816787,
					1.9388957172752725
				],
				[
					11.079387796684387,
					2.077386004338223
				],
				[
					11.494864997551986,
					2.146634317709186
				],
				[
					11.702603597985672,
					2.2851246047720224
				],
				[
					11.771845571677659,
					2.2851246047720224
				],
				[
					11.771845571677659,
					2.2851246047720224
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 20,
			"versionNonce": 1964252656,
			"isDeleted": false,
			"id": "50Mi_rj686CPyLHgBiNwO",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3395.8387565913004,
			"y": -453.1668894301407,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.146627978029983,
			"height": 7.963308790176939,
			"seed": 27712272,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.06924197369176,
					-0.20773860043379955
				],
				[
					0.20773860043368586,
					-0.692457774993386
				],
				[
					0.3462225478176606,
					-1.246431602602911
				],
				[
					0.623215801301285,
					-1.8696474039043096
				],
				[
					0.7616997486852597,
					-2.2158762914010595
				],
				[
					1.2464316026027973,
					-3.3930595806330075
				],
				[
					1.5234121767284705,
					-4.154772008676332
				],
				[
					1.7311507771623837,
					-5.054968384103518
				],
				[
					1.938889377596297,
					-5.816680812146842
				],
				[
					2.0081313512882843,
					-6.509138587140228
				],
				[
					2.0773860043379955,
					-7.063112414749753
				],
				[
					2.146627978029983,
					-7.5478315893093395
				],
				[
					2.146627978029983,
					-7.824818503114102
				],
				[
					2.146627978029983,
					-7.963308790176939
				],
				[
					2.146627978029983,
					-7.963308790176939
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 23,
			"versionNonce": 180019184,
			"isDeleted": false,
			"id": "3tizlXUXAELqJhsDlQ3iG",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3397.0851881939034,
			"y": -459.9530149310857,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.456184674740825,
			"height": 3.808543121179582,
			"seed": 741931280,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.20773860043391323,
					0
				],
				[
					-0.3462352271756117,
					-0.06924831337096293
				],
				[
					-0.8309544017351982,
					-0.20773860043379955
				],
				[
					-1.3849282293447231,
					-0.34622888749674985
				],
				[
					-2.077386004338223,
					-0.5539674879305494
				],
				[
					-2.9775950591233595,
					-0.9002027151061611
				],
				[
					-3.877791434550545,
					-1.246431602602911
				],
				[
					-5.054981063461582,
					-1.731157116841473
				],
				[
					-6.024419412580755,
					-2.2158762914010595
				],
				[
					-7.063112414749639,
					-2.562111518576785
				],
				[
					-8.10180541691875,
					-2.977588719444384
				],
				[
					-8.932759818654176,
					-3.32381760694102
				],
				[
					-9.6252302730054,
					-3.6008045207457826
				],
				[
					-10.040707473872999,
					-3.739294807808733
				],
				[
					-10.248446074306912,
					-3.739294807808733
				],
				[
					-10.3176880479989,
					-3.739294807808733
				],
				[
					-10.456184674740825,
					-3.808543121179582
				],
				[
					-10.456184674740825,
					-3.808543121179582
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "line",
			"version": 137,
			"versionNonce": 37315056,
			"isDeleted": false,
			"id": "_wtYC_CBAmyjjrXwF9BN3",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3297.0604836223984,
			"y": -560.1423609902578,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 69.88325682611548,
			"height": 121.04135142121709,
			"seed": 987191056,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-69.88325682611548,
					-121.04135142121709
				]
			]
		},
		{
			"type": "line",
			"version": 64,
			"versionNonce": 1251451888,
			"isDeleted": false,
			"id": "BM8ORMyRvkHBu_1CO7cuv",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3317.1793288083727,
			"y": -514.9218903408477,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 41.439150827236745,
			"height": 71.77471465528367,
			"seed": 1643771152,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					41.439150827236745,
					71.77471465528367
				]
			]
		},
		{
			"type": "freedraw",
			"version": 126,
			"versionNonce": 836609520,
			"isDeleted": false,
			"id": "HTFIF4pFRkOYnamJkb7GC",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.023682179613829568,
			"x": 3421.903502872374,
			"y": -958.5555984741139,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.9743589743589745,
			"height": 16.564102564102566,
			"seed": 119067408,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.8717948717948719
				],
				[
					0,
					1.7435897435897438
				],
				[
					0,
					2.615384615384616
				],
				[
					0,
					3.4871794871794877
				],
				[
					0.8717948717948718,
					3.4871794871794877
				],
				[
					0.8717948717948718,
					4.3589743589743595
				],
				[
					0.8717948717948718,
					5.230769230769232
				],
				[
					1.7435897435897436,
					5.230769230769232
				],
				[
					1.7435897435897436,
					6.102564102564103
				],
				[
					2.6153846153846154,
					6.974358974358975
				],
				[
					2.6153846153846154,
					7.846153846153848
				],
				[
					2.6153846153846154,
					8.717948717948719
				],
				[
					3.4871794871794872,
					10.461538461538463
				],
				[
					4.3589743589743595,
					12.205128205128206
				],
				[
					6.102564102564102,
					13.94871794871795
				],
				[
					6.102564102564102,
					14.820512820512823
				],
				[
					6.9743589743589745,
					15.692307692307695
				],
				[
					6.9743589743589745,
					16.564102564102566
				],
				[
					6.9743589743589745,
					16.564102564102566
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 124,
			"versionNonce": 85157872,
			"isDeleted": false,
			"id": "-88OQqoNZfhf5J_-AWG8P",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.023682179613829568,
			"x": 3438.5660588360333,
			"y": -962.5107911123299,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.846153846153847,
			"height": 16.564102564102566,
			"seed": 548139280,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.8717948717948719
				],
				[
					0,
					1.7435897435897438
				],
				[
					0,
					2.615384615384616
				],
				[
					0.8717948717948718,
					3.4871794871794877
				],
				[
					0.8717948717948718,
					4.3589743589743595
				],
				[
					1.7435897435897436,
					6.102564102564103
				],
				[
					2.6153846153846154,
					7.846153846153848
				],
				[
					3.4871794871794872,
					9.589743589743591
				],
				[
					4.3589743589743595,
					11.333333333333336
				],
				[
					5.230769230769231,
					12.205128205128206
				],
				[
					5.230769230769231,
					13.076923076923078
				],
				[
					6.102564102564102,
					14.820512820512823
				],
				[
					6.9743589743589745,
					14.820512820512823
				],
				[
					7.846153846153847,
					15.692307692307695
				],
				[
					7.846153846153847,
					16.564102564102566
				],
				[
					7.846153846153847,
					16.564102564102566
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 124,
			"versionNonce": 809560560,
			"isDeleted": false,
			"id": "BKaMyr4qJycVKYJCCOncm",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.023682179613829568,
			"x": 3431.8966383371653,
			"y": -929.4615628824005,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.948717948717949,
			"height": 1.7435897435897436,
			"seed": 371937040,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.8717948717948718,
					0
				],
				[
					1.7435897435897436,
					0
				],
				[
					2.6153846153846154,
					0
				],
				[
					3.4871794871794872,
					0
				],
				[
					4.3589743589743595,
					0
				],
				[
					5.230769230769231,
					0
				],
				[
					6.102564102564102,
					0
				],
				[
					6.9743589743589745,
					0
				],
				[
					7.846153846153847,
					0
				],
				[
					8.717948717948719,
					-0.8717948717948718
				],
				[
					9.58974358974359,
					-0.8717948717948718
				],
				[
					10.461538461538462,
					-1.7435897435897436
				],
				[
					11.333333333333334,
					-1.7435897435897436
				],
				[
					12.205128205128204,
					-1.7435897435897436
				],
				[
					13.076923076923077,
					-1.7435897435897436
				],
				[
					13.948717948717949,
					-1.7435897435897436
				],
				[
					13.948717948717949,
					-1.7435897435897436
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 138,
			"versionNonce": 1584278512,
			"isDeleted": false,
			"id": "uTPCgDn0pF9PW7u22c7Cc",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.023682179613829568,
			"x": 3431.9895366653245,
			"y": -929.4604628135393,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.948717948717949,
			"height": 9.58974358974359,
			"seed": 537849104,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.8717948717948718
				],
				[
					0,
					-1.7435897435897436
				],
				[
					0,
					-3.4871794871794872
				],
				[
					0,
					-4.3589743589743595
				],
				[
					0,
					-5.230769230769231
				],
				[
					0,
					-6.102564102564102
				],
				[
					0.8717948717948718,
					-6.102564102564102
				],
				[
					0.8717948717948718,
					-6.9743589743589745
				],
				[
					1.7435897435897436,
					-6.9743589743589745
				],
				[
					2.6153846153846154,
					-7.846153846153847
				],
				[
					3.4871794871794872,
					-7.846153846153847
				],
				[
					3.4871794871794872,
					-8.717948717948719
				],
				[
					4.3589743589743595,
					-8.717948717948719
				],
				[
					5.230769230769231,
					-9.58974358974359
				],
				[
					6.102564102564102,
					-9.58974358974359
				],
				[
					6.9743589743589745,
					-9.58974358974359
				],
				[
					7.846153846153847,
					-9.58974358974359
				],
				[
					9.58974358974359,
					-9.58974358974359
				],
				[
					10.461538461538462,
					-9.58974358974359
				],
				[
					11.333333333333334,
					-8.717948717948719
				],
				[
					11.333333333333334,
					-7.846153846153847
				],
				[
					12.205128205128204,
					-6.9743589743589745
				],
				[
					12.205128205128204,
					-6.102564102564102
				],
				[
					13.076923076923077,
					-6.102564102564102
				],
				[
					13.076923076923077,
					-5.230769230769231
				],
				[
					13.076923076923077,
					-4.3589743589743595
				],
				[
					13.948717948717949,
					-4.3589743589743595
				],
				[
					13.948717948717949,
					-3.4871794871794872
				],
				[
					13.948717948717949,
					-2.6153846153846154
				],
				[
					13.948717948717949,
					-1.7435897435897436
				],
				[
					13.948717948717949,
					-1.7435897435897436
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 299,
			"versionNonce": 430124528,
			"isDeleted": false,
			"id": "LLq4VTpK7-5ApweBq2ppb",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0.023682179613829568,
			"x": 3400.875738826194,
			"y": -966.2791101814568,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 68,
			"height": 67.12820512820512,
			"seed": 667863824,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.8717948717948717
				],
				[
					0,
					1.7435897435897434
				],
				[
					0,
					2.615384615384615
				],
				[
					0,
					3.487179487179487
				],
				[
					0,
					4.358974358974359
				],
				[
					0,
					5.23076923076923
				],
				[
					0,
					6.102564102564102
				],
				[
					0,
					6.974358974358974
				],
				[
					0.8717948717948718,
					6.974358974358974
				],
				[
					0.8717948717948718,
					7.846153846153845
				],
				[
					0.8717948717948718,
					8.717948717948717
				],
				[
					1.7435897435897436,
					9.58974358974359
				],
				[
					2.6153846153846154,
					10.46153846153846
				],
				[
					2.6153846153846154,
					11.333333333333332
				],
				[
					4.3589743589743595,
					15.69230769230769
				],
				[
					4.3589743589743595,
					16.564102564102562
				],
				[
					4.3589743589743595,
					17.435897435897434
				],
				[
					6.102564102564102,
					20.92307692307692
				],
				[
					6.9743589743589745,
					21.794871794871792
				],
				[
					8.717948717948719,
					26.15384615384615
				],
				[
					8.717948717948719,
					27.025641025641022
				],
				[
					8.717948717948719,
					27.897435897435894
				],
				[
					9.58974358974359,
					31.38461538461538
				],
				[
					10.461538461538462,
					33.99999999999999
				],
				[
					10.461538461538462,
					34.87179487179487
				],
				[
					11.333333333333334,
					37.48717948717948
				],
				[
					11.333333333333334,
					40.102564102564095
				],
				[
					12.205128205128204,
					42.717948717948715
				],
				[
					12.205128205128204,
					43.589743589743584
				],
				[
					13.076923076923077,
					44.46153846153846
				],
				[
					13.076923076923077,
					45.33333333333333
				],
				[
					13.076923076923077,
					46.2051282051282
				],
				[
					13.076923076923077,
					47.07692307692307
				],
				[
					13.076923076923077,
					47.94871794871794
				],
				[
					13.076923076923077,
					48.82051282051282
				],
				[
					13.076923076923077,
					49.692307692307686
				],
				[
					13.948717948717949,
					50.564102564102555
				],
				[
					13.948717948717949,
					51.43589743589743
				],
				[
					13.948717948717949,
					52.3076923076923
				],
				[
					13.948717948717949,
					53.179487179487175
				],
				[
					14.820512820512821,
					53.179487179487175
				],
				[
					15.692307692307693,
					53.179487179487175
				],
				[
					16.564102564102566,
					53.179487179487175
				],
				[
					17.435897435897438,
					53.179487179487175
				],
				[
					17.435897435897438,
					54.051282051282044
				],
				[
					18.307692307692307,
					54.051282051282044
				],
				[
					19.17948717948718,
					54.051282051282044
				],
				[
					20.05128205128205,
					54.051282051282044
				],
				[
					21.794871794871796,
					54.051282051282044
				],
				[
					23.53846153846154,
					54.051282051282044
				],
				[
					24.41025641025641,
					54.051282051282044
				],
				[
					27.897435897435898,
					54.051282051282044
				],
				[
					28.76923076923077,
					54.051282051282044
				],
				[
					29.641025641025642,
					54.051282051282044
				],
				[
					31.384615384615387,
					54.051282051282044
				],
				[
					32.256410256410255,
					54.051282051282044
				],
				[
					34,
					54.051282051282044
				],
				[
					37.48717948717949,
					52.3076923076923
				],
				[
					38.35897435897436,
					52.3076923076923
				],
				[
					39.23076923076923,
					52.3076923076923
				],
				[
					40.1025641025641,
					52.3076923076923
				],
				[
					40.97435897435898,
					51.43589743589743
				],
				[
					41.84615384615385,
					51.43589743589743
				],
				[
					42.717948717948715,
					51.43589743589743
				],
				[
					43.58974358974359,
					50.564102564102555
				],
				[
					44.46153846153846,
					50.564102564102555
				],
				[
					45.333333333333336,
					50.564102564102555
				],
				[
					46.205128205128204,
					50.564102564102555
				],
				[
					46.205128205128204,
					49.692307692307686
				],
				[
					47.94871794871795,
					48.82051282051282
				],
				[
					48.82051282051282,
					47.94871794871794
				],
				[
					49.69230769230769,
					47.94871794871794
				],
				[
					50.56410256410256,
					47.94871794871794
				],
				[
					51.43589743589744,
					47.07692307692307
				],
				[
					52.30769230769231,
					47.07692307692307
				],
				[
					53.17948717948718,
					47.07692307692307
				],
				[
					54.05128205128205,
					46.2051282051282
				],
				[
					54.05128205128205,
					45.33333333333333
				],
				[
					54.92307692307693,
					45.33333333333333
				],
				[
					55.794871794871796,
					44.46153846153846
				],
				[
					56.666666666666664,
					44.46153846153846
				],
				[
					58.41025641025641,
					43.589743589743584
				],
				[
					60.15384615384615,
					41.84615384615384
				],
				[
					61.02564102564103,
					41.84615384615384
				],
				[
					62.769230769230774,
					40.97435897435897
				],
				[
					63.64102564102564,
					40.97435897435897
				],
				[
					63.64102564102564,
					40.102564102564095
				],
				[
					63.64102564102564,
					39.230769230769226
				],
				[
					63.64102564102564,
					38.35897435897436
				],
				[
					63.64102564102564,
					37.48717948717948
				],
				[
					63.64102564102564,
					36.61538461538461
				],
				[
					63.64102564102564,
					35.74358974358974
				],
				[
					63.64102564102564,
					33.99999999999999
				],
				[
					63.64102564102564,
					33.128205128205124
				],
				[
					63.64102564102564,
					32.256410256410255
				],
				[
					63.64102564102564,
					31.38461538461538
				],
				[
					63.64102564102564,
					29.64102564102564
				],
				[
					63.64102564102564,
					28.769230769230766
				],
				[
					63.64102564102564,
					27.897435897435894
				],
				[
					63.64102564102564,
					27.025641025641022
				],
				[
					63.64102564102564,
					26.15384615384615
				],
				[
					63.64102564102564,
					24.41025641025641
				],
				[
					63.64102564102564,
					23.538461538461537
				],
				[
					63.64102564102564,
					22.666666666666664
				],
				[
					63.64102564102564,
					20.92307692307692
				],
				[
					63.64102564102564,
					20.051282051282048
				],
				[
					62.769230769230774,
					20.051282051282048
				],
				[
					62.769230769230774,
					19.17948717948718
				],
				[
					62.769230769230774,
					18.307692307692307
				],
				[
					62.769230769230774,
					17.435897435897434
				],
				[
					62.769230769230774,
					16.564102564102562
				],
				[
					62.769230769230774,
					15.69230769230769
				],
				[
					62.769230769230774,
					14.82051282051282
				],
				[
					62.769230769230774,
					13.948717948717947
				],
				[
					61.8974358974359,
					13.076923076923075
				],
				[
					61.8974358974359,
					11.333333333333332
				],
				[
					61.8974358974359,
					10.46153846153846
				],
				[
					61.8974358974359,
					9.58974358974359
				],
				[
					61.02564102564103,
					9.58974358974359
				],
				[
					61.02564102564103,
					8.717948717948717
				],
				[
					61.02564102564103,
					7.846153846153845
				],
				[
					61.02564102564103,
					6.974358974358974
				],
				[
					61.02564102564103,
					6.102564102564102
				],
				[
					60.15384615384615,
					5.23076923076923
				],
				[
					60.15384615384615,
					4.358974358974359
				],
				[
					60.15384615384615,
					3.487179487179487
				],
				[
					59.282051282051285,
					2.615384615384615
				],
				[
					59.282051282051285,
					1.7435897435897434
				],
				[
					59.282051282051285,
					0.8717948717948717
				],
				[
					58.41025641025641,
					0.8717948717948717
				],
				[
					58.41025641025641,
					-0.8717948717948717
				],
				[
					57.53846153846154,
					-2.615384615384615
				],
				[
					57.53846153846154,
					-4.358974358974359
				],
				[
					57.53846153846154,
					-6.102564102564102
				],
				[
					56.666666666666664,
					-7.846153846153845
				],
				[
					56.666666666666664,
					-9.58974358974359
				],
				[
					55.794871794871796,
					-10.46153846153846
				],
				[
					55.794871794871796,
					-11.333333333333332
				],
				[
					55.794871794871796,
					-12.205128205128204
				],
				[
					54.92307692307693,
					-12.205128205128204
				],
				[
					54.92307692307693,
					-13.076923076923075
				],
				[
					54.05128205128205,
					-13.076923076923075
				],
				[
					53.17948717948718,
					-13.076923076923075
				],
				[
					52.30769230769231,
					-13.076923076923075
				],
				[
					51.43589743589744,
					-13.076923076923075
				],
				[
					49.69230769230769,
					-13.076923076923075
				],
				[
					47.94871794871795,
					-13.076923076923075
				],
				[
					45.333333333333336,
					-13.076923076923075
				],
				[
					40.1025641025641,
					-11.333333333333332
				],
				[
					38.35897435897436,
					-10.46153846153846
				],
				[
					37.48717948717949,
					-10.46153846153846
				],
				[
					36.61538461538461,
					-10.46153846153846
				],
				[
					35.743589743589745,
					-10.46153846153846
				],
				[
					33.12820512820513,
					-9.58974358974359
				],
				[
					32.256410256410255,
					-9.58974358974359
				],
				[
					31.384615384615387,
					-8.717948717948717
				],
				[
					30.512820512820515,
					-8.717948717948717
				],
				[
					29.641025641025642,
					-8.717948717948717
				],
				[
					28.76923076923077,
					-8.717948717948717
				],
				[
					27.897435897435898,
					-7.846153846153845
				],
				[
					27.025641025641026,
					-7.846153846153845
				],
				[
					27.025641025641026,
					-6.974358974358974
				],
				[
					23.53846153846154,
					-6.974358974358974
				],
				[
					22.666666666666668,
					-6.102564102564102
				],
				[
					17.435897435897438,
					-4.358974358974359
				],
				[
					16.564102564102566,
					-4.358974358974359
				],
				[
					15.692307692307693,
					-4.358974358974359
				],
				[
					14.820512820512821,
					-4.358974358974359
				],
				[
					13.948717948717949,
					-4.358974358974359
				],
				[
					13.076923076923077,
					-4.358974358974359
				],
				[
					12.205128205128204,
					-4.358974358974359
				],
				[
					10.461538461538462,
					-4.358974358974359
				],
				[
					9.58974358974359,
					-4.358974358974359
				],
				[
					9.58974358974359,
					-3.487179487179487
				],
				[
					8.717948717948719,
					-3.487179487179487
				],
				[
					7.846153846153847,
					-3.487179487179487
				],
				[
					6.9743589743589745,
					-3.487179487179487
				],
				[
					6.102564102564102,
					-3.487179487179487
				],
				[
					4.3589743589743595,
					-3.487179487179487
				],
				[
					3.4871794871794872,
					-3.487179487179487
				],
				[
					2.6153846153846154,
					-2.615384615384615
				],
				[
					0.8717948717948718,
					-2.615384615384615
				],
				[
					0.8717948717948718,
					-1.7435897435897434
				],
				[
					0,
					-1.7435897435897434
				],
				[
					-0.8717948717948718,
					-0.8717948717948717
				],
				[
					-1.7435897435897436,
					-0.8717948717948717
				],
				[
					-2.6153846153846154,
					-0.8717948717948717
				],
				[
					-2.6153846153846154,
					0
				],
				[
					-3.4871794871794872,
					0
				],
				[
					-4.3589743589743595,
					0
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
			"version": 89,
			"versionNonce": 1793585136,
			"isDeleted": false,
			"id": "cpeEelkqB5Bys2sGT0H5-",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2945.7644933423107,
			"y": -737.5545238556477,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 441.9999999999998,
			"height": 132,
			"seed": 669182224,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
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
					0
				],
				[
					8,
					0
				],
				[
					18,
					-4
				],
				[
					30,
					-10
				],
				[
					32,
					-12
				],
				[
					42,
					-16
				],
				[
					54,
					-22
				],
				[
					82,
					-32
				],
				[
					90,
					-34
				],
				[
					108,
					-38
				],
				[
					140,
					-46
				],
				[
					154,
					-50
				],
				[
					168,
					-52
				],
				[
					212,
					-60
				],
				[
					214,
					-62
				],
				[
					220,
					-64
				],
				[
					242,
					-68
				],
				[
					244,
					-70
				],
				[
					258,
					-74
				],
				[
					264,
					-76
				],
				[
					266,
					-76
				],
				[
					268,
					-78
				],
				[
					278,
					-80
				],
				[
					280,
					-82
				],
				[
					282,
					-82
				],
				[
					290,
					-82
				],
				[
					292,
					-84
				],
				[
					298,
					-84
				],
				[
					302,
					-84
				],
				[
					316,
					-86
				],
				[
					320,
					-86
				],
				[
					342,
					-90
				],
				[
					356,
					-94
				],
				[
					358,
					-94
				],
				[
					363.9999999999998,
					-94
				],
				[
					369.9999999999998,
					-96
				],
				[
					379.9999999999998,
					-100
				],
				[
					385.9999999999998,
					-102
				],
				[
					387.9999999999998,
					-104
				],
				[
					395.9999999999998,
					-108
				],
				[
					399.9999999999998,
					-110
				],
				[
					403.9999999999998,
					-110
				],
				[
					413.9999999999998,
					-116
				],
				[
					423.9999999999998,
					-120
				],
				[
					423.9999999999998,
					-122
				],
				[
					425.9999999999998,
					-122
				],
				[
					429.9999999999998,
					-124
				],
				[
					431.9999999999998,
					-126
				],
				[
					433.9999999999998,
					-126
				],
				[
					437.9999999999998,
					-130
				],
				[
					439.9999999999998,
					-132
				],
				[
					441.9999999999998,
					-132
				],
				[
					441.9999999999998,
					-132
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 120,
			"versionNonce": 2051305968,
			"isDeleted": false,
			"id": "NMSfuVsX5_xrwwcWU_iDg",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3317.7644933423107,
			"y": -835.5545238556477,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 441.9999999999998,
			"height": 132,
			"seed": 197347088,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
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
					0
				],
				[
					8,
					0
				],
				[
					18,
					-4
				],
				[
					30,
					-10
				],
				[
					32,
					-12
				],
				[
					42,
					-16
				],
				[
					54,
					-22
				],
				[
					82,
					-32
				],
				[
					90,
					-34
				],
				[
					108,
					-38
				],
				[
					140,
					-46
				],
				[
					154,
					-50
				],
				[
					168,
					-52
				],
				[
					212,
					-60
				],
				[
					214,
					-62
				],
				[
					220,
					-64
				],
				[
					242,
					-68
				],
				[
					244,
					-70
				],
				[
					258,
					-74
				],
				[
					264,
					-76
				],
				[
					266,
					-76
				],
				[
					268,
					-78
				],
				[
					278,
					-80
				],
				[
					280,
					-82
				],
				[
					282,
					-82
				],
				[
					290,
					-82
				],
				[
					292,
					-84
				],
				[
					298,
					-84
				],
				[
					302,
					-84
				],
				[
					316,
					-86
				],
				[
					320,
					-86
				],
				[
					342,
					-90
				],
				[
					356,
					-94
				],
				[
					358,
					-94
				],
				[
					363.9999999999998,
					-94
				],
				[
					369.9999999999998,
					-96
				],
				[
					379.9999999999998,
					-100
				],
				[
					385.9999999999998,
					-102
				],
				[
					387.9999999999998,
					-104
				],
				[
					395.9999999999998,
					-108
				],
				[
					399.9999999999998,
					-110
				],
				[
					403.9999999999998,
					-110
				],
				[
					413.9999999999998,
					-116
				],
				[
					423.9999999999998,
					-120
				],
				[
					423.9999999999998,
					-122
				],
				[
					425.9999999999998,
					-122
				],
				[
					429.9999999999998,
					-124
				],
				[
					431.9999999999998,
					-126
				],
				[
					433.9999999999998,
					-126
				],
				[
					437.9999999999998,
					-130
				],
				[
					439.9999999999998,
					-132
				],
				[
					441.9999999999998,
					-132
				],
				[
					441.9999999999998,
					-132
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 32,
			"versionNonce": 784380912,
			"isDeleted": false,
			"id": "L4FXHsIFkEtB80XaM6cYF",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3430.7116520190184,
			"y": -197.01129343629248,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 56.327451718831526,
			"height": 132.89750459913807,
			"seed": 266855696,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.4400714362218423
				],
				[
					0,
					-0.880102583930011
				],
				[
					0,
					-1.760245456373923
				],
				[
					-1.3201740201520806,
					-3.960522060456242
				],
				[
					-2.20031689259622,
					-6.600870100760403
				],
				[
					-3.960522060456242,
					-10.561392161216645
				],
				[
					-6.160838953052462,
					-14.96198565789473
				],
				[
					-8.801186993356623,
					-20.24268173850305
				],
				[
					-11.441535033660784,
					-27.283582986971624
				],
				[
					-15.402057094117026,
					-36.52480112803619
				],
				[
					-18.922467429837525,
					-44.44584524894867
				],
				[
					-23.32310121502951,
					-54.56720626245715
				],
				[
					-28.603797295637833,
					-64.68852698745195
				],
				[
					-33.004350503802016,
					-75.68999058489044
				],
				[
					-36.96487256425826,
					-85.37123987366317
				],
				[
					-41.365425772422896,
					-93.73235543079761
				],
				[
					-44.88591668517074,
					-102.53350213564022
				],
				[
					-47.5262647254749,
					-109.13437223640062
				],
				[
					-49.28646989333538,
					-114.41506831700895
				],
				[
					-51.486786785931145,
					-119.69576439761727
				],
				[
					-52.366929658375284,
					-122.33611243792143
				],
				[
					-53.687103678527365,
					-126.29663449837767
				],
				[
					-54.5671659739437,
					-128.0568799547517
				],
				[
					-55.007277698679445,
					-130.2571565588339
				],
				[
					-55.88733999409578,
					-132.01740201520795
				],
				[
					-56.327451718831526,
					-132.89750459913807
				],
				[
					-56.327451718831526,
					-132.89750459913807
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 265,
			"versionNonce": 1315223024,
			"isDeleted": false,
			"id": "Z9-G1zK9tVEQDmvjJ8-Lu",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 4.970641200195729,
			"x": 2343.7644933423117,
			"y": -809.5545238556477,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 441.9999999999998,
			"height": 132,
			"seed": 566805264,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
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
					0
				],
				[
					8,
					0
				],
				[
					18,
					-4
				],
				[
					30,
					-10
				],
				[
					32,
					-12
				],
				[
					42,
					-16
				],
				[
					54,
					-22
				],
				[
					82,
					-32
				],
				[
					90,
					-34
				],
				[
					108,
					-38
				],
				[
					140,
					-46
				],
				[
					154,
					-50
				],
				[
					168,
					-52
				],
				[
					212,
					-60
				],
				[
					214,
					-62
				],
				[
					220,
					-64
				],
				[
					242,
					-68
				],
				[
					244,
					-70
				],
				[
					258,
					-74
				],
				[
					264,
					-76
				],
				[
					266,
					-76
				],
				[
					268,
					-78
				],
				[
					278,
					-80
				],
				[
					280,
					-82
				],
				[
					282,
					-82
				],
				[
					290,
					-82
				],
				[
					292,
					-84
				],
				[
					298,
					-84
				],
				[
					302,
					-84
				],
				[
					316,
					-86
				],
				[
					320,
					-86
				],
				[
					342,
					-90
				],
				[
					356,
					-94
				],
				[
					358,
					-94
				],
				[
					363.9999999999998,
					-94
				],
				[
					369.9999999999998,
					-96
				],
				[
					379.9999999999998,
					-100
				],
				[
					385.9999999999998,
					-102
				],
				[
					387.9999999999998,
					-104
				],
				[
					395.9999999999998,
					-108
				],
				[
					399.9999999999998,
					-110
				],
				[
					403.9999999999998,
					-110
				],
				[
					413.9999999999998,
					-116
				],
				[
					423.9999999999998,
					-120
				],
				[
					423.9999999999998,
					-122
				],
				[
					425.9999999999998,
					-122
				],
				[
					429.9999999999998,
					-124
				],
				[
					431.9999999999998,
					-126
				],
				[
					433.9999999999998,
					-126
				],
				[
					437.9999999999998,
					-130
				],
				[
					439.9999999999998,
					-132
				],
				[
					441.9999999999998,
					-132
				],
				[
					441.9999999999998,
					-132
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 61,
			"versionNonce": 507017200,
			"isDeleted": false,
			"id": "5bJHdozS8tkgS_9l960-5",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3237.5262139291062,
			"y": -119.56109768354179,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 134.21763833077625,
			"height": 217.38864188887112,
			"seed": 1071505680,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.44003114770816865
				],
				[
					0,
					-1.3201740201520806
				],
				[
					0.44003114770816865,
					-2.6403480403041613
				],
				[
					1.3201740201520806,
					-3.960522060456242
				],
				[
					2.200236315568418,
					-5.720727228316491
				],
				[
					2.6403480403041613,
					-7.480932396176513
				],
				[
					4.840584355872579,
					-11.001423308924814
				],
				[
					6.600870100760403,
					-13.641771349228975
				],
				[
					8.361075268620652,
					-16.282119389533136
				],
				[
					10.561392161216645,
					-20.24264144998915
				],
				[
					14.081802496937144,
					-25.083306382889532
				],
				[
					18.48243628212913,
					-30.364002463497627
				],
				[
					23.323020638001708,
					-35.64469854410595
				],
				[
					29.043828443345774,
					-43.56574266501843
				],
				[
					36.96487256425826,
					-52.366889369861156
				],
				[
					41.80545692013084,
					-58.08765688669132
				],
				[
					49.28646989333515,
					-66.0087010076038
				],
				[
					56.327371141803724,
					-74.80984771244653
				],
				[
					63.80838411500804,
					-84.05106585351109
				],
				[
					71.28939708821235,
					-92.85221255835359
				],
				[
					77.45015546423701,
					-101.65339955170998
				],
				[
					83.17096326958108,
					-110.4545462565527
				],
				[
					88.01154762545343,
					-119.69576439761727
				],
				[
					92.85221255835381,
					-128.49691110245976
				],
				[
					97.69287749125397,
					-137.73812924352433
				],
				[
					100.7732566792663,
					-144.7790707805068
				],
				[
					105.61392161216645,
					-154.02028892157136
				],
				[
					109.13433194788672,
					-162.82143562641386
				],
				[
					111.77467998819088,
					-168.9822745794661
				],
				[
					115.73520204864712,
					-177.7834212843087
				],
				[
					117.93551894124334,
					-182.1840147809869
				],
				[
					121.01589812925545,
					-187.46471086159522
				],
				[
					123.65624616955961,
					-191.86526406975963
				],
				[
					124.97642018971169,
					-195.3857549825077
				],
				[
					126.29659420986377,
					-197.5860315865899
				],
				[
					127.61676823001585,
					-199.78630819067212
				],
				[
					127.61676823001585,
					-201.9866250832681
				],
				[
					128.49691110246,
					-202.86672766719823
				],
				[
					128.49691110246,
					-204.62697312357227
				],
				[
					128.93694225016793,
					-205.94714714372435
				],
				[
					129.37705397490367,
					-206.82724972765448
				],
				[
					129.81708512261207,
					-208.5874951840285
				],
				[
					130.25711627032,
					-209.9076692041806
				],
				[
					130.25711627032,
					-211.22784322433267
				],
				[
					131.13725914276415,
					-212.1079458082628
				],
				[
					131.5772902904721,
					-213.42811982841488
				],
				[
					132.01740201520784,
					-214.308222412345
				],
				[
					132.45743316291623,
					-214.74829384856696
				],
				[
					132.89746431062417,
					-215.18836528478892
				],
				[
					132.89746431062417,
					-215.62839643249708
				],
				[
					132.89746431062417,
					-216.06846786871904
				],
				[
					132.89746431062417,
					-216.508539304941
				],
				[
					133.33757603535992,
					-216.94857045264916
				],
				[
					133.7776071830683,
					-217.38864188887112
				],
				[
					134.21763833077625,
					-217.38864188887112
				],
				[
					134.21763833077625,
					-217.38864188887112
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 15,
			"versionNonce": 38009328,
			"isDeleted": false,
			"id": "HI6UVukAeODgcGTZgfAeF",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3371.7438522598827,
			"y": -336.9497395724128,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.2806960806083225,
			"height": 16.282159678046924,
			"seed": 1503608592,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.440071436221956
				],
				[
					0.44011172473574334,
					2.2002766040822053
				],
				[
					0.8801428724441394,
					4.400593496678198
				],
				[
					0.8801428724441394,
					7.480972684690528
				],
				[
					2.20031689259622,
					9.68128957728652
				],
				[
					3.0804597650399046,
					11.881566181368726
				],
				[
					3.960522060456242,
					14.081842785450931
				],
				[
					4.840664932900381,
					15.402016805603012
				],
				[
					5.2806960806083225,
					16.282159678046924
				],
				[
					5.2806960806083225,
					16.282159678046924
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 326,
			"versionNonce": 495926256,
			"isDeleted": false,
			"id": "lLjb5yXJYEZeSAZfkDk4z",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3368.223441924162,
			"y": -336.9497395724128,
			"strokeColor": "#a18072",
			"backgroundColor": "transparent",
			"width": 195.3857549825077,
			"height": 216.94861074116295,
			"seed": 797236496,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.440071436221956
				],
				[
					-0.44011172473574334,
					1.3201740201520806
				],
				[
					-0.8801428724436846,
					2.2002766040822053
				],
				[
					-0.8801428724436846,
					3.0804194765261173
				],
				[
					-1.3201740201520806,
					4.400593496678198
				],
				[
					-1.3201740201520806,
					5.2806960806083225
				],
				[
					-1.760285744887824,
					6.600870100760403
				],
				[
					-1.760285744887824,
					7.480972684690528
				],
				[
					-2.2003168925957652,
					8.801146704842608
				],
				[
					-2.2003168925957652,
					10.121320724994689
				],
				[
					-2.6403480403041613,
					11.881566181368726
				],
				[
					-2.6403480403041613,
					13.201740201520806
				],
				[
					-3.0804597650399046,
					14.961985657894843
				],
				[
					-3.0804597650399046,
					16.282159678046924
				],
				[
					-3.0804597650399046,
					18.042364845907173
				],
				[
					-3.0804597650399046,
					18.922507718351085
				],
				[
					-3.520490912747846,
					20.682712886211334
				],
				[
					-3.520490912747846,
					22.44295834258537
				],
				[
					-3.960522060456242,
					23.76313236273745
				],
				[
					-4.400633785191985,
					25.523377819111488
				],
				[
					-4.8406649328999265,
					27.283582986971737
				],
				[
					-4.8406649328999265,
					29.043828443345774
				],
				[
					-5.720807805344066,
					30.80407389971981
				],
				[
					-5.720807805344066,
					32.56427906758006
				],
				[
					-5.720807805344066,
					33.88445308773214
				],
				[
					-6.160838953052007,
					35.64469854410618
				],
				[
					-6.600870100760403,
					36.96487256425826
				],
				[
					-6.600870100760403,
					38.28504658441034
				],
				[
					-7.481012973204088,
					40.045292040784375
				],
				[
					-7.921044120912484,
					41.805497208644624
				],
				[
					-8.361155845648227,
					43.56574266501866
				],
				[
					-8.361155845648227,
					45.3259881213927
				],
				[
					-8.801186993356168,
					47.08619328925295
				],
				[
					-9.681329865800308,
					48.84643874562698
				],
				[
					-10.121361013508249,
					51.04671534970919
				],
				[
					-11.001503885952388,
					52.806960806083225
				],
				[
					-11.881566181368726,
					54.127134826235306
				],
				[
					-12.76170905381241,
					56.32741143031751
				],
				[
					-13.201740201520806,
					57.64758545046959
				],
				[
					-13.64185192625655,
					59.40783090684363
				],
				[
					-13.64185192625655,
					60.72800492699571
				],
				[
					-14.96202594640863,
					62.488250383369746
				],
				[
					-15.402057094116572,
					63.808424403521826
				],
				[
					-15.842088241824968,
					65.56862957138208
				],
				[
					-16.722231114268652,
					67.328875027756
				],
				[
					-17.60237398671279,
					68.64904904790808
				],
				[
					-18.48243628212913,
					69.96922306806016
				],
				[
					-18.922548006864872,
					71.72946852443431
				],
				[
					-20.242722027016953,
					73.48967369229456
				],
				[
					-21.12278432243329,
					75.24991914866848
				],
				[
					-22.002927194876975,
					77.4501957527508
				],
				[
					-23.323101215029055,
					79.21044120912472
				],
				[
					-24.203244087473195,
					80.97068666549887
				],
				[
					-25.523418107625275,
					82.73089183335912
				],
				[
					-26.403480403041385,
					85.37123987366328
				],
				[
					-27.723654423193466,
					87.13148533003721
				],
				[
					-28.603797295637378,
					88.45165935018929
				],
				[
					-29.483940168081517,
					91.09200739049345
				],
				[
					-30.804114188233598,
					92.8522528468676
				],
				[
					-32.12428820838568,
					94.17242686701968
				],
				[
					-33.00435050380179,
					96.81277490732384
				],
				[
					-34.32452452395387,
					98.57298007518409
				],
				[
					-35.20466739639778,
					100.77329696778008
				],
				[
					-36.96487256425803,
					102.97357357186218
				],
				[
					-38.28504658441011,
					105.1738501759445
				],
				[
					-40.04533232929816,
					107.81419821624866
				],
				[
					-41.36550634945024,
					110.45454625655282
				],
				[
					-42.68568036960232,
					112.65486314914881
				],
				[
					-44.445885537462345,
					115.29521118945297
				],
				[
					-45.326028409906485,
					117.49548779353506
				],
				[
					-47.08623357776651,
					119.69576439761738
				],
				[
					-48.40640759791859,
					121.4560098539913
				],
				[
					-49.72658161807067,
					124.09635789429547
				],
				[
					-50.60672449051458,
					125.41653191444755
				],
				[
					-51.48678678593092,
					126.73670593459963
				],
				[
					-52.806960806083,
					128.93698253868195
				],
				[
					-53.68710367852691,
					130.25715655883403
				],
				[
					-55.00727769867899,
					131.5773305789861
				],
				[
					-55.8874205711229,
					132.8975045991382
				],
				[
					-57.20759459127498,
					134.6577500555121
				],
				[
					-58.527768611427064,
					136.41799551188626
				],
				[
					-60.72800492699548,
					138.1782006797465
				],
				[
					-62.04817894714756,
					139.93844613612043
				],
				[
					-64.68852698745172,
					143.01886561264666
				],
				[
					-66.0087010076038,
					144.33903963279874
				],
				[
					-67.76898675249163,
					146.53931623688084
				],
				[
					-69.52919192035188,
					148.73959284096316
				],
				[
					-70.84936594050396,
					150.49983829733708
				],
				[
					-72.16953996065604,
					152.7001149014194
				],
				[
					-73.92974512851629,
					154.46036035779332
				],
				[
					-75.24991914866837,
					156.22060581416747
				],
				[
					-76.57009316882045,
					158.42088241824956
				],
				[
					-77.89026718897253,
					160.62115902233188
				],
				[
					-80.09058408156852,
					161.94133304248396
				],
				[
					-81.85078924942877,
					164.14164993507995
				],
				[
					-85.37128016217684,
					167.22202912309228
				],
				[
					-88.45165935018917,
					169.86237716339645
				],
				[
					-91.97215026293725,
					172.94279663992245
				],
				[
					-96.37270347110166,
					176.02321611644868
				],
				[
					-99.01305151140582,
					177.78342128430893
				],
				[
					-102.97357357186206,
					180.4237693246131
				],
				[
					-105.61392161216622,
					182.62408621720908
				],
				[
					-107.81423850476222,
					184.38429138506933
				],
				[
					-108.69438137720613,
					185.7044654052214
				],
				[
					-110.01455539735821,
					187.0246394253735
				],
				[
					-110.89461769277455,
					187.9047822978174
				],
				[
					-111.33472941751029,
					188.78488488174742
				],
				[
					-111.77476056521846,
					189.2249563179695
				],
				[
					-112.21479171292663,
					189.66498746567743
				],
				[
					-112.65490343766237,
					190.54513033812157
				],
				[
					-113.09493458537054,
					191.42527321056548
				],
				[
					-113.5349657330787,
					191.86530435827365
				],
				[
					-113.97507745781445,
					193.18547837842573
				],
				[
					-114.85513975323079,
					194.5056523985778
				],
				[
					-116.17531377338287,
					195.38579527102172
				],
				[
					-116.61542549811861,
					196.7059692911738
				],
				[
					-117.49548779353495,
					197.14600043888197
				],
				[
					-118.37563066597886,
					197.5860315865899
				],
				[
					-118.37563066597886,
					198.02614331132588
				],
				[
					-118.37563066597886,
					198.46617445903405
				],
				[
					-118.81566181368703,
					198.906205606742
				],
				[
					-119.25577353842277,
					199.34631733147796
				],
				[
					-119.69580468613094,
					199.78634847918613
				],
				[
					-120.57594755857485,
					200.22637962689407
				],
				[
					-121.01597870628302,
					201.10652249933798
				],
				[
					-121.45600985399119,
					202.42669651949006
				],
				[
					-122.3361527264351,
					202.86672766719823
				],
				[
					-122.77618387414327,
					203.74687053964215
				],
				[
					-122.77618387414327,
					204.1869016873503
				],
				[
					-123.21629559887901,
					204.1869016873503
				],
				[
					-123.65632674658718,
					204.62701341208628
				],
				[
					-124.09635789429535,
					205.06704455979423
				],
				[
					-124.5364696190311,
					205.94718743223837
				],
				[
					-124.97650076673926,
					206.3872185799463
				],
				[
					-125.41653191444743,
					206.82724972765448
				],
				[
					-125.85664363918318,
					206.82724972765448
				],
				[
					-125.85664363918318,
					207.26736145239045
				],
				[
					-126.29667478689134,
					207.26736145239045
				],
				[
					-126.29667478689134,
					207.7073926000984
				],
				[
					-127.17681765933526,
					208.14742374780656
				],
				[
					-128.9370228271955,
					209.9077094926946
				],
				[
					-128.9370228271955,
					210.34774064040255
				],
				[
					-128.9370228271955,
					210.78777178811072
				],
				[
					-128.9370228271955,
					211.2278835128467
				],
				[
					-128.9370228271955,
					211.66791466055463
				],
				[
					-129.37705397490367,
					212.1079458082628
				],
				[
					-129.37705397490367,
					212.54805753299854
				],
				[
					-129.37705397490367,
					212.9880886807067
				],
				[
					-129.37705397490367,
					213.42811982841488
				],
				[
					-129.81716569963942,
					214.3082627008588
				],
				[
					-129.81716569963942,
					214.74829384856696
				],
				[
					-129.81716569963942,
					215.1884055733027
				],
				[
					-129.81716569963942,
					215.62843672101087
				],
				[
					-130.2571968473476,
					216.06846786871904
				],
				[
					-130.2571968473476,
					216.50857959345478
				],
				[
					-130.69722799505575,
					216.50857959345478
				],
				[
					-130.69722799505575,
					216.94861074116295
				],
				[
					-129.81716569963942,
					216.94861074116295
				],
				[
					-129.37705397490367,
					216.94861074116295
				],
				[
					-128.9370228271955,
					216.94861074116295
				],
				[
					-128.49699167948734,
					216.94861074116295
				],
				[
					-128.0568799547516,
					216.94861074116295
				],
				[
					-127.61684880704343,
					216.94861074116295
				],
				[
					-127.17681765933526,
					216.50857959345478
				],
				[
					-126.73670593459951,
					216.50857959345478
				],
				[
					-125.41653191444743,
					216.50857959345478
				],
				[
					-124.09635789429535,
					216.06846786871904
				],
				[
					-123.21629559887901,
					215.62843672101087
				],
				[
					-121.45600985399119,
					215.62843672101087
				],
				[
					-120.13583583383911,
					215.1884055733027
				],
				[
					-118.37563066597886,
					214.74829384856696
				],
				[
					-116.61542549811861,
					213.86823155315062
				],
				[
					-114.85513975323079,
					213.42811982841488
				],
				[
					-113.09493458537054,
					212.9880886807067
				],
				[
					-111.77476056521846,
					212.1079458082628
				],
				[
					-110.45458654506638,
					211.2278835128467
				],
				[
					-108.69438137720613,
					210.34774064040255
				],
				[
					-107.81423850476222,
					209.9077094926946
				],
				[
					-106.05403333690197,
					209.46759776795864
				],
				[
					-104.29374759201414,
					208.58753547254253
				],
				[
					-102.5335424241539,
					207.7073926000984
				],
				[
					-99.89319438384973,
					206.82724972765448
				],
				[
					-96.8128151958374,
					205.5070757075024
				],
				[
					-93.29232428308933,
					205.06704455979423
				],
				[
					-89.77183337034126,
					203.74687053964215
				],
				[
					-85.81131130988501,
					202.42669651949006
				],
				[
					-82.73093212187268,
					201.98666537178212
				],
				[
					-78.77041006141644,
					200.66649135163004
				],
				[
					-75.24991914866837,
					199.78634847918613
				],
				[
					-72.16953996065604,
					198.906205606742
				],
				[
					-68.2090179001998,
					197.5860315865899
				],
				[
					-64.24849583974355,
					195.8258264187299
				],
				[
					-62.04817894714756,
					194.94568354628575
				],
				[
					-58.527768611427064,
					193.18547837842573
				],
				[
					-55.44730884638716,
					191.86530435827365
				],
				[
					-51.48678678593092,
					190.1050589018995
				],
				[
					-47.96637645021042,
					189.2249563179695
				],
				[
					-44.445885537462345,
					187.46471086159534
				],
				[
					-40.4853634770061,
					186.14453684144326
				],
				[
					-37.404984288994,
					185.26443425751324
				],
				[
					-34.32452452395387,
					183.94426023736116
				],
				[
					-31.24414533594154,
					183.06411736491725
				],
				[
					-28.163766147929437,
					182.184014780987
				],
				[
					-26.403480403041385,
					181.303912197057
				],
				[
					-23.763132362737224,
					180.86384076083493
				],
				[
					-21.12278432243329,
					179.98373817690492
				],
				[
					-18.48243628212913,
					179.103595304461
				],
				[
					-15.842088241824968,
					178.22349272053077
				],
				[
					-13.201740201520806,
					177.34339013660076
				],
				[
					-9.681329865800308,
					176.02321611644868
				],
				[
					-6.160838953052007,
					175.14307324400477
				],
				[
					-2.6403480403041613,
					173.8228992238527
				],
				[
					1.7602051678604766,
					172.5027252037006
				],
				[
					5.2806960806083225,
					171.18255118354853
				],
				[
					8.801106416328821,
					169.42234601568828
				],
				[
					11.881566181368726,
					168.1021719955362
				],
				[
					14.961945369381283,
					167.22202912309228
				],
				[
					16.722150537241305,
					165.9018551029402
				],
				[
					18.042324557393385,
					165.02175251900996
				],
				[
					18.922467429837525,
					164.58168108278812
				],
				[
					20.242641449989605,
					163.70157849885788
				],
				[
					23.76313236273745,
					161.94133304248396
				],
				[
					24.64319465815379,
					161.5013018947758
				],
				[
					25.96336867830587,
					160.62115902233188
				],
				[
					28.16368557090209,
					160.1811278746237
				],
				[
					29.92389073876211,
					158.86095385447163
				],
				[
					32.56423877906627,
					157.54077983431955
				],
				[
					34.324524523954096,
					157.10070839809748
				],
				[
					36.96487256425826,
					155.34046294172356
				],
				[
					38.725077732118734,
					154.9004317940154
				],
				[
					41.365425772422896,
					153.5802577738633
				],
				[
					43.12563094028292,
					152.26008375371123
				],
				[
					44.445804960435,
					151.82001231748916
				],
				[
					46.64612185303122,
					150.49983829733708
				],
				[
					48.40632702089124,
					149.179664277185
				],
				[
					49.72650104104332,
					148.73959284096316
				],
				[
					50.60664391348746,
					147.85949025703292
				],
				[
					51.486786785931145,
					146.9793876731029
				],
				[
					52.36684908134748,
					146.9793876731029
				],
				[
					52.806960806083225,
					146.53931623688084
				],
				[
					53.68702310149956,
					145.65921365295083
				],
				[
					54.5671659739437,
					145.21914221672876
				],
				[
					55.447308846387386,
					144.33903963279874
				],
				[
					56.76748286653947,
					144.33903963279874
				],
				[
					57.647545161955804,
					143.45889676035483
				],
				[
					58.967719182107885,
					143.01886561264666
				],
				[
					59.40783090684363,
					142.13872274020275
				],
				[
					60.287893202259966,
					142.13872274020275
				],
				[
					60.72800492699571,
					142.13872274020275
				],
				[
					61.168036074704105,
					142.13872274020275
				],
				[
					61.608067222412046,
					141.69869159249458
				],
				[
					62.488210094856186,
					141.69869159249458
				],
				[
					62.92824124256413,
					141.69869159249458
				],
				[
					63.36835296729987,
					141.2586201562725
				],
				[
					64.24841526271621,
					141.2586201562725
				],
				[
					64.68852698745195,
					141.2586201562725
				],
				[
					63.808384115008266,
					140.3785175723425
				],
				[
					63.36835296729987,
					139.4983746998986
				],
				[
					62.488210094856186,
					138.61827211596835
				],
				[
					61.608067222412046,
					137.29809809581627
				],
				[
					60.287893202259966,
					135.09782149173418
				],
				[
					58.967719182107885,
					133.33757603536003
				],
				[
					57.647545161955804,
					131.13729943127794
				],
				[
					56.76748286653947,
					128.93698253868195
				],
				[
					55.447308846387386,
					126.29663449837778
				],
				[
					54.5671659739437,
					124.09635789429547
				],
				[
					53.24699195379162,
					121.89608129021337
				],
				[
					51.92681793363954,
					119.69576439761738
				],
				[
					51.0466750611954,
					117.49548779353506
				],
				[
					49.72650104104332,
					115.73524233716114
				],
				[
					48.40632702089124,
					113.09489429685698
				],
				[
					47.08615300073916,
					110.45454625655282
				],
				[
					46.20609070532282,
					108.69434108869257
				],
				[
					44.445804960435,
					106.0539930483884
				],
				[
					43.12563094028292,
					103.85367615579241
				],
				[
					41.365425772422896,
					101.21332811548825
				],
				[
					39.60522060456242,
					98.13294892747592
				],
				[
					37.844934859674595,
					95.49260088717176
				],
				[
					36.96487256425826,
					92.8522528468676
				],
				[
					35.204586819370434,
					90.21190480656344
				],
				[
					33.88441279921835,
					87.57155676625928
				],
				[
					32.56423877906627,
					84.93120872595512
				],
				[
					31.24406475891419,
					83.17096326958097
				],
				[
					30.364002463497854,
					80.5306152292768
				],
				[
					28.60371671861003,
					77.89026718897264
				],
				[
					27.28354269845795,
					75.24991914866848
				],
				[
					25.523337530597928,
					72.60957110836432
				],
				[
					24.203163510445847,
					69.96922306806016
				],
				[
					22.882989490293767,
					66.88880359153416
				],
				[
					21.12278432243329,
					64.68852698745184
				],
				[
					20.242641449989605,
					62.488250383369746
				],
				[
					18.042324557393385,
					58.96775947062167
				],
				[
					17.602293409685444,
					57.64758545046959
				],
				[
					15.842088241824968,
					54.56720626245726
				],
				[
					14.961945369381283,
					51.9268582221531
				],
				[
					13.641771349229202,
					49.72654132955711
				],
				[
					12.321597329077122,
					47.08619328925295
				],
				[
					11.881566181368726,
					45.766019269100866
				],
				[
					11.001423308925041,
					43.56574266501866
				],
				[
					10.121280436480902,
					41.805497208644624
				],
				[
					10.121280436480902,
					39.60522060456242
				],
				[
					8.801106416328821,
					37.84497514818838
				],
				[
					7.921044120912484,
					35.64469854410618
				],
				[
					7.48093239617674,
					33.44442194002397
				],
				[
					6.600870100760403,
					30.364002463497854
				],
				[
					5.2806960806083225,
					28.16372585941565
				],
				[
					4.400553208164638,
					25.963408966819657
				],
				[
					3.0803791880125573,
					23.76313236273745
				],
				[
					1.7602051678604766,
					21.562855758655246
				],
				[
					1.3201740201520806,
					19.80261030228121
				],
				[
					0.8800622954163373,
					18.922507718351085
				],
				[
					0.440031147708396,
					18.042364845907173
				],
				[
					0.440031147708396,
					17.602333698199004
				],
				[
					0,
					17.162262261977048
				],
				[
					-0.44011172473574334,
					15.842088241824968
				],
				[
					-0.44011172473574334,
					14.961985657894843
				],
				[
					-0.8801428724436846,
					14.521914221672887
				],
				[
					-0.8801428724436846,
					13.201740201520806
				],
				[
					-1.760285744887824,
					11.881566181368726
				],
				[
					-2.2003168925957652,
					11.44149474514677
				],
				[
					-2.2003168925957652,
					11.44149474514677
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 236,
			"versionNonce": 1914846704,
			"isDeleted": false,
			"id": "YH94CScmY0iRTACl1dkPt",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 4.885070472002695,
			"x": 3503.7644933423107,
			"y": -1121.5545238556479,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 441.9999999999998,
			"height": 132,
			"seed": 856079120,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
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
					0
				],
				[
					8,
					0
				],
				[
					18,
					-4
				],
				[
					30,
					-10
				],
				[
					32,
					-12
				],
				[
					42,
					-16
				],
				[
					54,
					-22
				],
				[
					82,
					-32
				],
				[
					90,
					-34
				],
				[
					108,
					-38
				],
				[
					140,
					-46
				],
				[
					154,
					-50
				],
				[
					168,
					-52
				],
				[
					212,
					-60
				],
				[
					214,
					-62
				],
				[
					220,
					-64
				],
				[
					242,
					-68
				],
				[
					244,
					-70
				],
				[
					258,
					-74
				],
				[
					264,
					-76
				],
				[
					266,
					-76
				],
				[
					268,
					-78
				],
				[
					278,
					-80
				],
				[
					280,
					-82
				],
				[
					282,
					-82
				],
				[
					290,
					-82
				],
				[
					292,
					-84
				],
				[
					298,
					-84
				],
				[
					302,
					-84
				],
				[
					316,
					-86
				],
				[
					320,
					-86
				],
				[
					342,
					-90
				],
				[
					356,
					-94
				],
				[
					358,
					-94
				],
				[
					363.9999999999998,
					-94
				],
				[
					369.9999999999998,
					-96
				],
				[
					379.9999999999998,
					-100
				],
				[
					385.9999999999998,
					-102
				],
				[
					387.9999999999998,
					-104
				],
				[
					395.9999999999998,
					-108
				],
				[
					399.9999999999998,
					-110
				],
				[
					403.9999999999998,
					-110
				],
				[
					413.9999999999998,
					-116
				],
				[
					423.9999999999998,
					-120
				],
				[
					423.9999999999998,
					-122
				],
				[
					425.9999999999998,
					-122
				],
				[
					429.9999999999998,
					-124
				],
				[
					431.9999999999998,
					-126
				],
				[
					433.9999999999998,
					-126
				],
				[
					437.9999999999998,
					-130
				],
				[
					439.9999999999998,
					-132
				],
				[
					441.9999999999998,
					-132
				],
				[
					441.9999999999998,
					-132
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 70,
			"versionNonce": 17104880,
			"isDeleted": false,
			"id": "S3g7tIRUcFMQ4eQ7cnAlR",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2999.378072511846,
			"y": -517.3170934630103,
			"strokeColor": "#a18072",
			"backgroundColor": "transparent",
			"width": 275.6154695652531,
			"height": 29.434674642049686,
			"seed": 1721555216,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5351429411057325,
					0
				],
				[
					1.0703348790013933,
					0
				],
				[
					1.6055268168972816,
					0
				],
				[
					2.6758616958989023,
					0
				],
				[
					3.746196574900523,
					0
				],
				[
					4.281388512796184,
					0
				],
				[
					5.351723391797805,
					0
				],
				[
					6.422107267589581,
					0
				],
				[
					8.562777025592823,
					0
				],
				[
					9.6331609013846,
					0
				],
				[
					11.773830659387613,
					0
				],
				[
					14.449741352076671,
					0
				],
				[
					17.1256030479758,
					0
				],
				[
					20.87184861966648,
					0
				],
				[
					25.68842907035878,
					-0.5351919378957746
				],
				[
					28.899482704153797,
					-0.5351919378957746
				],
				[
					33.18087121695021,
					-0.5351919378957746
				],
				[
					37.46225972974662,
					-0.5351919378957746
				],
				[
					42.27884018043892,
					-1.0703348790016207
				],
				[
					48.70094744802873,
					-2.14071875479317
				],
				[
					54.58791177451258,
					-2.6758616958989023
				],
				[
					60.474827104206724,
					-3.2110536337947906
				],
				[
					66.8969343717963,
					-3.2110536337947906
				],
				[
					73.31904163938611,
					-3.746245571690679
				],
				[
					80.81148378597754,
					-4.281388512796411
				],
				[
					85.62806423666962,
					-5.351772388588074
				],
				[
					92.58536344215531,
					-5.351772388588074
				],
				[
					97.40194389284761,
					-5.88691532969392
				],
				[
					103.28885922254153,
					-6.422107267589695
				],
				[
					108.64063161112972,
					-6.422107267589695
				],
				[
					113.99240399971768,
					-6.422107267589695
				],
				[
					119.34412739151594,
					-6.422107267589695
				],
				[
					124.6958997801039,
					-6.422107267589695
				],
				[
					130.04767216869232,
					-6.422107267589695
				],
				[
					136.4697794362819,
					-6.422107267589695
				],
				[
					142.8918867038717,
					-6.422107267589695
				],
				[
					149.3139939714615,
					-5.88691532969392
				],
				[
					156.80643611805272,
					-4.8165804506923
				],
				[
					164.8340702025398,
					-4.281388512796411
				],
				[
					173.396896224923,
					-3.2110536337947906
				],
				[
					181.42453030941033,
					-2.14071875479317
				],
				[
					189.45216439389742,
					-1.0703348790016207
				],
				[
					197.4797984783845,
					0
				],
				[
					203.90190574597432,
					1.0703348790016207
				],
				[
					210.85915595466986,
					2.1407187547933972
				],
				[
					217.28126322225944,
					3.7462455716907925
				],
				[
					222.63308460763778,
					4.281388512796525
				],
				[
					227.44966505833008,
					5.351772388588188
				],
				[
					232.26624550902238,
					6.957299205485697
				],
				[
					236.54758502502864,
					8.027634084487318
				],
				[
					240.82902253461543,
					9.6331609013846
				],
				[
					245.6456029853075,
					11.238687718282108
				],
				[
					249.9270404948943,
					12.844214535179617
				],
				[
					254.20838001090056,
					14.449741352077012
				],
				[
					257.9546745793814,
					15.52007623107852
				],
				[
					262.2360140953879,
					17.660794985871917
				],
				[
					265.44706772918266,
					18.731129864873537
				],
				[
					269.1933622976635,
					20.33665668177082
				],
				[
					271.33403205566674,
					20.871848619666707
				],
				[
					272.4044159314583,
					21.942183498668328
				],
				[
					274.00994274835557,
					22.477375436564216
				],
				[
					274.5450856894613,
					22.477375436564216
				],
				[
					275.08022863056726,
					23.01256737445999
				],
				[
					275.6154695652531,
					23.01256737445999
				],
				[
					275.6154695652531,
					23.01256737445999
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 47,
			"versionNonce": 1782546928,
			"isDeleted": false,
			"id": "4RVEmpspDluRHzYpsCFO3",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3274.458301142413,
			"y": -495.374909964342,
			"strokeColor": "#a18072",
			"backgroundColor": "transparent",
			"width": 49.23609038913469,
			"height": 88.83914236885977,
			"seed": 1035941648,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.605526816897509,
					-2.1406697580032414
				],
				[
					-3.2110536337947906,
					-5.351723391798032
				],
				[
					-4.8165804506923,
					-8.02763408448709
				],
				[
					-6.957250208695541,
					-10.70349578038622
				],
				[
					-8.56277702559305,
					-13.91454941418101
				],
				[
					-10.168303842490559,
					-16.055268168974408
				],
				[
					-12.84421453517939,
					-19.80146474387493
				],
				[
					-14.984884293182631,
					-24.082902253461498
				],
				[
					-17.660794985871917,
					-27.82909882836225
				],
				[
					-20.871848619666707,
					-32.1105363379487
				],
				[
					-23.01251837766995,
					-36.39192485074523
				],
				[
					-25.688429070359007,
					-40.673337861936716
				],
				[
					-26.75871495257047,
					-43.884391495731506
				],
				[
					-28.899482704154025,
					-47.09544512952647
				],
				[
					-30.505009521051306,
					-50.306498763321315
				],
				[
					-31.575295403263,
					-53.51755239711622
				],
				[
					-32.11053633794859,
					-56.193438591410256
				],
				[
					-33.7160631548461,
					-59.40449222520516
				],
				[
					-35.321589971743606,
					-62.08035392110418
				],
				[
					-36.39187585395507,
					-64.75624011539827
				],
				[
					-37.99740267085258,
					-68.50246118869393
				],
				[
					-39.067786546644356,
					-71.17834738298802
				],
				[
					-41.2084563046476,
					-73.85423357728206
				],
				[
					-42.81398312154488,
					-75.99492783368032
				],
				[
					-44.41950993844239,
					-78.67081402797436
				],
				[
					-45.48989381423394,
					-79.74114890697598
				],
				[
					-46.02503675533967,
					-81.88186766176926
				],
				[
					-46.02503675533967,
					-82.41703510127007
				],
				[
					-46.560277690025714,
					-82.95220254077083
				],
				[
					-47.09542063113145,
					-83.48739447866666
				],
				[
					-47.09542063113145,
					-84.02256191816747
				],
				[
					-47.09542063113145,
					-84.55772935766828
				],
				[
					-47.09542063113145,
					-85.09292129556411
				],
				[
					-47.63056357223718,
					-85.09292129556411
				],
				[
					-48.16580450692322,
					-85.62808873506492
				],
				[
					-48.16580450692322,
					-86.16325617456573
				],
				[
					-48.700947448028955,
					-86.16325617456573
				],
				[
					-48.700947448028955,
					-87.23361555196237
				],
				[
					-48.700947448028955,
					-88.30397492935901
				],
				[
					-48.700947448028955,
					-88.83914236885977
				],
				[
					-49.23609038913469,
					-88.83914236885977
				],
				[
					-49.23609038913469,
					-88.83914236885977
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 84,
			"versionNonce": 215598064,
			"isDeleted": false,
			"id": "80ymVNLnxnJfL4CDYbIXW",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3002.0539342077445,
			"y": -522.6688658515985,
			"strokeColor": "#a18072",
			"backgroundColor": "transparent",
			"width": 238.15316083871653,
			"height": 73.85423357728206,
			"seed": 2095437072,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690850,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.5351919378956609,
					0
				],
				[
					2.14071875479317,
					0
				],
				[
					2.6758616958989023,
					-0.5351429411058461
				],
				[
					4.281388512796411,
					-1.0703348790016207
				],
				[
					6.4221072675898085,
					-1.0703348790016207
				],
				[
					8.562826022382978,
					-1.0703348790016207
				],
				[
					10.168352839280487,
					-1.6055268168973953
				],
				[
					12.309022597283501,
					-2.675861695899016
				],
				[
					15.52007623107852,
					-3.2110536337949043
				],
				[
					18.195986923767578,
					-3.7461965749006367
				],
				[
					20.33665668177082,
					-4.8165804506923
				],
				[
					23.012567374459877,
					-5.35174789019311
				],
				[
					25.688429070359007,
					-6.957274707090505
				],
				[
					28.899482704153797,
					-7.492442146591316
				],
				[
					32.645728275844476,
					-9.097968963488825
				],
				[
					36.39192485074523,
					-9.6331609013846
				],
				[
					40.138170422435905,
					-11.238687718281994
				],
				[
					43.884415994126584,
					-12.309022597283615
				],
				[
					48.700996444818884,
					-13.914549414181124
				],
				[
					54.052719836616916,
					-15.52007623107852
				],
				[
					60.474827104206724,
					-17.660794985871803
				],
				[
					65.29140755489902,
					-19.266321802769255
				],
				[
					72.2487067603845,
					-21.94218349866827
				],
				[
					79.20600596587019,
					-24.618069692962365
				],
				[
					85.09292129556411,
					-26.75876394936057
				],
				[
					91.51502856315369,
					-29.434650143654665
				],
				[
					96.33160901384622,
					-31.040176960552117
				],
				[
					101.68338140243418,
					-33.18087121695032
				],
				[
					105.96476991523082,
					-35.321589971743606
				],
				[
					109.7110154869215,
					-36.92711678864106
				],
				[
					113.99240399971791,
					-38.53264360553845
				],
				[
					117.20345763351293,
					-39.602978484540074
				],
				[
					120.94970320520338,
					-41.74369723933336
				],
				[
					124.69589978010413,
					-43.34922405623081
				],
				[
					128.44214535179503,
					-43.88439149573162
				],
				[
					131.6531989855896,
					-45.489918312629015
				],
				[
					135.3994445572805,
					-47.09544512952647
				],
				[
					138.6104981910753,
					-48.16580450692311
				],
				[
					142.35669476597582,
					-49.23613938592473
				],
				[
					145.56774839977084,
					-50.306498763321315
				],
				[
					148.24365909246012,
					-50.841666202822125
				],
				[
					150.91952078835902,
					-52.44719301971958
				],
				[
					153.0602395431522,
					-52.98238495761541
				],
				[
					155.20090930115543,
					-53.51755239711622
				],
				[
					156.80643611805294,
					-54.58791177451286
				],
				[
					159.482346810742,
					-55.12307921401367
				],
				[
					161.62301656874524,
					-56.193438591410256
				],
				[
					163.7637353235384,
					-56.72860603091107
				],
				[
					166.43959701943754,
					-57.26377347041188
				],
				[
					169.65065065323256,
					-58.33413284780852
				],
				[
					173.396896224923,
					-58.86930028730933
				],
				[
					177.14314179661392,
					-59.93965966470597
				],
				[
					181.959722247306,
					-60.47482710420678
				],
				[
					186.77630269799852,
					-61.545186481603366
				],
				[
					191.5928831486906,
					-62.61554585900001
				],
				[
					194.8039367824856,
					-63.68588073800163
				],
				[
					198.55013335738636,
					-64.75624011539827
				],
				[
					201.76118699118115,
					-65.29140755489908
				],
				[
					204.4370976838702,
					-66.36176693229572
				],
				[
					207.1130083765595,
					-66.89693437179648
				],
				[
					209.2536781345625,
					-67.43212630969236
				],
				[
					211.92958882725156,
					-67.96729374919312
				],
				[
					213.53511564414907,
					-67.96729374919312
				],
				[
					215.67578540215231,
					-68.50246118869393
				],
				[
					217.28131221904982,
					-69.03765312658976
				],
				[
					219.42198197705306,
					-69.57282056609057
				],
				[
					221.56274972863616,
					-70.10798800559138
				],
				[
					223.7034194866394,
					-70.10798800559138
				],
				[
					225.3089463035369,
					-70.64317994348721
				],
				[
					227.44961606154015,
					-71.17834738298802
				],
				[
					229.05514287843766,
					-71.17834738298802
				],
				[
					231.19591063002076,
					-71.17834738298802
				],
				[
					232.80143744691827,
					-71.71351482248883
				],
				[
					234.40696426381578,
					-72.78387419988547
				],
				[
					236.0124910807133,
					-72.78387419988547
				],
				[
					237.08277696292475,
					-73.31904163938623
				],
				[
					237.6180178976108,
					-73.85423357728206
				],
				[
					238.15316083871653,
					-73.85423357728206
				],
				[
					238.15316083871653,
					-73.85423357728206
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 967,
			"versionNonce": 651937264,
			"isDeleted": false,
			"id": "q9gHbCVGIobr3Zw3SVplO",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3369.281834319,
			"y": -299.1682621463823,
			"strokeColor": "#a18072",
			"backgroundColor": "transparent",
			"width": 166.76794491677992,
			"height": 166.38720199385773,
			"seed": 428389136,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.3807254936282334,
					0.19038017610796487
				],
				[
					-0.5711230990300464,
					0.5711230990300464
				],
				[
					-0.7614858458441631,
					0.9518747365990521
				],
				[
					-0.9518485926582798,
					1.713369297090253
				],
				[
					-0.9518485926582798,
					2.665244033689305
				],
				[
					-0.9518485926582798,
					3.807490231749398
				],
				[
					-0.5711230990300464,
					4.9497364298096045
				],
				[
					0.38076035221592974,
					6.472734265438703
				],
				[
					1.1422461980600929,
					7.80535192495995
				],
				[
					2.284492396120413,
					9.51872122205009
				],
				[
					3.426738594180506,
					11.232090519140343
				],
				[
					4.949745144456529,
					13.135831277691523
				],
				[
					6.282354089330738,
					15.420323673811822
				],
				[
					7.805360639606761,
					17.32407314701004
				],
				[
					9.328367189882783,
					20.179688642160386
				],
				[
					11.041736486972923,
					22.273800862172607
				],
				[
					12.564708178661476,
					25.129416357322953
				],
				[
					14.468475081153429,
					27.794660391012258
				],
				[
					16.181844378243795,
					31.22139898519265
				],
				[
					18.08557642214805,
					34.83850904083408
				],
				[
					20.560431565082354,
					38.836370734044635
				],
				[
					23.416047060232813,
					42.834232427255074
				],
				[
					26.271662555383273,
					46.64172265900447
				],
				[
					29.317675655935318,
					50.639584352215024
				],
				[
					32.36365389789967,
					54.44707458396442
				],
				[
					34.8385090408342,
					57.1123099030068
				],
				[
					38.07488488820036,
					60.348677035726155
				],
				[
					40.93050038335082,
					63.77541562990655
				],
				[
					42.26310932822503,
					65.29841346553565
				],
				[
					43.97647862531517,
					67.20216293873386
				],
				[
					44.92836207656114,
					68.53477188360819
				],
				[
					45.49948517559119,
					69.86739825777624
				],
				[
					46.070608274621236,
					71.2000246319443
				],
				[
					46.451368626837166,
					72.3422708300044
				],
				[
					46.64173137365128,
					73.4845170280646
				],
				[
					46.83209412046563,
					74.81712597293892
				],
				[
					47.02249172586721,
					76.14975234710698
				],
				[
					47.212854472681556,
					77.29199854516708
				],
				[
					47.59361482489726,
					78.81498766614936
				],
				[
					47.97434031852572,
					80.14761404031742
				],
				[
					48.35510067074165,
					81.48024041448559
				],
				[
					48.926223769771696,
					82.8128493593598
				],
				[
					49.306984121987625,
					83.76473281060578
				],
				[
					49.87810722101767,
					84.71659883255802
				],
				[
					50.44923032004772,
					85.66846485451015
				],
				[
					50.639593066861835,
					86.04922520672608
				],
				[
					50.82995581367618,
					86.62034830575612
				],
				[
					51.020353419077765,
					87.00109122867832
				],
				[
					51.21071616589188,
					87.3818341516004
				],
				[
					51.21071616589188,
					87.95295725063045
				],
				[
					51.21071616589188,
					88.14333742673841
				],
				[
					51.21071616589188,
					88.90484070187642
				],
				[
					51.401078912706225,
					89.2855836247985
				],
				[
					51.59147651810781,
					90.04708689993652
				],
				[
					51.59147651810781,
					90.8085727457808
				],
				[
					51.781839264922155,
					91.76045619702677
				],
				[
					51.781839264922155,
					92.52194204287105
				],
				[
					52.16259961713786,
					93.28344531800906
				],
				[
					52.54332511076632,
					94.04494859314707
				],
				[
					52.73372271616813,
					94.9968146150992
				],
				[
					52.92408546298225,
					95.75831789023721
				],
				[
					53.30484581519818,
					96.51980373608149
				],
				[
					53.495208562012294,
					97.09092683511153
				],
				[
					53.68557130882641,
					97.47168718732746
				],
				[
					53.68557130882641,
					97.85243011024954
				],
				[
					53.68557130882641,
					98.04281028635751
				],
				[
					53.68557130882641,
					98.61393338538755
				],
				[
					53.68557130882641,
					99.1850564844176
				],
				[
					53.30484581519818,
					99.75617958344776
				],
				[
					53.114448209796365,
					99.94654233026188
				],
				[
					52.92408546298225,
					100.70804560539989
				],
				[
					52.73372271616813,
					101.08878852832197
				],
				[
					52.3529623639522,
					101.4695488805379
				],
				[
					52.16259961713786,
					102.23103472638218
				],
				[
					51.97220201173627,
					102.42141490249003
				],
				[
					51.97220201173627,
					102.80215782541222
				],
				[
					51.781839264922155,
					103.18291817762815
				],
				[
					51.781839264922155,
					103.37328092444227
				],
				[
					51.401078912706225,
					103.37328092444227
				],
				[
					51.21071616589188,
					103.56366110055023
				],
				[
					50.82995581367618,
					103.94440402347232
				],
				[
					50.44923032004772,
					104.13478419958028
				],
				[
					49.68770961561586,
					104.51552712250248
				],
				[
					48.73586102295758,
					104.89628747471829
				],
				[
					47.59361482489726,
					105.46741057374845
				],
				[
					46.26097102143558,
					105.84815349667053
				],
				[
					44.16687623071698,
					106.80001951862266
				],
				[
					42.834232427255074,
					107.56152279376067
				],
				[
					41.120863130164935,
					108.32302606889868
				],
				[
					39.407493833074795,
					109.27489209085093
				],
				[
					37.12300143695438,
					110.41713828891102
				],
				[
					35.40963213986424,
					111.55938448697123
				],
				[
					33.696262842774104,
					112.51125050892335
				],
				[
					31.982893545683737,
					113.27275378406136
				],
				[
					30.45992185399541,
					114.03425705919938
				],
				[
					28.74655255690527,
					114.60538015822942
				],
				[
					26.46206016078486,
					115.3668660040737
				],
				[
					24.939053610508836,
					115.74762635628963
				],
				[
					23.035321566604352,
					115.93798910310375
				],
				[
					20.941191917298283,
					116.69949237824176
				],
				[
					18.275939168962168,
					117.27061547727192
				],
				[
					16.56256987187203,
					117.84173857630196
				],
				[
					13.897351982123382,
					118.60324185143998
				],
				[
					11.232099233787267,
					119.5551078733921
				],
				[
					9.13796958448097,
					120.50697389534434
				],
				[
					6.853477188360785,
					121.26847717048236
				],
				[
					4.949745144456529,
					122.41072336854245
				],
				[
					2.8556154951504595,
					123.36258939049469
				],
				[
					0.9518834512459762,
					124.50483558855478
				],
				[
					-0.7614858458441631,
					125.45671903980076
				],
				[
					-2.0940947907186,
					126.21820488564492
				],
				[
					-3.6171013409946227,
					126.97970816078305
				],
				[
					-4.949710285868832,
					127.5508312598131
				],
				[
					-6.282354089330738,
					128.3123345349511
				],
				[
					-7.614963034204948,
					128.6930774578732
				],
				[
					-9.13796958448097,
					129.26420055690335
				],
				[
					-10.851338881571337,
					129.64494347982543
				],
				[
					-12.374310573259663,
					130.40644675496344
				],
				[
					-14.278077475751616,
					130.9775698539935
				],
				[
					-15.991446772841982,
					131.35831277691557
				],
				[
					-18.275939168962168,
					132.31019622816154
				],
				[
					-19.989308466052307,
					132.8813193271916
				],
				[
					-21.89304050995679,
					133.2620622501138
				],
				[
					-23.796772553861047,
					134.0235655252518
				],
				[
					-25.700539456353,
					134.97543154720393
				],
				[
					-27.413908753443366,
					135.54655464623409
				],
				[
					-29.31764079734762,
					136.4984206681862
				],
				[
					-31.221372841251878,
					137.4503041194322
				],
				[
					-33.12513974374383,
					138.40217014138432
				],
				[
					-34.83850904083397,
					139.54441633944452
				],
				[
					-36.551878337924336,
					140.49628236139665
				],
				[
					-38.265247635014475,
					141.63852855945686
				],
				[
					-39.78821932670303,
					142.40003183459487
				],
				[
					-41.120863130164935,
					143.351897856547
				],
				[
					-42.26310932822503,
					144.113401131685
				],
				[
					-43.59571827309924,
					145.06526715363725
				],
				[
					-44.73796447115933,
					145.6363902526673
				],
				[
					-45.88021066921942,
					146.20751335169734
				],
				[
					-47.02245686727974,
					146.58827370391327
				],
				[
					-48.545463417555766,
					147.34975954975755
				],
				[
					-50.06843510924432,
					147.73051990197337
				],
				[
					-51.59144165952034,
					148.30164300100353
				],
				[
					-53.87593405564053,
					149.0631288468477
				],
				[
					-56.16042645176071,
					149.44388919906362
				],
				[
					-58.25455610106678,
					150.20537504490778
				],
				[
					-60.539048497187196,
					150.5861353971237
				],
				[
					-62.633143287905796,
					151.15725849615376
				],
				[
					-64.53691019039775,
					151.7283815951838
				],
				[
					-66.05988188208607,
					152.109124518106
				],
				[
					-67.5828884323621,
					152.29950469421397
				],
				[
					-68.72513463042219,
					152.870627793244
				],
				[
					-69.86738082848228,
					153.2513707161661
				],
				[
					-70.62886667432667,
					153.44175089227406
				],
				[
					-71.77111287238677,
					153.82249381519625
				],
				[
					-72.72299632363274,
					154.3936169142263
				],
				[
					-74.24600287390876,
					154.77435983714838
				],
				[
					-75.9593721709989,
					155.5358631122864
				],
				[
					-77.67274146808927,
					156.10698621131644
				],
				[
					-79.57647351199353,
					156.67810931034649
				],
				[
					-81.09948006226955,
					156.86848948645445
				],
				[
					-83.19357485298815,
					157.4396125854845
				],
				[
					-85.28770450229422,
					158.01073568451466
				],
				[
					-87.38183415160029,
					158.20109843132877
				],
				[
					-89.28556619550477,
					158.5818587835447
				],
				[
					-91.18929823940903,
					158.77222153035882
				],
				[
					-92.71230478968505,
					158.96260170646678
				],
				[
					-94.04491373455949,
					158.96260170646678
				],
				[
					-95.37755753802116,
					159.15298188257475
				],
				[
					-96.51980373608149,
					159.53372480549683
				],
				[
					-97.28128958192565,
					159.7241049816048
				],
				[
					-98.23317303317162,
					160.104847904527
				],
				[
					-99.56578197804606,
					160.29522808063496
				],
				[
					-100.51766542929204,
					160.866351179665
				],
				[
					-101.2791512751362,
					161.05671392647912
				],
				[
					-102.23103472638218,
					161.62783702550917
				],
				[
					-103.18288331904046,
					162.1989601245392
				],
				[
					-104.32512951710055,
					162.77008322356926
				],
				[
					-105.27701296834653,
					163.34120632259942
				],
				[
					-106.2288964195925,
					163.72196667481523
				],
				[
					-107.3711426176526,
					164.2930897738454
				],
				[
					-108.3229912103111,
					164.4834525206595
				],
				[
					-109.27487466155708,
					164.67383269676748
				],
				[
					-110.03636050740124,
					165.24495579579752
				],
				[
					-110.7978812118331,
					165.4353359719055
				],
				[
					-111.55936705767726,
					165.62569871871972
				],
				[
					-112.13049015670754,
					166.00645907093553
				],
				[
					-112.70161325573758,
					166.00645907093553
				],
				[
					-112.8919760025517,
					166.19682181774976
				],
				[
					-112.8919760025517,
					166.38720199385773
				],
				[
					-113.08237360795351,
					166.38720199385773
				],
				[
					-112.70161325573758,
					166.19682181774976
				],
				[
					-112.13049015670754,
					165.81607889482768
				],
				[
					-111.55936705767726,
					165.05457561968956
				],
				[
					-110.7978812118331,
					164.2930897738454
				],
				[
					-109.84599776058712,
					163.53158649870738
				],
				[
					-108.89411430934115,
					162.77008322356926
				],
				[
					-107.94226571668264,
					161.81821720161713
				],
				[
					-106.99038226543666,
					160.67597100355704
				],
				[
					-106.03849881419069,
					159.53372480549683
				],
				[
					-105.08665022153241,
					158.5818587835447
				],
				[
					-104.13476677028643,
					157.24923240937653
				],
				[
					-103.18288331904046,
					155.91660603520847
				],
				[
					-102.4213974731963,
					154.77435983714838
				],
				[
					-101.46951402195032,
					153.82249381519625
				],
				[
					-100.51766542929204,
					152.48986744102808
				],
				[
					-99.75614472486018,
					151.15725849615376
				],
				[
					-98.61389852680009,
					149.44388919906362
				],
				[
					-97.8524126809557,
					148.11126282489556
				],
				[
					-96.90052922970972,
					146.7786364507274
				],
				[
					-95.94868063705144,
					145.06526715363725
				],
				[
					-94.99679718580546,
					144.113401131685
				],
				[
					-94.04491373455949,
					142.59041201070283
				],
				[
					-92.90266753649917,
					141.25778563653466
				],
				[
					-91.76042133843907,
					139.9251592623666
				],
				[
					-90.42781239356486,
					138.7829130643065
				],
				[
					-88.52408034966061,
					137.25992394332422
				],
				[
					-87.00107379938436,
					135.92729756915617
				],
				[
					-85.85882760132426,
					134.59468862428184
				],
				[
					-84.33582105104824,
					133.45244242622164
				],
				[
					-82.6224517539581,
					131.7390731291315
				],
				[
					-81.48020555589778,
					130.5968269310714
				],
				[
					-79.38611076517941,
					128.6930774578732
				],
				[
					-78.0534669617175,
					127.5508312598131
				],
				[
					-77.10161836905922,
					126.78932798467508
				],
				[
					-75.76897456559732,
					125.64708178661488
				],
				[
					-74.24600287390876,
					124.50483558855478
				],
				[
					-72.72299632363274,
					123.17222664368046
				],
				[
					-71.58075012557265,
					122.22034319243448
				],
				[
					-69.86738082848228,
					121.26847717048236
				],
				[
					-68.53477188360807,
					120.12623097242215
				],
				[
					-67.01176533333205,
					119.17436495047002
				],
				[
					-65.67915638845784,
					118.22248149922405
				],
				[
					-64.34651258499593,
					117.08023530116395
				],
				[
					-63.20426638693584,
					115.93798910310375
				],
				[
					-62.06202018887575,
					114.79574290504365
				],
				[
					-60.91977399081543,
					113.65349670698345
				],
				[
					-59.777527792755336,
					112.70163068503132
				],
				[
					-58.63528159469524,
					111.55938448697123
				],
				[
					-57.49303539663515,
					110.60751846501898
				],
				[
					-56.16042645176071,
					109.46527226695889
				],
				[
					-54.827817506886504,
					108.32302606889868
				],
				[
					-53.68557130882641,
					107.18077987083859
				],
				[
					-52.352927505364505,
					106.0385336727785
				],
				[
					-51.020318560490296,
					104.89628747471829
				],
				[
					-49.30694926339993,
					103.7540412766582
				],
				[
					-48.164703065339836,
					102.23103472638218
				],
				[
					-46.64169651506381,
					100.89842578150785
				],
				[
					-45.49945031700372,
					99.5657994073398
				],
				[
					-44.3572041189434,
					98.23317303317162
				],
				[
					-43.40535552628512,
					97.2813070112195
				],
				[
					-42.64383482185326,
					95.94868063705132
				],
				[
					-41.31122587697905,
					94.61607169217712
				],
				[
					-40.54974003113489,
					93.28344531800906
				],
				[
					-39.59785657988891,
					91.95081894384089
				],
				[
					-38.45561038182859,
					90.61820999896656
				],
				[
					-37.503726930582616,
					89.2855836247985
				],
				[
					-36.93260383155257,
					88.33371760284638
				],
				[
					-35.98075523889429,
					87.19147140478628
				],
				[
					-34.83850904083397,
					85.85884503061811
				],
				[
					-33.88662558958799,
					84.52621865645006
				],
				[
					-32.93474213834202,
					83.19360971157573
				],
				[
					-31.982893545683737,
					82.05136351351564
				],
				[
					-30.840647347623644,
					80.52835696323962
				],
				[
					-30.079126643191785,
					79.00536784225733
				],
				[
					-29.31764079734762,
					77.48237872127504
				],
				[
					-28.55615495150346,
					75.95937217099902
				],
				[
					-27.7946342470716,
					74.24600287390888
				],
				[
					-27.223511148041553,
					72.53263357681863
				],
				[
					-26.842785654413092,
					71.39038737875842
				],
				[
					-26.08126494998146,
					69.67701808166828
				],
				[
					-25.510141850951413,
					67.96364878457803
				],
				[
					-24.93901875192114,
					66.63103983970382
				],
				[
					-24.558293258292906,
					65.10803328942768
				],
				[
					-23.60640980704693,
					63.585044168445506
				],
				[
					-23.035286708016883,
					62.25241779427745
				],
				[
					-21.89304050995679,
					60.539048497187196
				],
				[
					-21.1315546641124,
					58.82567920009694
				],
				[
					-19.989308466052307,
					57.30269007911477
				],
				[
					-19.03742501480633,
					55.39894060591655
				],
				[
					-17.89517881674624,
					53.11444820979625
				],
				[
					-17.133692970902075,
					51.40107891270611
				],
				[
					-15.991446772841982,
					49.49733815415482
				],
				[
					-14.849200574781662,
					47.59359739560364
				],
				[
					-14.08767987035003,
					45.68984792240542
				],
				[
					-12.94543367228971,
					43.786107163854126
				],
				[
					-11.803187474229617,
					42.07273786676399
				],
				[
					-10.851338881571337,
					40.549740031134775
				],
				[
					-9.518695078109431,
					39.0267509101526
				],
				[
					-8.566846485450924,
					37.69412453598454
				],
				[
					-7.805325781019064,
					36.361506876463295
				],
				[
					-6.6630795829589715,
					35.02888921694205
				],
				[
					-5.901593737114808,
					33.69626284277399
				],
				[
					-5.140107891270645,
					32.173273721791816
				],
				[
					-4.378587186838786,
					30.840647347623644
				],
				[
					-3.8074640878087394,
					29.50802968810251
				],
				[
					-3.0459782419645762,
					27.9850318524733
				],
				[
					-2.47485514293453,
					27.03316583052117
				],
				[
					-2.0940947907186,
					25.890919632461078
				],
				[
					-1.7133692970901393,
					24.74867343440087
				],
				[
					-1.3326089448742096,
					23.606427236340778
				],
				[
					-0.9518485926582798,
					22.46418103828057
				],
				[
					-0.5711230990300464,
					21.131554664112514
				],
				[
					-0.3807254936282334,
					20.179688642160386
				],
				[
					-0.1903627468141167,
					19.22781390556122
				],
				[
					0.19039760540181305,
					18.275939168962168
				],
				[
					0.19039760540181305,
					17.32407314701004
				],
				[
					0.38076035221592974,
					16.562569871871915
				],
				[
					0.7615207044318595,
					15.801075311380828
				],
				[
					0.9518834512459762,
					15.03958075088974
				],
				[
					0.9518834512459762,
					14.468457651859694
				],
				[
					0.9518834512459762,
					13.516582915260528
				],
				[
					1.1422461980600929,
					13.135831277691523
				],
				[
					1.1422461980600929,
					12.564708178661476
				],
				[
					1.1422461980600929,
					12.374336717200435
				],
				[
					1.332643803461906,
					12.374336717200435
				],
				[
					1.332643803461906,
					12.564708178661476
				],
				[
					1.332643803461906,
					13.516582915260528
				],
				[
					1.5230065502760226,
					15.229952212350781
				],
				[
					2.284492396120413,
					17.70481606993212
				],
				[
					3.617136199582319,
					20.941183202651473
				],
				[
					5.711230990300692,
					25.319796533430917
				],
				[
					7.614997892792644,
					29.127278050533505
				],
				[
					10.66097613475722,
					34.077014480342996
				],
				[
					13.70695437672157,
					39.21712237161364
				],
				[
					17.324090576303888,
					44.73798190045329
				],
				[
					20.941191917298283,
					50.829955813676065
				],
				[
					23.796807412448743,
					55.01819768299447
				],
				[
					27.033183259814905,
					59.01605937620491
				],
				[
					29.508038402749435,
					62.25241779427745
				],
				[
					31.41177044665369,
					65.29841346553565
				],
				[
					33.12513974374383,
					68.15402896068599
				],
				[
					33.88666044817569,
					69.48665533485416
				],
				[
					34.64814629402008,
					71.77114773097435
				],
				[
					35.40963213986424,
					73.86525995098668
				],
				[
					36.36151559111022,
					75.95937217099902
				],
				[
					36.932638690140266,
					77.67274146808916
				],
				[
					37.88452214138624,
					79.76687111739534
				],
				[
					38.45564524041629,
					81.67060316129971
				],
				[
					39.21713108626068,
					83.19360971157573
				],
				[
					39.97861693210484,
					84.52621865645006
				],
				[
					40.7401376365367,
					86.23958795354031
				],
				[
					41.69198622919498,
					87.00109122867832
				],
				[
					42.07274658141091,
					87.76259450381633
				],
				[
					42.45350693362684,
					87.95295725063045
				],
				[
					42.45350693362684,
					88.14333742673841
				],
				[
					42.64386968044096,
					88.14333742673841
				],
				[
					42.64386968044096,
					88.71446052576846
				],
				[
					42.64386968044096,
					89.47596380090647
				],
				[
					42.45350693362684,
					90.23744964675075
				],
				[
					42.26310932822503,
					91.18933309799672
				],
				[
					42.07274658141091,
					91.95081894384089
				],
				[
					42.07274658141091,
					92.71232221897901
				],
				[
					41.882383834596794,
					93.66418824093114
				],
				[
					41.501623482380865,
					94.23531133996119
				],
				[
					41.501623482380865,
					94.9968146150992
				],
				[
					41.31126073556675,
					95.75831789023721
				],
				[
					41.120863130164935,
					96.13906081315929
				],
				[
					40.93050038335082,
					97.09092683511153
				],
				[
					40.93050038335082,
					97.85243011024954
				],
				[
					40.7401376365367,
					98.42355320927959
				],
				[
					40.7401376365367,
					99.1850564844176
				],
				[
					40.35937728432077,
					100.32730268247781
				],
				[
					39.97861693210484,
					100.70804560539989
				],
				[
					39.788254185290725,
					101.65991162735202
				],
				[
					39.59789143847638,
					102.04067197956795
				],
				[
					38.83637073404475,
					102.99253800152019
				],
				[
					38.2652476350147,
					103.37328092444227
				],
				[
					37.313399042356195,
					103.94440402347232
				],
				[
					35.98075523889429,
					104.89628747471829
				],
				[
					33.696262842774104,
					105.65777332056257
				],
				[
					31.602168052055504,
					106.0385336727785
				],
				[
					28.74655255690527,
					107.18077987083859
				],
				[
					25.129416357322953,
					107.94226571668275
				],
				[
					21.1315546641124,
					108.89414916792873
				],
				[
					17.895213675333935,
					109.65563501377301
				],
				[
					12.75510578406329,
					111.17864156404903
				],
				[
					9.89949028891283,
					111.94012740989331
				],
				[
					6.282354089330738,
					113.46313396016933
				],
				[
					2.665252748336343,
					114.79574290504365
				],
				[
					-1.5229716916885536,
					116.31874945531968
				],
				[
					-4.378587186838786,
					117.651358400194
				],
				[
					-7.805325781019064,
					119.17436495047002
				],
				[
					-10.851338881571337,
					120.6973540714522
				],
				[
					-14.278077475751616,
					122.41072336854245
				],
				[
					-17.89517881674624,
					124.1240926656327
				],
				[
					-21.51228015774086,
					125.64708178661488
				],
				[
					-25.700539456353,
					126.78932798467508
				],
				[
					-29.50800354416174,
					128.3123345349511
				],
				[
					-33.88662558958799,
					129.26420055690335
				],
				[
					-38.07485002961289,
					130.5968269310714
				],
				[
					-43.40535552628512,
					132.11981605205358
				],
				[
					-46.26097102143535,
					132.69093915108363
				],
				[
					-49.30694926339993,
					133.64280517303587
				],
				[
					-52.733687857580435,
					134.59468862428184
				],
				[
					-55.9700637049466,
					135.73693482234194
				],
				[
					-58.25455610106678,
					136.68880084429418
				],
				[
					-60.91977399081543,
					137.83104704235427
				],
				[
					-63.58502673915177,
					138.97329324041436
				],
				[
					-65.67915638845784,
					139.9251592623666
				],
				[
					-67.5828884323621,
					140.87704271361258
				],
				[
					-69.67701808166817,
					141.82890873556482
				],
				[
					-72.53263357681863,
					143.16153510973288
				],
				[
					-74.62672836753723,
					144.4941440546071
				],
				[
					-77.29198111587334,
					146.01715060488323
				],
				[
					-79.76683625880764,
					147.15939680294332
				],
				[
					-82.43208900714376,
					148.87276610003357
				],
				[
					-84.90694415007829,
					150.39575522101575
				],
				[
					-87.00107379938436,
					151.53800141907595
				],
				[
					-88.71444309647472,
					152.48986744102808
				],
				[
					-90.42781239356486,
					153.82249381519625
				],
				[
					-91.37969584481084,
					154.58399709033426
				],
				[
					-92.141181690655,
					154.96474001325635
				],
				[
					-92.90266753649917,
					155.72624328839436
				],
				[
					-93.47379063552921,
					155.91660603520847
				],
				[
					-93.85455098774514,
					156.2973663874244
				],
				[
					-93.85455098774514,
					156.48772913423852
				],
				[
					-94.04491373455949,
					156.48772913423852
				],
				[
					-94.04491373455949,
					156.2973663874244
				],
				[
					-93.66418824093103,
					155.91660603520847
				],
				[
					-93.2834278887151,
					155.1551201893643
				],
				[
					-92.33154443746912,
					154.0128739913041
				],
				[
					-91.37969584481084,
					152.48986744102808
				],
				[
					-90.04705204134893,
					150.5861353971237
				],
				[
					-88.71444309647472,
					149.25350902295565
				],
				[
					-87.38183415160029,
					147.15939680294332
				],
				[
					-85.66846485451015,
					145.06526715363725
				],
				[
					-84.14545830423413,
					142.97115493362492
				],
				[
					-82.43208900714376,
					140.87704271361258
				],
				[
					-81.09948006226955,
					138.7829130643065
				],
				[
					-79.00535041296348,
					136.68880084429418
				],
				[
					-77.48234386268746,
					134.97543154720393
				],
				[
					-75.19785146656727,
					133.07168207400582
				],
				[
					-73.29411942266279,
					130.78718967788552
				],
				[
					-71.3903873787583,
					128.88345763398115
				],
				[
					-68.53477188360807,
					126.40858506175289
				],
				[
					-66.63100498111612,
					124.50483558855478
				],
				[
					-64.15614983818182,
					121.8396002695124
				],
				[
					-61.871657442061405,
					119.5551078733921
				],
				[
					-59.777527792755336,
					117.27061547727192
				],
				[
					-57.49303539663515,
					114.2246198060135
				],
				[
					-56.16042645176071,
					112.51125050892335
				],
				[
					-54.63741990148469,
					110.60751846501898
				],
				[
					-53.114448209796365,
					107.94226571668275
				],
				[
					-51.78180440633446,
					106.60965677180855
				],
				[
					-50.639558208274366,
					104.89628747471829
				],
				[
					-49.30694926339993,
					103.18291817762815
				],
				[
					-48.164703065339836,
					102.23103472638218
				],
				[
					-47.21281961409386,
					101.08878852832197
				],
				[
					-46.26097102143535,
					100.13692250636984
				],
				[
					-45.11872482337526,
					99.5657994073398
				],
				[
					-44.166841372129284,
					98.42355320927959
				],
				[
					-43.02459517406919,
					97.66204993414158
				],
				[
					-42.26310932822503,
					97.09092683511153
				],
				[
					-41.120863130164935,
					95.94868063705132
				],
				[
					-40.16897967891896,
					94.9968146150992
				],
				[
					-38.83637073404452,
					93.8545684170391
				],
				[
					-37.69412453598443,
					92.71232221897901
				],
				[
					-36.171117985708406,
					91.18933309799672
				],
				[
					-34.45774868861827,
					89.47596380090647
				],
				[
					-32.7443793915279,
					87.95295725063045
				],
				[
					-31.03101009443776,
					86.04922520672608
				],
				[
					-29.127278050533505,
					84.14547573352786
				],
				[
					-27.223511148041553,
					82.43210643643772
				],
				[
					-25.510141850951413,
					80.71873713934758
				],
				[
					-23.98717015926286,
					79.1957480183653
				],
				[
					-22.083403256770907,
					77.48237872127504
				],
				[
					-20.37003395968054,
					75.95937217099902
				],
				[
					-19.03742501480633,
					74.24600287390888
				],
				[
					-17.324055717716192,
					72.53263357681863
				],
				[
					-15.610686420626052,
					70.62890153291426
				],
				[
					-13.70695437672157,
					68.53477188360819
				],
				[
					-12.183947826445547,
					66.63103983970382
				],
				[
					-10.280215782541063,
					63.96578709136759
				],
				[
					-8.566846485450924,
					61.68129469524729
				],
				[
					-7.424600287390831,
					59.587182475234954
				],
				[
					-6.091956483928925,
					57.30269007911477
				],
				[
					-4.949710285868832,
					54.827817506886504
				],
				[
					-4.188224440024669,
					52.352953649305164
				],
				[
					-3.0459782419645762,
					49.49733815415482
				],
				[
					-2.2844923961201857,
					47.21284575803463
				],
				[
					-1.3326089448742096,
					45.11872482337537
				],
				[
					-0.3807254936282334,
					42.834232427255074
				],
				[
					0.38076035221592974,
					40.930491668703894
				],
				[
					1.5230065502760226,
					39.21712237161364
				],
				[
					2.474890001521999,
					37.50375307452339
				],
				[
					3.046013100552045,
					36.361506876463295
				],
				[
					3.8074989463964357,
					34.83850904083408
				],
				[
					4.1882592986123655,
					34.077014480342996
				],
				[
					4.568984792240599,
					33.31551991985191
				],
				[
					4.759382397642412,
					32.74439682082186
				],
				[
					4.949745144456529,
					32.74439682082186
				],
				[
					4.949745144456529,
					32.9347682822829
				],
				[
					4.949745144456529,
					33.50589138131295
				],
				[
					4.949745144456529,
					34.457766117912
				],
				[
					4.949745144456529,
					35.60001231597221
				],
				[
					4.949745144456529,
					36.361506876463295
				],
				[
					5.140107891270645,
					37.50375307452339
				],
				[
					5.330505496672458,
					39.21712237161364
				],
				[
					5.520868243486575,
					40.74012020724274
				],
				[
					6.282354089330738,
					42.834232427255074
				],
				[
					7.424600287390831,
					45.49947646094438
				],
				[
					8.947606837666854,
					48.73584359366373
				],
				[
					10.66097613475722,
					52.16258218784412
				],
				[
					12.75510578406329,
					55.97006370494671
				],
				[
					14.84920057478189,
					59.20643083766606
				],
				[
					17.133692970902075,
					63.01392106941546
				],
				[
					19.608582972424074,
					66.44065966359585
				],
				[
					21.89307536854426,
					69.86739825777624
				],
				[
					24.177567764664673,
					72.15189065389654
				],
				[
					25.890937061754812,
					74.43638305001684
				],
				[
					26.84278565441332,
					75.95937217099902
				],
				[
					27.60430635884495,
					77.10161836905911
				],
				[
					28.55615495150346,
					78.24386456711932
				],
				[
					29.127278050533505,
					79.1957480183653
				],
				[
					29.888798754965364,
					79.95723386420946
				],
				[
					30.269524248593598,
					81.09948006226966
				],
				[
					31.031044953025457,
					82.05136351351564
				],
				[
					31.79253079886962,
					83.19360971157573
				],
				[
					32.55401664471378,
					84.14547573352786
				],
				[
					33.31553734914564,
					85.0973417554801
				],
				[
					33.88666044817569,
					86.04922520672608
				],
				[
					34.64814629402008,
					86.81071105257035
				],
				[
					35.40963213986424,
					87.57221432770837
				],
				[
					35.98075523889429,
					88.14333742673841
				],
				[
					36.36151559111022,
					88.71446052576846
				],
				[
					36.36151559111022,
					88.90484070187642
				],
				[
					36.36151559111022,
					89.09520344869054
				],
				[
					36.36151559111022,
					89.2855836247985
				],
				[
					36.36151559111022,
					89.66632654772059
				],
				[
					36.36151559111022,
					90.04708689993652
				],
				[
					36.36151559111022,
					90.61820999896656
				],
				[
					36.36151559111022,
					91.18933309799672
				],
				[
					36.36151559111022,
					91.95081894384089
				],
				[
					36.36151559111022,
					92.52194204287105
				],
				[
					36.1711528442961,
					93.47382549411702
				],
				[
					36.1711528442961,
					94.23531133996119
				],
				[
					36.1711528442961,
					95.18719479120716
				],
				[
					35.98075523889429,
					95.94868063705132
				],
				[
					35.79039249208017,
					96.9005640882973
				],
				[
					35.600029745266056,
					97.66204993414158
				],
				[
					35.40963213986424,
					98.42355320927959
				],
				[
					35.02890664623578,
					99.1850564844176
				],
				[
					34.26738594180415,
					100.32730268247781
				],
				[
					33.696262842774104,
					101.27916870442994
				],
				[
					32.36365389789967,
					102.23103472638218
				],
				[
					30.650284600809528,
					103.18291817762815
				],
				[
					28.55615495150346,
					104.32516437568825
				],
				[
					26.08129980856893,
					105.27703039764049
				],
				[
					22.844923961202767,
					106.60965677180855
				],
				[
					19.037459873394027,
					108.13264589279072
				],
				[
					15.420323673811936,
					109.08451191474296
				],
				[
					11.612859586003196,
					110.22675811280305
				],
				[
					7.614997892792644,
					111.36900431086326
				],
				[
					3.617136199582319,
					112.51125050892335
				],
				[
					-0.3807254936282334,
					113.65349670698345
				],
				[
					-4.378587186838786,
					114.41499998212146
				],
				[
					-6.6630795829589715,
					114.98612308115162
				],
				[
					-10.280215782541063,
					115.55724618018166
				],
				[
					-13.70695437672157,
					116.12836927921171
				],
				[
					-17.324055717716192,
					116.50911220213379
				],
				[
					-21.1315546641124,
					116.88987255434972
				],
				[
					-25.31977910413707,
					117.46099565337977
				],
				[
					-28.55615495150346,
					117.651358400194
				],
				[
					-31.982893545683737,
					118.22248149922405
				],
				[
					-35.40963213986424,
					118.79360459825409
				],
				[
					-38.83637073404452,
					119.36472769728414
				],
				[
					-41.31122587697905,
					119.93585079631418
				],
				[
					-43.59571827309924,
					120.88773424756016
				],
				[
					-45.49945031700372,
					121.64922009340444
				],
				[
					-47.21281961409386,
					122.02998044562037
				],
				[
					-48.73582616436988,
					122.9818464675725
				],
				[
					-49.68770961561586,
					123.17222664368046
				],
				[
					-50.639558208274366,
					123.55296956660266
				],
				[
					-51.59144165952034,
					124.1240926656327
				],
				[
					-52.352927505364505,
					124.31447284174067
				],
				[
					-53.4951737034246,
					124.50483558855478
				],
				[
					-54.447057154670574,
					124.88559594077071
				],
				[
					-55.58930335273067,
					124.88559594077071
				],
				[
					-56.73154955079076,
					125.2663388636928
				],
				[
					-58.25455610106678,
					125.45671903980076
				],
				[
					-59.01604194691117,
					125.45671903980076
				],
				[
					-59.96792539815715,
					125.64708178661488
				],
				[
					-60.158288144971266,
					125.64708178661488
				],
				[
					-60.34865089178538,
					125.64708178661488
				],
				[
					-60.158288144971266,
					125.45671903980076
				],
				[
					-59.58716504594122,
					124.69521576466275
				],
				[
					-58.63528159469524,
					123.74334974271062
				],
				[
					-57.302672649820806,
					122.60110354465041
				],
				[
					-56.54118680397664,
					121.64922009340444
				],
				[
					-54.25669440785646,
					119.74548804950007
				],
				[
					-52.733687857580435,
					118.41286167533201
				],
				[
					-50.44919546146002,
					116.50911220213379
				],
				[
					-47.21281961409386,
					113.84387688309141
				],
				[
					-44.54760172434521,
					111.94012740989331
				],
				[
					-41.120863130164935,
					109.08451191474296
				],
				[
					-37.3133641837685,
					105.65777332056257
				],
				[
					-34.07698833640234,
					102.80215782541222
				],
				[
					-30.459886995407714,
					99.1850564844176
				],
				[
					-26.652388049011506,
					94.80643443899123
				],
				[
					-24.177532906076976,
					91.95081894384089
				],
				[
					-20.75079431189647,
					87.95295725063045
				],
				[
					-18.275939168962168,
					84.52621865645006
				],
				[
					-15.420323673811936,
					80.90911731545543
				],
				[
					-11.99358507963143,
					76.72087544613703
				],
				[
					-9.709092683511017,
					73.4845170280646
				],
				[
					-6.472716836144855,
					69.2962751587462
				],
				[
					-3.9978616932105524,
					66.25027948748789
				],
				[
					-1.5229716916885536,
					63.585044168445506
				],
				[
					1.1422461980600929,
					60.539048497187196
				],
				[
					3.426738594180506,
					57.873813178144815
				],
				[
					5.711230990300692,
					55.779692243485556
				],
				[
					7.043874793762598,
					54.06632294639542
				],
				[
					8.18612099182269,
					52.73370528687417
				],
				[
					8.947606837666854,
					51.78183055027512
				],
				[
					9.5187299366969,
					51.40107891270611
				],
				[
					9.709092683511244,
					50.829955813676065
				],
				[
					10.28021578254129,
					50.449212890753984
				],
				[
					10.66097613475722,
					50.449212890753984
				],
				[
					11.232099233787267,
					50.068461253184864
				],
				[
					11.803222332817313,
					49.68770961561586
				],
				[
					12.564708178661476,
					49.30696669269378
				],
				[
					13.135831277691523,
					49.11658651658581
				],
				[
					13.70695437672157,
					48.73584359366373
				],
				[
					13.897351982123382,
					48.355091956094725
				],
				[
					14.087714728937499,
					48.355091956094725
				],
				[
					14.087714728937499,
					48.92621505512477
				],
				[
					14.087714728937499,
					50.25883271464602
				],
				[
					13.897351982123382,
					52.352953649305164
				],
				[
					13.897351982123382,
					54.827817506886504
				],
				[
					13.897351982123382,
					58.254556101066896
				],
				[
					13.897351982123382,
					60.539048497187196
				],
				[
					13.897351982123382,
					63.39466399233754
				],
				[
					13.897351982123382,
					66.44065966359585
				],
				[
					13.70695437672157,
					68.53477188360819
				],
				[
					13.516591629907452,
					71.77114773097435
				],
				[
					12.945468530877406,
					75.00750614904689
				],
				[
					12.564708178661476,
					78.62462491933513
				],
				[
					11.803222332817313,
					83.38397245838985
				],
				[
					11.232099233787267,
					86.42996812964816
				],
				[
					9.709092683511244,
					91.18933309799672
				],
				[
					8.757244090852737,
					95.18719479120716
				],
				[
					7.043874793762598,
					100.51766542929192
				],
				[
					5.330505496672458,
					104.32516437568825
				],
				[
					2.8556154951504595,
					108.70376899182088
				],
				[
					1.1422461980600929,
					111.36900431086326
				],
				[
					-0.9518485926582798,
					113.65349670698345
				],
				[
					-2.855615495150232,
					115.17650325725947
				],
				[
					-4.949710285868832,
					116.12836927921171
				],
				[
					-6.282354089330738,
					116.69949237824176
				],
				[
					-8.186086133234994,
					116.69949237824176
				],
				[
					-10.470578529355407,
					116.69949237824176
				],
				[
					-12.564708178661476,
					116.69949237824176
				],
				[
					-15.229926068410123,
					116.50911220213379
				],
				[
					-16.943295365500262,
					116.12836927921171
				],
				[
					-18.6566646625904,
					115.74762635628963
				],
				[
					-19.798910860650494,
					115.3668660040737
				],
				[
					-20.179671212866424,
					115.17650325725947
				],
				[
					-20.179671212866424,
					114.98612308115162
				],
				[
					-19.989308466052307,
					114.41499998212146
				],
				[
					-19.41818536702226,
					113.46313396016933
				],
				[
					-17.89517881674624,
					111.94012740989331
				],
				[
					-15.80104916744017,
					109.65563501377301
				],
				[
					-13.70695437672157,
					107.18077987083859
				],
				[
					-10.470578529355407,
					103.37328092444227
				],
				[
					-6.6630795829589715,
					99.94654233026188
				],
				[
					-2.47485514293453,
					96.13906081315929
				],
				[
					1.9037669024919524,
					91.76045619702677
				],
				[
					5.520868243486575,
					87.76259450381633
				],
				[
					9.13796958448097,
					84.14547573352786
				],
				[
					12.183982685033243,
					80.90911731545543
				],
				[
					14.468475081153429,
					78.43424474322728
				],
				[
					17.133692970902075,
					75.38824907196897
				],
				[
					18.656699521178098,
					73.67487977487872
				],
				[
					19.989308466052307,
					72.3422708300044
				],
				[
					21.1315546641124,
					71.2000246319443
				],
				[
					22.083438115358376,
					70.62890153291426
				],
				[
					22.27380086217272,
					70.43852135680629
				],
				[
					22.464198467574306,
					70.43852135680629
				],
				[
					22.65456121438865,
					70.43852135680629
				],
				[
					22.65456121438865,
					70.62890153291426
				],
				[
					22.27380086217272,
					71.58076755486638
				],
				[
					21.321952269514213,
					73.67487977487872
				],
				[
					19.79894571923819,
					76.34013252321495
				],
				[
					17.514453323118005,
					79.76687111739534
				],
				[
					14.468475081153429,
					83.38397245838985
				],
				[
					10.66097613475722,
					87.3818341516004
				],
				[
					6.091991342516621,
					91.76045619702677
				],
				[
					0.7615207044318595,
					96.71018391218945
				],
				[
					-4.7593475390547155,
					100.89842578150785
				],
				[
					-8.947571979079385,
					103.94440402347232
				],
				[
					-12.94543367228971,
					106.80001951862266
				],
				[
					-15.610686420626052,
					108.51338881571291
				],
				[
					-17.70481606993212,
					109.65563501377301
				],
				[
					-18.275939168962168,
					110.03639536598894
				],
				[
					-18.6566646625904,
					110.41713828891102
				],
				[
					-18.6566646625904,
					110.60751846501898
				],
				[
					-18.6566646625904,
					110.41713828891102
				],
				[
					-18.6566646625904,
					110.22675811280305
				],
				[
					-18.6566646625904,
					109.46527226695889
				],
				[
					-18.466301915776285,
					107.94226571668275
				],
				[
					-17.89517881674624,
					106.60965677180855
				],
				[
					-17.324055717716192,
					104.70590729861033
				],
				[
					-15.80104916744017,
					101.65991162735202
				],
				[
					-13.70695437672157,
					98.23317303317162
				],
				[
					-10.851338881571337,
					93.28344531800906
				],
				[
					-8.186086133234994,
					89.85670672382855
				],
				[
					-5.140107891270645,
					85.85884503061811
				],
				[
					-1.3326089448742096,
					81.09948006226966
				],
				[
					1.332643803461906,
					78.05350182030509
				],
				[
					3.8074989463964357,
					74.43638305001684
				],
				[
					6.091991342516621,
					71.58076755486638
				],
				[
					7.805360639606761,
					69.2962751587462
				],
				[
					9.328367189882783,
					67.58290586165595
				],
				[
					10.28021578254129,
					66.25027948748789
				],
				[
					10.851338881571337,
					65.4887849269968
				],
				[
					11.422461980601383,
					64.7272903665056
				],
				[
					11.612859586003196,
					64.53691019039763
				],
				[
					11.803222332817313,
					64.3465387289366
				],
				[
					11.612859586003196,
					64.3465387289366
				],
				[
					10.470613387942876,
					65.4887849269968
				],
				[
					8.376483738636807,
					67.58290586165595
				],
				[
					6.282354089330738,
					70.05777843388421
				],
				[
					3.426738594180506,
					73.86525995098668
				],
				[
					0.19039760540181305,
					78.62462491933513
				],
				[
					-3.426738594180506,
					84.33585590963582
				],
				[
					-7.805325781019064,
					90.8085727457808
				],
				[
					-12.374310573259663,
					97.2813070112195
				],
				[
					-16.752932618686145,
					103.18291817762815
				],
				[
					-20.37003395968054,
					108.13264589279072
				],
				[
					-23.225649454831,
					111.94012740989331
				],
				[
					-25.890902203167116,
					114.98612308115162
				],
				[
					-27.413908753443366,
					116.69949237824176
				],
				[
					-28.55615495150346,
					118.22248149922405
				],
				[
					-29.50800354416174,
					119.36472769728414
				],
				[
					-30.269524248593598,
					120.12623097242215
				],
				[
					-30.65024974222183,
					120.50697389534434
				],
				[
					-30.65024974222183,
					120.6973540714522
				],
				[
					-30.459886995407714,
					120.31661114853011
				],
				[
					-29.50800354416174,
					118.98398477436206
				],
				[
					-27.985031852473412,
					117.08023530116395
				],
				[
					-25.890902203167116,
					114.60538015822942
				],
				[
					-23.225649454831,
					111.17864156404903
				],
				[
					-20.37003395968054,
					107.94226571668275
				],
				[
					-16.56256987187203,
					103.94440402347232
				],
				[
					-14.08767987035003,
					101.08878852832197
				],
				[
					-11.23206437519957,
					97.85243011024954
				],
				[
					-9.709092683511017,
					95.94868063705132
				],
				[
					-8.186086133234994,
					94.42569151606915
				],
				[
					-7.424600287390831,
					93.28344531800906
				],
				[
					-6.853477188360785,
					92.90270239508686
				],
				[
					-7.424600287390831,
					93.66418824093114
				],
				[
					-9.328332331295087,
					95.56793771412924
				],
				[
					-11.422461980601383,
					97.85243011024954
				],
				[
					-15.420323673811936,
					101.27916870442994
				],
				[
					-20.179671212866424,
					104.89628747471829
				],
				[
					-25.700539456353,
					109.27489209085093
				],
				[
					-32.55401664471378,
					114.2246198060135
				],
				[
					-39.40749383307457,
					118.60324185143998
				],
				[
					-45.689847922405306,
					122.22034319243448
				],
				[
					-51.020318560490296,
					124.88559594077071
				],
				[
					-54.827817506886504,
					126.78932798467508
				],
				[
					-58.82567920009683,
					129.26420055690335
				],
				[
					-61.490897089845475,
					130.78718967788552
				],
				[
					-62.82354089330738,
					131.92943587594561
				],
				[
					-63.77538948596589,
					132.8813193271916
				],
				[
					-64.34651258499593,
					133.45244242622164
				],
				[
					-64.91763568402598,
					134.2139282720659
				],
				[
					-65.1080332894278,
					134.59468862428184
				],
				[
					-65.29839603624191,
					134.78505137109596
				],
				[
					-65.48875878305603,
					135.1658117233119
				],
				[
					-64.91763568402598,
					135.1658117233119
				],
				[
					-63.9657870913677,
					134.78505137109596
				],
				[
					-62.82354089330738,
					134.2139282720659
				],
				[
					-61.11017159621724,
					133.07168207400582
				],
				[
					-59.96792539815715,
					132.11981605205358
				],
				[
					-58.63528159469524,
					130.9775698539935
				],
				[
					-57.302672649820806,
					129.64494347982543
				],
				[
					-56.16042645176071,
					128.6930774578732
				],
				[
					-55.58930335273067,
					127.74121143592106
				],
				[
					-55.20854300051474,
					127.1700883368909
				],
				[
					-54.827817506886504,
					126.78932798467508
				],
				[
					-54.827817506886504,
					126.40858506175289
				],
				[
					-54.63741990148469,
					126.40858506175289
				],
				[
					-54.63741990148469,
					126.21820488564492
				],
				[
					-54.447057154670574,
					126.21820488564492
				],
				[
					-53.87593405564053,
					126.0278421388308
				],
				[
					-53.68557130882641,
					126.0278421388308
				],
				[
					-52.733687857580435,
					125.45671903980076
				],
				[
					-52.16256475855039,
					125.07595868758483
				],
				[
					-51.401078912706,
					124.69521576466275
				],
				[
					-51.020318560490296,
					124.1240926656327
				],
				[
					-50.44919546146002,
					123.55296956660266
				],
				[
					-49.68770961561586,
					122.79146629146464
				],
				[
					-48.73582616436988,
					121.8396002695124
				],
				[
					-47.40321721949567,
					120.6973540714522
				],
				[
					-45.49945031700372,
					119.17436495047002
				],
				[
					-43.02459517406919,
					117.46099565337977
				],
				[
					-39.59785657988891,
					114.98612308115162
				],
				[
					-35.21923453446243,
					112.32088776210924
				],
				[
					-29.127278050533505,
					108.89414916792873
				],
				[
					-23.796772553861047,
					106.0385336727785
				],
				[
					-17.133692970902075,
					102.80215782541222
				],
				[
					-10.851338881571337,
					99.1850564844176
				],
				[
					-4.568984792240599,
					96.13906081315929
				],
				[
					-0.5711230990300464,
					93.8545684170391
				],
				[
					3.2363758473663893,
					91.5700760209188
				],
				[
					7.043874793762598,
					89.66632654772059
				],
				[
					9.13796958448097,
					88.33371760284638
				],
				[
					10.851338881571337,
					87.19147140478628
				],
				[
					12.183982685033243,
					86.23958795354031
				],
				[
					13.135831277691523,
					86.04922520672608
				],
				[
					13.135831277691523,
					85.85884503061811
				],
				[
					13.326228883093336,
					85.85884503061811
				],
				[
					13.326228883093336,
					86.04922520672608
				],
				[
					12.564708178661476,
					86.81071105257035
				],
				[
					10.851338881571337,
					88.33371760284638
				],
				[
					9.13796958448097,
					90.61820999896656
				],
				[
					6.663114441546668,
					93.28344531800906
				],
				[
					4.1882592986123655,
					96.13906081315929
				],
				[
					1.9037669024919524,
					98.80429613220178
				],
				[
					0.38076035221592974,
					101.65991162735202
				],
				[
					-0.7614858458441631,
					104.13478419958028
				],
				[
					-1.1422461980600929,
					106.0385336727785
				],
				[
					-1.3326089448742096,
					107.37114261765271
				],
				[
					-1.3326089448742096,
					108.32302606889868
				],
				[
					-1.3326089448742096,
					108.89414916792873
				],
				[
					-1.3326089448742096,
					109.08451191474296
				],
				[
					-1.1422461980600929,
					109.08451191474296
				],
				[
					-1.1422461980600929,
					109.27489209085093
				],
				[
					-1.7133692970901393,
					109.84601518988097
				],
				[
					-2.47485514293453,
					110.22675811280305
				],
				[
					-3.236340988778693,
					110.98826138794118
				],
				[
					-4.188224440024669,
					111.55938448697123
				],
				[
					-4.7593475390547155,
					112.13050758600127
				],
				[
					-5.330470638084762,
					112.32088776210924
				],
				[
					-5.711230990300692,
					112.32088776210924
				],
				[
					-5.520833384898879,
					112.13050758600127
				],
				[
					-4.7593475390547155,
					110.98826138794118
				],
				[
					-3.236340988778693,
					109.08451191474296
				],
				[
					-2.0940947907186,
					107.56152279376067
				],
				[
					-0.1903627468141167,
					105.65777332056257
				],
				[
					2.094129649306069,
					103.37328092444227
				],
				[
					4.378622045426482,
					101.08878852832197
				],
				[
					6.472751694732551,
					98.99467630830975
				],
				[
					7.805360639606761,
					97.66204993414158
				],
				[
					8.376483738636807,
					96.71018391218945
				],
				[
					8.566846485450924,
					96.32944098926725
				],
				[
					8.18612099182269,
					96.51980373608149
				],
				[
					7.424600287390831,
					96.9005640882973
				],
				[
					6.663114441546668,
					97.2813070112195
				],
				[
					5.711230990300692,
					97.47168718732746
				],
				[
					4.759382397642412,
					97.66204993414158
				],
				[
					3.426738594180506,
					97.66204993414158
				],
				[
					0.5711230990300464,
					97.47168718732746
				],
				[
					-2.2844923961201857,
					97.09092683511153
				],
				[
					-7.043839935174901,
					96.13906081315929
				],
				[
					-12.94543367228971,
					95.18719479120716
				],
				[
					-19.41818536702226,
					93.8545684170391
				],
				[
					-25.129416357322953,
					93.09306514190109
				],
				[
					-30.269524248593598,
					92.90270239508686
				],
				[
					-33.12513974374383,
					92.90270239508686
				],
				[
					-35.21923453446243,
					93.09306514190109
				],
				[
					-35.79035763349248,
					93.47382549411702
				],
				[
					-35.21923453446243,
					93.66418824093114
				],
				[
					-34.07698833640234,
					94.04494859314707
				],
				[
					-32.36361903931197,
					94.23531133996119
				],
				[
					-30.459886995407714,
					94.23531133996119
				],
				[
					-27.604271500257482,
					94.23531133996119
				],
				[
					-24.748656005107023,
					94.04494859314707
				],
				[
					-20.941157058710814,
					92.71232221897901
				],
				[
					-16.372172266470216,
					91.76045619702677
				],
				[
					-11.041701628385454,
					90.04708689993652
				],
				[
					-7.234202681989018,
					88.5240803496605
				],
				[
					-2.47485514293453,
					87.00109122867832
				],
				[
					2.094129649306069,
					85.85884503061811
				],
				[
					5.711230990300692,
					84.71659883255802
				],
				[
					8.947606837666854,
					83.95509555742001
				],
				[
					11.422461980601383,
					83.76473281060578
				],
				[
					13.326228883093336,
					83.76473281060578
				],
				[
					14.658837827967545,
					83.95509555742001
				],
				[
					15.610721279213521,
					84.52621865645006
				],
				[
					16.56256987187203,
					85.28772193158807
				],
				[
					17.133692970902075,
					86.62034830575612
				],
				[
					17.514453323118005,
					88.5240803496605
				],
				[
					17.514453323118005,
					91.18933309799672
				],
				[
					17.514453323118005,
					93.8545684170391
				],
				[
					16.75296747727384,
					96.9005640882973
				],
				[
					15.420323673811936,
					99.94654233026188
				],
				[
					13.70695437672157,
					102.80215782541222
				],
				[
					11.232099233787267,
					105.84815349667053
				],
				[
					8.18612099182269,
					109.08451191474296
				],
				[
					5.520868243486575,
					111.17864156404903
				],
				[
					3.2363758473663893,
					113.0823736079534
				],
				[
					0.9518834512459762,
					114.41499998212146
				],
				[
					-0.5711230990300464,
					115.17650325725947
				],
				[
					-1.1422461980600929,
					115.74762635628963
				],
				[
					-0.5711230990300464,
					115.74762635628963
				],
				[
					0.7615207044318595,
					114.79574290504365
				],
				[
					2.665252748336343,
					113.0823736079534
				],
				[
					4.1882592986123655,
					111.55938448697123
				],
				[
					7.043874793762598,
					108.32302606889868
				],
				[
					9.13796958448097,
					105.65777332056257
				],
				[
					12.183982685033243,
					102.42141490249003
				],
				[
					14.84920057478189,
					98.99467630830975
				],
				[
					17.514453323118005,
					95.94868063705132
				],
				[
					19.79894571923819,
					93.09306514190109
				],
				[
					22.083438115358376,
					90.61820999896656
				],
				[
					23.796807412448743,
					88.90484070187642
				],
				[
					25.700539456353,
					87.57221432770837
				],
				[
					27.033183259814905,
					86.81071105257035
				],
				[
					28.365792204689342,
					86.42996812964816
				],
				[
					28.93691530371939,
					86.23958795354031
				],
				[
					29.69840114956355,
					86.23958795354031
				],
				[
					29.69840114956355,
					86.81071105257035
				],
				[
					29.317675655935318,
					87.3818341516004
				],
				[
					28.55615495150346,
					89.09520344869054
				],
				[
					27.60430635884495,
					90.42782982285871
				],
				[
					26.46206016078486,
					92.14119911994885
				],
				[
					24.74869086369472,
					94.23531133996119
				],
				[
					22.464198467574306,
					96.51980373608149
				],
				[
					20.370068818268237,
					98.61393338538755
				],
				[
					18.656699521178098,
					100.70804560539989
				],
				[
					17.324090576303888,
					102.61179507859799
				],
				[
					16.56256987187203,
					103.7540412766582
				],
				[
					16.372207125057912,
					104.51552712250248
				],
				[
					16.372207125057912,
					105.08665022153252
				],
				[
					16.94333022408796,
					105.08665022153252
				],
				[
					17.514453323118005,
					105.08665022153252
				],
				[
					18.656699521178098,
					104.89628747471829
				],
				[
					20.750829170484167,
					103.94440402347232
				],
				[
					22.27380086217272,
					102.42141490249003
				],
				[
					24.177567764664673,
					100.70804560539989
				],
				[
					25.890937061754812,
					98.23317303317162
				],
				[
					27.413908753443366,
					95.75831789023721
				],
				[
					28.175429457875225,
					93.47382549411702
				],
				[
					28.93691530371939,
					91.37969584481084
				],
				[
					29.127278050533505,
					90.04708689993652
				],
				[
					29.317675655935318,
					88.90484070187642
				],
				[
					29.317675655935318,
					88.33371760284638
				],
				[
					28.93691530371939,
					87.76259450381633
				],
				[
					28.55615495150346,
					87.3818341516004
				],
				[
					27.794669105659295,
					87.19147140478628
				],
				[
					27.22354600662925,
					87.19147140478628
				],
				[
					26.271662555383273,
					87.19147140478628
				],
				[
					25.510176709538882,
					87.19147140478628
				],
				[
					24.74869086369472,
					87.3818341516004
				],
				[
					24.36793051147879,
					88.5240803496605
				],
				[
					24.177567764664673,
					89.85670672382855
				],
				[
					23.98717015926286,
					91.95081894384089
				],
				[
					24.177567764664673,
					93.8545684170391
				],
				[
					24.939053610508836,
					96.13906081315929
				],
				[
					25.890937061754812,
					98.23317303317162
				],
				[
					27.22354600662925,
					99.5657994073398
				],
				[
					28.175429457875225,
					100.32730268247781
				],
				[
					28.93691530371939,
					100.70804560539989
				],
				[
					29.508038402749435,
					100.89842578150785
				],
				[
					30.45992185399541,
					100.89842578150785
				],
				[
					31.031044953025457,
					100.89842578150785
				],
				[
					31.79253079886962,
					100.70804560539989
				],
				[
					32.17329115108555,
					100.32730268247781
				],
				[
					32.36365389789967,
					99.5657994073398
				],
				[
					32.36365389789967,
					99.5657994073398
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 777,
			"versionNonce": 1968015344,
			"isDeleted": false,
			"id": "DBsufXFRwwQS9Psv1YmGm",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3268.8855057489054,
			"y": -501.13117428862654,
			"strokeColor": "#a18072",
			"backgroundColor": "transparent",
			"width": 238.7855183412239,
			"height": 89.46294759215272,
			"seed": 438292752,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.2176979523035243,
					-0.6530141432697292
				],
				[
					-0.43535604778639936,
					-1.3060282865393447
				],
				[
					-1.088370191056356,
					-2.6120565730786893
				],
				[
					-1.5237262388427553,
					-3.7004267641350452
				],
				[
					-2.394398477595587,
					-4.7887770267810765
				],
				[
					-3.2650707163484185,
					-6.530141432696837
				],
				[
					-4.135782811921445,
					-7.618511623753193
				],
				[
					-4.788796955191174,
					-9.142207969980745
				],
				[
					-5.659469193944005,
					-10.230568196831882
				],
				[
					-6.530141432696837,
					-11.53659648337134
				],
				[
					-7.400853528269863,
					-13.277960889287101
				],
				[
					-7.836169719236295,
					-14.583989175826446
				],
				[
					-8.706881814809321,
					-16.107695486259104
				],
				[
					-9.35989595807905,
					-17.63139183248677
				],
				[
					-9.795212149045483,
					-19.372766202607636
				],
				[
					-10.665924244618282,
					-21.331808632416596
				],
				[
					-11.536596483371113,
					-23.29085106222567
				],
				[
					-12.62496667442747,
					-25.249893492034744
				],
				[
					-13.713297008663403,
					-27.208935921843818
				],
				[
					-15.237023247506158,
					-29.16797835165289
				],
				[
					-16.543051534045617,
					-31.780034924731694
				],
				[
					-17.63138186828155,
					-33.521399330647455
				],
				[
					-18.93741015482101,
					-35.48044176045653
				],
				[
					-19.59042429809074,
					-37.00414807088919
				],
				[
					-20.461136393663764,
					-38.52784441711685
				],
				[
					-21.331808632416596,
					-39.61620464396799
				],
				[
					-21.767164680203223,
					-40.70455490661408
				],
				[
					-22.420178823472952,
					-42.01058319315348
				],
				[
					-23.073192966742454,
					-42.881275360316465
				],
				[
					-23.290851062225784,
					-43.96962562296255
				],
				[
					-24.161523300978615,
					-45.05798584981375
				],
				[
					-25.03223539655164,
					-46.79936021993461
				],
				[
					-25.68524953982137,
					-47.67004242289249
				],
				[
					-26.555921778574202,
					-48.976070709431895
				],
				[
					-27.426594017327034,
					-50.28209899597124
				],
				[
					-28.514964208383162,
					-51.80579534219885
				],
				[
					-29.603334399439518,
					-53.11182362873819
				],
				[
					-30.47400663819235,
					-54.63552993917085
				],
				[
					-31.56237682924848,
					-56.15922628539846
				],
				[
					-32.43304906800131,
					-57.247586512249654
				],
				[
					-33.08606321127104,
					-58.118268715207535
				],
				[
					-33.521419259057666,
					-59.20662894205873
				],
				[
					-33.95673545002387,
					-59.8596430853284
				],
				[
					-34.17443340232717,
					-60.51265722859807
				],
				[
					-34.6097495932936,
					-61.38333943155601
				],
				[
					-35.04510564108,
					-62.25402163451389
				],
				[
					-35.480461688866626,
					-63.124713801676876
				],
				[
					-36.35113392761946,
					-64.21306406432296
				],
				[
					-37.22180616637229,
					-65.51909235086237
				],
				[
					-37.87482030964202,
					-66.6074525777135
				],
				[
					-38.52783445291175,
					-67.9134808642529
				],
				[
					-39.616204643967876,
					-69.2195091507923
				],
				[
					-40.48687688272071,
					-70.30786937764344
				],
				[
					-41.13989102599044,
					-71.61389766418284
				],
				[
					-41.575247073777064,
					-72.48457986714072
				],
				[
					-42.01060312156346,
					-73.35526207009866
				],
				[
					-42.22826121704679,
					-74.00827621336833
				],
				[
					-42.445919312529895,
					-74.87896838053132
				],
				[
					-42.66361726483342,
					-75.31430449990773
				],
				[
					-42.66361726483342,
					-76.18499666707066
				],
				[
					-42.66361726483342,
					-76.62033278644708
				],
				[
					-42.881275360316295,
					-77.49102495361007
				],
				[
					-43.098933455799624,
					-78.36170715656795
				],
				[
					-43.53428950358625,
					-79.23238935952588
				],
				[
					-43.751947599069126,
					-80.10308152668881
				],
				[
					-44.18730364685575,
					-81.40910981322821
				],
				[
					-44.62265969464238,
					-82.2797920161861
				],
				[
					-45.057975885608585,
					-83.36815224303729
				],
				[
					-45.49333193339521,
					-84.67418052957669
				],
				[
					-45.710990028878314,
					-85.76253079222278
				],
				[
					-46.14634607666494,
					-86.63322295938576
				],
				[
					-46.14634607666494,
					-87.28623710265543
				],
				[
					-46.36400417214804,
					-87.9392512459251
				],
				[
					-46.58170212445134,
					-88.15691930561331
				],
				[
					-46.58170212445134,
					-88.59226538919484
				],
				[
					-46.58170212445134,
					-88.80993344888304
				],
				[
					-46.58170212445134,
					-89.24527953246451
				],
				[
					-46.58170212445134,
					-89.46294759215272
				],
				[
					-46.58170212445134,
					-89.24527953246451
				],
				[
					-47.01701831541777,
					-89.02760150857125
				],
				[
					-47.23471626772107,
					-88.59226538919484
				],
				[
					-47.45237436320417,
					-88.37458736530152
				],
				[
					-47.8877304109908,
					-88.15691930561331
				],
				[
					-48.323046601957,
					-87.50390516234364
				],
				[
					-48.75840264974363,
					-87.28623710265543
				],
				[
					-49.19375869753026,
					-86.85089101907397
				],
				[
					-50.06443093628309,
					-86.19787687580424
				],
				[
					-50.71744507955259,
					-85.76253079222278
				],
				[
					-51.805815270608946,
					-85.1095166489531
				],
				[
					-53.111843557148404,
					-84.23883444599517
				],
				[
					-54.417871843687635,
					-83.5858203027255
				],
				[
					-56.1592163211933,
					-82.93280615945582
				],
				[
					-57.46524460773276,
					-82.06212395649789
				],
				[
					-59.42428703754172,
					-81.40910981322821
				],
				[
					-61.383329467350904,
					-80.53841764606523
				],
				[
					-63.34237189716009,
					-79.88540350279555
				],
				[
					-65.51911227927235,
					-78.79705324014947
				],
				[
					-67.91347090004797,
					-78.14403909687974
				],
				[
					-70.74322542542996,
					-77.0556788700286
				],
				[
					-73.57294009399197,
					-76.62033278644708
				],
				[
					-76.62035271485729,
					-75.9673186431774
				],
				[
					-81.62676790871137,
					-75.09663644021953
				],
				[
					-83.36815224303723,
					-74.661290356638
				],
				[
					-86.85088105486898,
					-74.00827621336833
				],
				[
					-90.3336497235207,
					-73.35526207009866
				],
				[
					-94.46939267862194,
					-72.91992595072225
				],
				[
					-98.38747753824009,
					-72.48457986714072
				],
				[
					-102.30556239785824,
					-71.61389766418284
				],
				[
					-106.22364725747639,
					-70.96088352091317
				],
				[
					-109.92407402161143,
					-69.87252329406198
				],
				[
					-112.97144678565655,
					-69.0018410911041
				],
				[
					-116.6718735497916,
					-67.9134808642529
				],
				[
					-121.02531445719615,
					-66.3897845180253
				],
				[
					-123.20201498248844,
					-65.30142429117416
				],
				[
					-126.90244174662348,
					-63.995396004634756
				],
				[
					-130.385170558455,
					-62.689367718095355
				],
				[
					-132.5618710837473,
					-61.38333943155601
				],
				[
					-135.3916256091295,
					-60.294979204704816
				],
				[
					-137.78598422990467,
					-59.424297001746936
				],
				[
					-140.3980408029836,
					-58.33593677489574
				],
				[
					-142.57478118509607,
					-57.68292263162607
				],
				[
					-144.75148171038813,
					-57.02990848835634
				],
				[
					-147.14588018798372,
					-56.15922628539846
				],
				[
					-149.54023880875934,
					-55.94155822571025
				],
				[
					-151.4992812385683,
					-55.28854408244058
				],
				[
					-153.45832366837726,
					-54.85319799885906
				],
				[
					-155.19970800270335,
					-54.20018385558939
				],
				[
					-157.1587504325123,
					-53.76483777200792
				],
				[
					-159.3354509578046,
					-53.32950165263151
				],
				[
					-161.29449338761356,
					-52.24114142578031
				],
				[
					-163.47123376972627,
					-51.58812728251064
				],
				[
					-165.64793429501833,
					-50.717445079552704
				],
				[
					-167.82463482031062,
					-49.62908485270157
				],
				[
					-170.4366913933893,
					-48.75840264974369
				],
				[
					-172.6134317755018,
					-47.67004242289249
				],
				[
					-175.0077903962772,
					-47.01702827962282
				],
				[
					-176.96683282608615,
					-45.92866805277163
				],
				[
					-178.70821716041223,
					-45.275653909501955
				],
				[
					-180.6672595902212,
					-44.40497170654402
				],
				[
					-182.19094597224375,
					-43.751957563274345
				],
				[
					-183.4969742587832,
					-43.09894342000467
				],
				[
					-184.80300254532244,
					-42.66359733642315
				],
				[
					-185.8913727363788,
					-42.01058319315348
				],
				[
					-186.97974292743515,
					-42.01058319315348
				],
				[
					-188.5034293094575,
					-41.35756904988381
				],
				[
					-189.80945759599695,
					-41.1399009901956
				],
				[
					-191.1154858825364,
					-40.48688684692587
				],
				[
					-192.85687021686226,
					-40.26921878723766
				],
				[
					-194.59823462277814,
					-39.61620464396799
				],
				[
					-196.5572770525871,
					-38.96319050069826
				],
				[
					-198.29864145850297,
					-38.310176357428645
				],
				[
					-200.47536191220524,
					-37.657162214158916
				],
				[
					-202.43440434201443,
					-36.78647004699599
				],
				[
					-204.3934467718234,
					-36.13345590372626
				],
				[
					-206.13481117773927,
					-35.26277370076832
				],
				[
					-208.31153163144154,
					-34.609759557498705
				],
				[
					-209.18222379860458,
					-34.174413473917184
				],
				[
					-210.27057406125073,
					-33.73907735454077
				],
				[
					-211.35892432389664,
					-33.08606321127104
				],
				[
					-212.2296164910597,
					-32.433049068001424
				],
				[
					-213.10030865822273,
					-32.21537104410811
				],
				[
					-213.75332280149246,
					-31.780034924731694
				],
				[
					-215.0593510880317,
					-31.127020781461965
				],
				[
					-215.2770091835148,
					-31.127020781461965
				],
				[
					-216.80071549394756,
					-30.47400663819235
				],
				[
					-218.10674378048702,
					-30.03866055461083
				],
				[
					-219.41277206702625,
					-29.603314471029307
				],
				[
					-220.5011223296724,
					-29.16797835165289
				],
				[
					-222.67784278337467,
					-28.514964208383276
				],
				[
					-224.20154909380744,
					-28.079618124801755
				],
				[
					-225.94291349972332,
					-27.644272041220233
				],
				[
					-227.46661981015586,
					-27.208935921843818
				],
				[
					-228.77264809669532,
					-26.991257897950618
				],
				[
					-230.51401250261097,
					-26.555921778574202
				],
				[
					-230.94934862198738,
					-26.12057569499268
				],
				[
					-231.82004078915043,
					-26.12057569499268
				],
				[
					-232.25537690852684,
					-25.68522961141116
				],
				[
					-232.69073295631347,
					-25.46756155172295
				],
				[
					-232.90839105179657,
					-25.249893492034744
				],
				[
					-233.12606907568988,
					-25.249893492034744
				],
				[
					-233.34374709958297,
					-25.032215468141544
				],
				[
					-233.5614051950663,
					-24.814547408453336
				],
				[
					-233.7790832189596,
					-24.814547408453336
				],
				[
					-233.9967612428527,
					-24.814547408453336
				],
				[
					-234.2144193383358,
					-24.814547408453336
				],
				[
					-234.43209736222911,
					-24.59687934876513
				],
				[
					-234.86743348160553,
					-24.379201324871815
				],
				[
					-235.08511150549884,
					-24.379201324871815
				],
				[
					-235.52044762487526,
					-24.161533265183607
				],
				[
					-235.9558036726619,
					-23.9438652054954
				],
				[
					-236.173461768145,
					-23.9438652054954
				],
				[
					-236.3911397920383,
					-23.9438652054954
				],
				[
					-236.60881781593162,
					-23.9438652054954
				],
				[
					-236.82647591141472,
					-23.9438652054954
				],
				[
					-237.04415393530803,
					-24.161533265183607
				],
				[
					-237.26183195920134,
					-24.161533265183607
				],
				[
					-237.26183195920134,
					-24.379201324871815
				],
				[
					-237.04415393530803,
					-24.59687934876513
				],
				[
					-236.173461768145,
					-24.59687934876513
				],
				[
					-234.64977538612243,
					-24.59687934876513
				],
				[
					-232.25537690852684,
					-24.814547408453336
				],
				[
					-231.1670266458807,
					-24.814547408453336
				],
				[
					-228.99030619217842,
					-25.032215468141544
				],
				[
					-226.3782496190995,
					-25.46756155172295
				],
				[
					-222.89552080726799,
					-25.68522961141116
				],
				[
					-218.97743594764984,
					-26.12057569499268
				],
				[
					-213.97098089697556,
					-26.555921778574202
				],
				[
					-208.74686775081796,
					-26.991257897950618
				],
				[
					-201.7813901987447,
					-27.644272041220233
				],
				[
					-196.12194093321068,
					-27.861950065113547
				],
				[
					-189.15644345272722,
					-28.514964208383276
				],
				[
					-182.19094597224375,
					-28.95030032775969
				],
				[
					-175.66080453954692,
					-29.16797835165289
				],
				[
					-169.34836105915338,
					-29.603314471029307
				],
				[
					-163.90654996069247,
					-29.82099249492262
				],
				[
					-157.59410648029893,
					-30.47400663819235
				],
				[
					-153.8936797161639,
					-30.47400663819235
				],
				[
					-149.54023880875934,
					-30.691674697880558
				],
				[
					-145.18683775817476,
					-30.691674697880558
				],
				[
					-140.8333968507702,
					-30.691674697880558
				],
				[
					-137.78598422990467,
					-30.909342757568766
				],
				[
					-133.21488522701702,
					-30.909342757568766
				],
				[
					-129.51449831970217,
					-30.909342757568766
				],
				[
					-125.37871550778073,
					-30.909342757568766
				],
				[
					-120.58995840940975,
					-30.909342757568766
				],
				[
					-115.58350335873524,
					-30.909342757568766
				],
				[
					-110.57708816488116,
					-31.127020781461965
				],
				[
					-105.35297501872355,
					-31.127020781461965
				],
				[
					-100.7818760158359,
					-31.127020781461965
				],
				[
					-96.42843510843113,
					-31.127020781461965
				],
				[
					-92.51035024881298,
					-31.127020781461965
				],
				[
					-89.24527953246456,
					-31.127020781461965
				],
				[
					-87.06857900717227,
					-31.127020781461965
				],
				[
					-85.10953657736331,
					-31.127020781461965
				],
				[
					-83.58581033852056,
					-31.127020781461965
				],
				[
					-82.06212395649777,
					-30.909342757568766
				],
				[
					-80.75609566995854,
					-30.691674697880558
				],
				[
					-79.23240928793598,
					-30.256328614299036
				],
				[
					-76.83801081034039,
					-30.03866055461083
				],
				[
					-75.09662647601431,
					-29.603314471029307
				],
				[
					-72.70226785523914,
					-29.16797835165289
				],
				[
					-69.43719713889072,
					-28.514964208383276
				],
				[
					-66.1721264225423,
					-27.644272041220233
				],
				[
					-62.90705570619366,
					-26.77358983826241
				],
				[
					-59.64198498984524,
					-26.12057569499268
				],
				[
					-55.72390013022709,
					-25.032215468141544
				],
				[
					-53.32950165263151,
					-24.59687934876513
				],
				[
					-50.93510317503592,
					-23.9438652054954
				],
				[
					-48.75840264974363,
					-23.29085106222567
				],
				[
					-47.01701831541777,
					-22.855504978644262
				],
				[
					-45.49333193339521,
					-22.637836918956054
				],
				[
					-43.751947599069126,
					-21.984822775686325
				],
				[
					-42.445919312529895,
					-21.331808632416596
				],
				[
					-40.70457483502423,
					-20.67879448914698
				],
				[
					-38.52783445291175,
					-19.808102321983938
				],
				[
					-36.133475832136355,
					-18.719752059337907
				],
				[
					-33.08606321127104,
					-17.63139183248677
				],
				[
					-29.385636447135994,
					-16.32536354594731
				],
				[
					-26.555921778574202,
					-15.454681342989488
				],
				[
					-23.508509157708886,
					-14.366321116138238
				],
				[
					-20.461136393663764,
					-13.4956389131803
				],
				[
					-18.066737916068178,
					-12.842624769910685
				],
				[
					-16.10769548625899,
					-11.754264543059435
				],
				[
					-14.801667199719759,
					-11.318918459478027
				],
				[
					-13.930994960966927,
					-10.883582340101611
				],
				[
					-13.4956389131803,
					-10.883582340101611
				],
				[
					-13.277980817697198,
					-10.665904316208298
				],
				[
					-12.842624769910572,
					-10.44823625652009
				],
				[
					-12.62496667442747,
					-10.012890172938569
				],
				[
					-12.18961062664107,
					-9.795222113250475
				],
				[
					-11.536596483371113,
					-9.142207969980745
				],
				[
					-10.230568196831882,
					-8.271525767022808
				],
				[
					-8.706881814809321,
					-7.183155575966566
				],
				[
					-6.747839385000361,
					-6.312483337213735
				],
				[
					-4.5710990028876495,
					-5.00645505067439
				],
				[
					-2.8297545253819862,
					-4.353440907404661
				],
				[
					-1.306028286539231,
					-3.482748740241732
				],
				[
					0.21765809548310244,
					-2.8297345969720027
				],
				[
					1.3060282865394583,
					-2.394398477595587
				],
				[
					1.5236863820225608,
					-2.1767204537022735
				],
				[
					1.5236863820225608,
					-1.9590424298090738
				],
				[
					1.3060282865394583,
					-1.9590424298090738
				],
				[
					0.43531619096643226,
					-1.9590424298090738
				],
				[
					-0.43535604778639936,
					-2.1767204537022735
				],
				[
					-1.306028286539231,
					-2.1767204537022735
				],
				[
					-2.1767403821124844,
					-2.6120565730786893
				],
				[
					-3.2650707163484185,
					-2.8297345969720027
				],
				[
					-3.482768668651943,
					-3.047412620865316
				],
				[
					-3.9180848596181477,
					-3.047412620865316
				],
				[
					-4.135782811921445,
					-3.2650707163484185
				],
				[
					-4.353440907404774,
					-3.482748740241732
				],
				[
					-4.5710990028876495,
					-3.7004267641350452
				],
				[
					-4.788796955191174,
					-4.353440907404661
				],
				[
					-5.441811098460903,
					-5.224113146157492
				],
				[
					-6.312483337213735,
					-6.530141432696837
				],
				[
					-7.183155575966566,
					-8.053847743129609
				],
				[
					-8.706881814809321,
					-9.795222113250475
				],
				[
					-10.448226292314985,
					-11.754264543059435
				],
				[
					-12.18961062664107,
					-14.14865305645003
				],
				[
					-13.930994960966927,
					-16.32536354594731
				],
				[
					-15.890037390775888,
					-18.937420119026115
				],
				[
					-17.849079820585075,
					-21.114130608523396
				],
				[
					-19.808122250394035,
					-23.9438652054954
				],
				[
					-21.114150536933494,
					-25.68522961141116
				],
				[
					-22.637836918956054,
					-27.861950065113547
				],
				[
					-23.943865205495285,
					-29.82099249492262
				],
				[
					-24.596879348765015,
					-31.780034924731694
				],
				[
					-25.68524953982137,
					-33.73907735454077
				],
				[
					-26.555921778574202,
					-35.69811978434984
				],
				[
					-27.64429196963033,
					-37.657162214158916
				],
				[
					-28.95032025616979,
					-40.051540763344406
				],
				[
					-30.90936268597875,
					-43.31661147969288
				],
				[
					-32.21539097251821,
					-45.71099999308342
				],
				[
					-34.6097495932936,
					-48.54072462585037
				],
				[
					-36.786489975406084,
					-51.37045922282243
				],
				[
					-38.963190500698374,
					-54.20018385558939
				],
				[
					-40.922232930507334,
					-56.37689434508667
				],
				[
					-43.098933455799624,
					-58.77128285847721
				],
				[
					-43.96964555137265,
					-60.07731114501661
				],
				[
					-44.84031779012548,
					-61.38333943155601
				],
				[
					-45.27567383791211,
					-62.25402163451389
				],
				[
					-45.710990028878314,
					-62.90703577778356
				],
				[
					-45.92868798118184,
					-63.56004992105329
				],
				[
					-46.14634607666494,
					-64.21306406432296
				],
				[
					-46.36400417214804,
					-64.64841014790443
				],
				[
					-46.79936021993467,
					-65.30142429117416
				],
				[
					-47.01701831541777,
					-66.17210649413204
				],
				[
					-47.23471626772107,
					-66.82512063740171
				],
				[
					-47.6700324586875,
					-67.9134808642529
				],
				[
					-48.323046601957,
					-69.2195091507923
				],
				[
					-48.97606074522673,
					-70.09019135375019
				],
				[
					-49.62907488849646,
					-71.39621964028959
				],
				[
					-50.499786984069715,
					-72.48457986714072
				],
				[
					-50.93510317503592,
					-73.35526207009866
				],
				[
					-51.805815270608946,
					-74.661290356638
				],
				[
					-52.458829413878675,
					-75.53198252380099
				],
				[
					-52.89414560484488,
					-76.18499666707066
				],
				[
					-53.111843557148404,
					-76.40266472675887
				],
				[
					-53.32950165263151,
					-76.40266472675887
				],
				[
					-53.32950165263151,
					-76.62033278644708
				],
				[
					-53.32950165263151,
					-76.83801081034039
				],
				[
					-53.32950165263151,
					-77.0556788700286
				],
				[
					-53.32950165263151,
					-77.27334692971681
				],
				[
					-53.54715974811461,
					-77.0556788700286
				],
				[
					-54.20017389138434,
					-76.62033278644708
				],
				[
					-55.070885986957364,
					-75.7496505834892
				],
				[
					-55.941558225710196,
					-74.87896838053132
				],
				[
					-58.33595670330601,
					-73.57294009399192
				],
				[
					-59.859643085328344,
					-72.70224792682893
				],
				[
					-61.81868551513753,
					-71.83156572387105
				],
				[
					-64.64840018369932,
					-70.74320549701986
				],
				[
					-67.26045675677801,
					-69.65485523437377
				],
				[
					-71.17854161639639,
					-68.13114892394111
				],
				[
					-73.35528199850864,
					-67.26046672098323
				],
				[
					-76.83801081034039,
					-65.51909235086237
				],
				[
					-80.10308152668881,
					-64.21306406432296
				],
				[
					-83.36815224303723,
					-63.124713801676876
				],
				[
					-86.41556486390255,
					-62.25402163451389
				],
				[
					-89.02762143698124,
					-61.1656713718678
				],
				[
					-92.07499420102636,
					-60.294979204704816
				],
				[
					-95.5577628696783,
					-59.424297001746936
				],
				[
					-98.38747753824009,
					-58.988950918165415
				],
				[
					-101.87020635007184,
					-58.118268715207535
				],
				[
					-105.78829120968999,
					-57.02990848835634
				],
				[
					-109.0533619260384,
					-56.37689434508667
				],
				[
					-114.05981697671268,
					-55.50621214212879
				],
				[
					-116.6718735497916,
					-54.63552993917085
				],
				[
					-120.58995840940975,
					-53.76483777200792
				],
				[
					-124.07268722124127,
					-52.894155569049985
				],
				[
					-127.77311398537631,
					-52.023473366092105
				],
				[
					-130.6028286539381,
					-51.152781198929176
				],
				[
					-134.08559732259005,
					-50.06443093628303
				],
				[
					-137.13297008663517,
					-49.1937387691201
				],
				[
					-139.30971046874743,
					-48.323056566162165
				],
				[
					-141.48641099403972,
					-47.8877104825807
				],
				[
					-144.75148171038813,
					-47.01702827962282
				],
				[
					-146.49286604471422,
					-46.36401413635309
				],
				[
					-149.322580713276,
					-45.92866805277163
				],
				[
					-152.58765142962443,
					-45.49333193339521
				],
				[
					-155.41736609818645,
					-45.05798584981375
				],
				[
					-158.68243681453487,
					-44.40497170654402
				],
				[
					-161.94750753088329,
					-43.751957563274345
				],
				[
					-165.21257824723193,
					-43.09894342000467
				],
				[
					-168.04233277261392,
					-42.66359733642315
				],
				[
					-171.30740348896256,
					-42.228261217046736
				],
				[
					-173.26644591877152,
					-41.79291513346527
				],
				[
					-175.4431464440638,
					-41.1399009901956
				],
				[
					-177.61984696935588,
					-40.48688684692587
				],
				[
					-179.57888939916506,
					-40.051540763344406
				],
				[
					-181.53793182897402,
					-39.398526620074676
				],
				[
					-183.7146722110865,
					-38.310176357428645
				],
				[
					-185.23835859310907,
					-38.09249833353533
				],
				[
					-187.19740102291803,
					-37.4394841902656
				],
				[
					-188.93878535724411,
					-36.56880198730778
				],
				[
					-190.89782778705307,
					-36.13345590372626
				],
				[
					-192.42151416907564,
					-35.48044176045653
				],
				[
					-194.59823462277814,
					-34.609759557498705
				],
				[
					-195.68658488542405,
					-34.174413473917184
				],
				[
					-196.33959902869378,
					-33.73907735454077
				],
				[
					-196.9926131719635,
					-33.73907735454077
				],
				[
					-196.5572770525871,
					-33.73907735454077
				],
				[
					-196.12194093321068,
					-33.73907735454077
				],
				[
					-195.46892678994095,
					-33.73907735454077
				],
				[
					-194.38055659888482,
					-33.521399330647455
				],
				[
					-193.07452831234536,
					-33.521399330647455
				],
				[
					-191.1154858825364,
					-33.30373127095925
				],
				[
					-189.37410154821032,
					-33.30373127095925
				],
				[
					-187.19740102291803,
					-33.08606321127104
				],
				[
					-183.7146722110865,
					-32.86838518737784
				],
				[
					-181.32027373349092,
					-32.65071712768963
				],
				[
					-178.0552030171425,
					-32.65071712768963
				],
				[
					-174.57247420531098,
					-32.65071712768963
				],
				[
					-170.87204744117594,
					-32.65071712768963
				],
				[
					-166.51860653377116,
					-32.433049068001424
				],
				[
					-162.1652054831868,
					-32.433049068001424
				],
				[
					-158.24712062356866,
					-32.433049068001424
				],
				[
					-152.80530952510776,
					-31.997702984419902
				],
				[
					-148.45190847452318,
					-31.780034924731694
				],
				[
					-142.57478118509607,
					-30.909342757568766
				],
				[
					-136.47995594336544,
					-30.256328614299036
				],
				[
					-131.25584279720783,
					-29.603314471029307
				],
				[
					-124.725701364511,
					-28.514964208383276
				],
				[
					-120.15460236162312,
					-27.861950065113547
				],
				[
					-114.93048921546551,
					-26.77358983826241
				],
				[
					-108.8357038305553,
					-26.12057569499268
				],
				[
					-104.48226292315053,
					-25.46756155172295
				],
				[
					-99.91116392026265,
					-25.032215468141544
				],
				[
					-95.12240682189167,
					-24.161533265183607
				],
				[
					-91.63967801006015,
					-24.161533265183607
				],
				[
					-87.9392512459251,
					-23.726187181602086
				],
				[
					-84.02116638630696,
					-23.508519121913878
				],
				[
					-81.19145171774494,
					-23.29085106222567
				],
				[
					-77.92638100139652,
					-23.29085106222567
				],
				[
					-75.09662647601431,
					-23.07317303833247
				],
				[
					-72.26691180745252,
					-22.855504978644262
				],
				[
					-70.09021128216023,
					-22.637836918956054
				],
				[
					-66.82514056581181,
					-22.202490835374533
				],
				[
					-64.86609813600285,
					-21.984822775686325
				],
				[
					-62.68935775389036,
					-21.549476692104804
				],
				[
					-60.51265722859807,
					-21.331808632416596
				],
				[
					-58.553614798788885,
					-20.89646254883519
				],
				[
					-56.594572368979925,
					-20.24344840556546
				],
				[
					-54.417871843687635,
					-19.808102321983938
				],
				[
					-52.89414560484488,
					-19.59043426229573
				],
				[
					-51.15280112733922,
					-19.372766202607636
				],
				[
					-49.41141679301336,
					-19.155088178714323
				],
				[
					-47.8877304109908,
					-18.937420119026115
				],
				[
					-46.36400417214804,
					-18.937420119026115
				],
				[
					-44.18730364685575,
					-18.719752059337907
				],
				[
					-42.881275360316295,
					-18.502074035444593
				],
				[
					-41.13989102599044,
					-18.284405975756385
				],
				[
					-39.398546548484774,
					-18.066737916068178
				],
				[
					-38.310176357428645,
					-18.066737916068178
				],
				[
					-37.43950411867581,
					-18.066737916068178
				],
				[
					-36.56879202310279,
					-18.066737916068178
				],
				[
					-35.698119784349956,
					-17.63139183248677
				],
				[
					-34.6097495932936,
					-17.63139183248677
				],
				[
					-34.17443340232717,
					-17.41372377279845
				],
				[
					-33.08606321127104,
					-17.19604574890525
				],
				[
					-32.21539097251821,
					-16.97837768921704
				],
				[
					-31.12702078146208,
					-16.760709629528833
				],
				[
					-30.256348542709247,
					-16.54303160563552
				],
				[
					-29.603334399439518,
					-16.32536354594731
				],
				[
					-29.16797835165289,
					-16.32536354594731
				],
				[
					-29.16797835165289,
					-16.107695486259104
				],
				[
					-29.16797835165289,
					-16.32536354594731
				],
				[
					-28.95032025616979,
					-16.760709629528833
				],
				[
					-28.95032025616979,
					-18.066737916068178
				],
				[
					-28.95032025616979,
					-19.372766202607636
				],
				[
					-29.603334399439518,
					-20.89646254883519
				],
				[
					-30.47400663819235,
					-22.637836918956054
				],
				[
					-31.78003492473158,
					-24.379201324871815
				],
				[
					-32.86840511578794,
					-26.33824375468089
				],
				[
					-34.17443340232717,
					-27.861950065113547
				],
				[
					-35.26276373656333,
					-29.3856464113411
				],
				[
					-35.698119784349956,
					-30.256328614299036
				],
				[
					-36.35113392761946,
					-31.344688841150173
				],
				[
					-36.786489975406084,
					-32.433049068001424
				],
				[
					-37.00414807088919,
					-33.30373127095925
				],
				[
					-37.22180616637229,
					-34.174413473917184
				],
				[
					-37.87482030964202,
					-35.48044176045653
				],
				[
					-38.310176357428645,
					-37.00414807088919
				],
				[
					-38.745532405215044,
					-38.52784441711685
				],
				[
					-39.616204643967876,
					-40.051540763344406
				],
				[
					-40.70457483502423,
					-41.79291513346527
				],
				[
					-42.22826121704679,
					-43.96962562296255
				],
				[
					-43.53428950358625,
					-45.49333193339521
				],
				[
					-45.49333193339521,
					-47.452374363204285
				],
				[
					-47.23471626772107,
					-49.1937387691201
				],
				[
					-48.97606074522673,
					-50.717445079552704
				],
				[
					-50.499786984069715,
					-52.023473366092105
				],
				[
					-51.58811731830542,
					-52.894155569049985
				],
				[
					-52.24113146157538,
					-53.547169712319715
				],
				[
					-52.89414560484488,
					-53.98251579590118
				],
				[
					-53.111843557148404,
					-54.63552993917085
				],
				[
					-53.54715974811461,
					-55.07086605854727
				],
				[
					-53.982515795901236,
					-55.28854408244058
				],
				[
					-54.417871843687635,
					-55.94155822571025
				],
				[
					-54.85318803465407,
					-56.594572368979925
				],
				[
					-55.5062021779238,
					-57.46525457193786
				],
				[
					-55.941558225710196,
					-58.33593677489574
				],
				[
					-56.81223046446303,
					-59.424297001746936
				],
				[
					-57.46524460773276,
					-60.294979204704816
				],
				[
					-58.33595670330601,
					-61.38333943155601
				],
				[
					-58.98897084657551,
					-62.689367718095355
				],
				[
					-59.64198498984524,
					-63.56004992105329
				],
				[
					-59.859643085328344,
					-64.21306406432296
				],
				[
					-60.29499913311497,
					-64.86607820759264
				],
				[
					-60.51265722859807,
					-65.51909235086237
				],
				[
					-60.51265722859807,
					-66.17210649413204
				],
				[
					-60.730315324081175,
					-66.82512063740171
				],
				[
					-60.9480132763847,
					-67.47813478067144
				],
				[
					-60.9480132763847,
					-68.13114892394111
				],
				[
					-60.9480132763847,
					-69.0018410911041
				],
				[
					-61.1656713718678,
					-69.43717721048051
				],
				[
					-61.1656713718678,
					-70.30786937764344
				],
				[
					-61.383329467350904,
					-70.52553743733165
				],
				[
					-61.383329467350904,
					-70.96088352091317
				],
				[
					-61.60102741965443,
					-71.17855158060138
				],
				[
					-61.60102741965443,
					-70.96088352091317
				],
				[
					-61.81868551513753,
					-70.30786937764344
				],
				[
					-62.25404156292393,
					-69.43717721048051
				],
				[
					-62.90705570619366,
					-67.9134808642529
				],
				[
					-63.56006984946339,
					-66.6074525777135
				],
				[
					-64.43074208821622,
					-65.51909235086237
				],
				[
					-65.73677037475568,
					-63.77772794494655
				],
				[
					-67.47815470908154,
					-62.47169965840715
				],
				[
					-69.87251332985693,
					-60.73032528828628
				],
				[
					-72.48456990293562,
					-58.988950918165415
				],
				[
					-75.53198252380093,
					-57.68292263162607
				],
				[
					-79.01471133563268,
					-56.15922628539846
				],
				[
					-82.71513809976773,
					-55.07086605854727
				],
				[
					-86.85088105486898,
					-54.417851915277595
				],
				[
					-91.63967801006015,
					-53.32950165263151
				],
				[
					-95.12240682189167,
					-52.67648750936178
				],
				[
					-98.6051356337232,
					-52.24114142578031
				],
				[
					-103.17623463661107,
					-51.58812728251064
				],
				[
					-106.00598916199328,
					-51.152781198929176
				],
				[
					-109.70637606930813,
					-50.49976705565945
				],
				[
					-112.31843264238682,
					-49.62908485270157
				],
				[
					-115.14818716776904,
					-48.976070709431895
				],
				[
					-117.76024374084773,
					-47.8877104825807
				],
				[
					-119.93694426614002,
					-46.79936021993461
				],
				[
					-122.98435688700533,
					-45.49333193339521
				],
				[
					-125.37871550778073,
					-44.40497170654402
				],
				[
					-127.99077208085941,
					-43.53428950358614
				],
				[
					-131.03818470172473,
					-42.445929276734944
				],
				[
					-134.08559732259005,
					-41.575247073777064
				],
				[
					-137.35066803893847,
					-40.70455490661408
				],
				[
					-140.3980408029836,
					-40.051540763344406
				],
				[
					-143.2277953283658,
					-39.61620464396799
				],
				[
					-145.62215394914097,
					-39.18085856038647
				],
				[
					-148.23421052221988,
					-38.96319050069826
				],
				[
					-149.322580713276,
					-38.74551247680506
				],
				[
					-150.41095090433237,
					-38.52784441711685
				],
				[
					-151.4992812385683,
					-38.310176357428645
				],
				[
					-152.15229538183803,
					-38.310176357428645
				],
				[
					-152.36999333414133,
					-38.09249833353533
				],
				[
					-152.58765142962443,
					-37.874830273847124
				],
				[
					-153.02300747741106,
					-37.874830273847124
				],
				[
					-153.45832366837726,
					-37.4394841902656
				],
				[
					-154.111337811647,
					-36.78647004699599
				],
				[
					-154.76435195491672,
					-36.56880198730778
				],
				[
					-155.41736609818645,
					-35.91578784403805
				],
				[
					-156.07038024145618,
					-35.48044176045653
				],
				[
					-156.28807819375947,
					-35.26277370076832
				],
				[
					-156.5057362892428,
					-35.04510564108011
				],
				[
					-156.28807819375947,
					-35.04510564108011
				],
				[
					-155.85272214597285,
					-35.04510564108011
				],
				[
					-154.98204990722002,
					-35.04510564108011
				],
				[
					-153.67602162068079,
					-35.26277370076832
				],
				[
					-152.36999333414133,
					-35.48044176045653
				],
				[
					-150.84626709529857,
					-35.48044176045653
				],
				[
					-148.23421052221988,
					-35.48044176045653
				],
				[
					-146.2751680924107,
					-35.48044176045653
				],
				[
					-143.2277953283658,
					-35.48044176045653
				],
				[
					-139.09201251644413,
					-35.26277370076832
				],
				[
					-133.43258317932032,
					-34.82742761718691
				],
				[
					-128.64378622412914,
					-34.609759557498705
				],
				[
					-122.5490008392187,
					-34.3920914978105
				],
				[
					-115.58350335873524,
					-33.956745414228976
				],
				[
					-108.6180457350722,
					-33.956745414228976
				],
				[
					-101.21719220680211,
					-33.956745414228976
				],
				[
					-94.25173458313884,
					-33.956745414228976
				],
				[
					-88.15690934140821,
					-33.956745414228976
				],
				[
					-81.19145171774494,
					-33.956745414228976
				],
				[
					-74.87896838053143,
					-33.956745414228976
				],
				[
					-68.34882694783437,
					-33.956745414228976
				],
				[
					-62.036343610620634,
					-33.956745414228976
				],
				[
					-56.594572368979925,
					-33.956745414228976
				],
				[
					-51.15280112733922,
					-33.956745414228976
				],
				[
					-48.1053885064739,
					-33.956745414228976
				],
				[
					-45.057975885608585,
					-33.521399330647455
				],
				[
					-42.881275360316295,
					-33.30373127095925
				],
				[
					-41.13989102599044,
					-32.86838518737784
				],
				[
					-40.48687688272071,
					-32.65071712768963
				],
				[
					-39.833862739451206,
					-32.433049068001424
				],
				[
					-39.616204643967876,
					-32.21537104410811
				],
				[
					-39.398546548484774,
					-32.21537104410811
				],
				[
					-40.0515606917545,
					-32.433049068001424
				],
				[
					-41.35758897829396,
					-32.86838518737784
				],
				[
					-43.53428950358625,
					-33.30373127095925
				],
				[
					-46.14634607666494,
					-34.174413473917184
				],
				[
					-50.06443093628309,
					-35.91578784403805
				],
				[
					-53.54715974811461,
					-36.78647004699599
				],
				[
					-57.682942560036054,
					-38.310176357428645
				],
				[
					-62.47169965840726,
					-39.61620464396799
				],
				[
					-67.91347090004797,
					-42.01058319315348
				],
				[
					-72.26691180745252,
					-43.31661147969288
				],
				[
					-77.27336685812702,
					-44.84031779012554
				],
				[
					-83.58581033852056,
					-46.5816821960413
				],
				[
					-88.15690934140821,
					-47.67004242289249
				],
				[
					-93.16336439208271,
					-48.75840264974369
				],
				[
					-98.82283358602672,
					-49.62908485270157
				],
				[
					-102.52322049334157,
					-50.06443093628303
				],
				[
					-106.00598916199328,
					-50.28209899597124
				],
				[
					-108.8357038305553,
					-50.28209899597124
				],
				[
					-110.79474626036426,
					-50.28209899597124
				],
				[
					-111.6654184991171,
					-50.28209899597124
				],
				[
					-112.75378869017345,
					-50.06443093628303
				],
				[
					-112.75378869017345,
					-49.62908485270157
				],
				[
					-112.53613059469012,
					-49.846752912389775
				],
				[
					-111.6654184991171,
					-50.06443093628303
				],
				[
					-110.14173211709453,
					-50.28209899597124
				],
				[
					-108.40034778276868,
					-50.49976705565945
				],
				[
					-105.13527706642026,
					-50.93511313924091
				],
				[
					-99.91116392026265,
					-51.58812728251064
				],
				[
					-94.68705077410527,
					-52.24114142578031
				],
				[
					-87.721593150442,
					-52.894155569049985
				],
				[
					-80.53843757447544,
					-53.76483777200792
				],
				[
					-72.91992595072225,
					-54.20018385558939
				],
				[
					-66.1721264225423,
					-54.63552993917085
				],
				[
					-60.9480132763847,
					-54.85319799885906
				],
				[
					-57.247586512249654,
					-54.85319799885906
				],
				[
					-55.5062021779238,
					-54.85319799885906
				],
				[
					-54.635529939170965,
					-54.85319799885906
				],
				[
					-54.85318803465407,
					-53.76483777200792
				],
				[
					-55.72390013022709,
					-52.45880948546852
				],
				[
					-56.37691427349682,
					-51.152781198929176
				],
				[
					-57.682942560036054,
					-48.976070709431895
				],
				[
					-59.859643085328344,
					-46.36401413635309
				],
				[
					-62.90705570619366,
					-43.31661147969288
				],
				[
					-67.26045675677801,
					-40.051540763344406
				],
				[
					-71.83155575966589,
					-37.00414807088919
				],
				[
					-77.70868304909322,
					-34.609759557498705
				],
				[
					-82.2797820519811,
					-33.521399330647455
				],
				[
					-87.06857900717227,
					-32.433049068001424
				],
				[
					-91.63967801006015,
					-31.997702984419902
				],
				[
					-95.34006491737478,
					-31.997702984419902
				],
				[
					-98.38747753824009,
					-31.997702984419902
				],
				[
					-100.7818760158359,
					-32.433049068001424
				],
				[
					-102.08790430237514,
					-32.65071712768963
				],
				[
					-102.95857654112797,
					-33.08606321127104
				],
				[
					-102.95857654112797,
					-33.30373127095925
				],
				[
					-102.95857654112797,
					-33.73907735454077
				],
				[
					-102.52322049334157,
					-34.3920914978105
				],
				[
					-101.65254825458874,
					-35.26277370076832
				],
				[
					-100.34651996804928,
					-36.13345590372626
				],
				[
					-98.6051356337232,
					-37.221816130577395
				],
				[
					-95.7754209651614,
					-38.52784441711685
				],
				[
					-92.07499420102636,
					-40.48688684692587
				],
				[
					-88.59226538919484,
					-41.79291513346527
				],
				[
					-83.80350829082386,
					-43.31661147969288
				],
				[
					-79.01471133563268,
					-44.622639766232226
				],
				[
					-74.22595423726148,
					-45.92866805277163
				],
				[
					-69.65485523437383,
					-46.79936021993461
				],
				[
					-65.51911227927235,
					-47.23469633931103
				],
				[
					-62.90705570619366,
					-47.452374363204285
				],
				[
					-60.9480132763847,
					-47.452374363204285
				],
				[
					-60.07730118081167,
					-47.452374363204285
				],
				[
					-59.859643085328344,
					-47.452374363204285
				],
				[
					-60.07730118081167,
					-47.452374363204285
				],
				[
					-61.383329467350904,
					-47.01702827962282
				],
				[
					-63.56006984946339,
					-46.36401413635309
				],
				[
					-67.04279866129514,
					-45.92866805277163
				],
				[
					-72.04925371196941,
					-45.49333193339521
				],
				[
					-78.79705324014935,
					-45.05798584981375
				],
				[
					-84.89183862505979,
					-45.05798584981375
				],
				[
					-92.51035024881298,
					-45.05798584981375
				],
				[
					-99.69350582477955,
					-45.05798584981375
				],
				[
					-106.87666140074612,
					-45.275653909501955
				],
				[
					-112.75378869017345,
					-45.49333193339521
				],
				[
					-117.97790183633083,
					-45.71099999308342
				],
				[
					-121.46063064816258,
					-45.71099999308342
				],
				[
					-123.85502912575816,
					-45.71099999308342
				],
				[
					-124.725701364511,
					-45.71099999308342
				],
				[
					-125.37871550778073,
					-45.71099999308342
				],
				[
					-125.16105741229762,
					-45.92866805277163
				],
				[
					-124.07268722124127,
					-45.92866805277163
				],
				[
					-122.11364479143208,
					-45.92866805277163
				],
				[
					-119.28393012287029,
					-46.146346076664884
				],
				[
					-115.14818716776904,
					-46.146346076664884
				],
				[
					-109.92407402161143,
					-46.5816821960413
				],
				[
					-103.8292487798808,
					-46.79936021993461
				],
				[
					-98.38747753824009,
					-47.01702827962282
				],
				[
					-91.85733610554325,
					-47.23469633931103
				],
				[
					-85.76255072063282,
					-47.23469633931103
				],
				[
					-81.19145171774494,
					-47.23469633931103
				],
				[
					-78.36169719236295,
					-47.23469633931103
				],
				[
					-77.0556689058235,
					-47.23469633931103
				],
				[
					-76.83801081034039,
					-47.23469633931103
				],
				[
					-76.83801081034039,
					-47.01702827962282
				],
				[
					-76.83801081034039,
					-46.5816821960413
				],
				[
					-77.49102495361012,
					-45.92866805277163
				],
				[
					-78.57939514466625,
					-45.05798584981375
				],
				[
					-80.32073962217191,
					-43.751957563274345
				],
				[
					-82.4974800042844,
					-42.228261217046736
				],
				[
					-85.32719467284642,
					-40.70455490661408
				],
				[
					-89.24527953246456,
					-39.18085856038647
				],
				[
					-94.25173458313884,
					-37.874830273847124
				],
				[
					-98.82283358602672,
					-36.56880198730778
				],
				[
					-103.6115906843977,
					-36.13345590372626
				],
				[
					-107.96503159180247,
					-35.69811978434984
				],
				[
					-111.88311645142062,
					-35.69811978434984
				],
				[
					-114.27747507219578,
					-35.48044176045653
				],
				[
					-115.58350335873524,
					-35.26277370076832
				],
				[
					-116.01885940652187,
					-35.26277370076832
				],
				[
					-115.58350335873524,
					-35.91578784403805
				],
				[
					-115.14818716776904,
					-36.78647004699599
				],
				[
					-114.71283111998241,
					-37.221816130577395
				],
				[
					-113.62446092892628,
					-37.874830273847124
				],
				[
					-112.53613059469012,
					-38.52784441711685
				],
				[
					-110.79474626036426,
					-39.18085856038647
				],
				[
					-108.8357038305553,
					-39.8338727036562
				],
				[
					-105.57063311420666,
					-40.48688684692587
				],
				[
					-102.95857654112797,
					-41.1399009901956
				],
				[
					-100.56417806353238,
					-41.79291513346527
				],
				[
					-99.25814977699292,
					-42.445929276734944
				],
				[
					-99.04049168150982,
					-42.66359733642315
				],
				[
					-99.91116392026265,
					-42.66359733642315
				],
				[
					-100.99953411131901,
					-42.66359733642315
				],
				[
					-102.08790430237514,
					-42.66359733642315
				],
				[
					-103.3939325889146,
					-42.66359733642315
				],
				[
					-104.26460482766743,
					-42.445929276734944
				],
				[
					-104.91761897093716,
					-42.445929276734944
				],
				[
					-103.6115906843977,
					-42.01058319315348
				],
				[
					-100.99953411131901,
					-41.575247073777064
				],
				[
					-97.73446339497036,
					-40.70455490661408
				],
				[
					-92.29269215332988,
					-40.051540763344406
				],
				[
					-85.32719467284642,
					-39.61620464396799
				],
				[
					-77.70868304909322,
					-39.398526620074676
				],
				[
					-69.87251332985693,
					-39.398526620074676
				],
				[
					-62.25404156292393,
					-39.398526620074676
				],
				[
					-55.941558225710196,
					-39.398526620074676
				],
				[
					-51.37045922282255,
					-39.61620464396799
				],
				[
					-48.97606074522673,
					-40.051540763344406
				],
				[
					-47.45237436320417,
					-40.26921878723766
				],
				[
					-46.79936021993467,
					-40.26921878723766
				],
				[
					-46.58170212445134,
					-40.26921878723766
				],
				[
					-46.58170212445134,
					-40.48688684692587
				],
				[
					-46.36400417214804,
					-40.92223293050739
				],
				[
					-46.36400417214804,
					-41.35756904988381
				],
				[
					-46.36400417214804,
					-41.79291513346527
				],
				[
					-46.58170212445134,
					-42.445929276734944
				],
				[
					-46.79936021993467,
					-42.66359733642315
				],
				[
					-47.23471626772107,
					-43.31661147969288
				],
				[
					-47.45237436320417,
					-43.751957563274345
				],
				[
					-47.6700324586875,
					-43.96962562296255
				],
				[
					-47.8877304109908,
					-44.18730364685581
				],
				[
					-48.323046601957,
					-44.622639766232226
				],
				[
					-48.54074455426053,
					-45.05798584981375
				],
				[
					-48.75840264974363,
					-45.71099999308342
				],
				[
					-49.41141679301336,
					-46.36401413635309
				],
				[
					-50.28208903176619,
					-47.67004242289249
				],
				[
					-51.37045922282255,
					-48.54072462585037
				],
				[
					-52.67648750936178,
					-49.846752912389775
				],
				[
					-53.76485770041813,
					-50.717445079552704
				],
				[
					-54.85318803465407,
					-51.37045922282243
				],
				[
					-55.941558225710196,
					-52.023473366092105
				],
				[
					-56.1592163211933,
					-52.023473366092105
				],
				[
					-56.1592163211933,
					-52.24114142578031
				],
				[
					-56.1592163211933,
					-52.24114142578031
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 246,
			"versionNonce": 1412893168,
			"isDeleted": false,
			"id": "iTIIfeu5nqJuycf-lLgv7",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3274.183368435781,
			"y": -487.25284978874754,
			"strokeColor": "#846358",
			"backgroundColor": "transparent",
			"width": 277.10716921767767,
			"height": 36.49545648596484,
			"seed": 1982017296,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.3229785849152904
				],
				[
					-0.32294901624527483,
					-0.6459276011603379
				],
				[
					-0.9689061860758557,
					-0.968906186075742
				],
				[
					-0.9689061860758557,
					-1.2918847709910324
				],
				[
					-1.6148633559064365,
					-1.6148337872361935
				],
				[
					-2.2607613883967588,
					-2.2607909570667744
				],
				[
					-2.583769541982292,
					-2.583739973312049
				],
				[
					-2.9067185582273396,
					-2.9067185582273396
				],
				[
					-3.552675728058148,
					-3.22969714314263
				],
				[
					-3.8756247443031953,
					-3.22969714314263
				],
				[
					-4.5215819141340035,
					-3.22969714314263
				],
				[
					-4.8445309303788235,
					-3.22969714314263
				],
				[
					-5.167479946624098,
					-3.552646159387791
				],
				[
					-5.490488100209632,
					-3.552646159387791
				],
				[
					-5.813437116454679,
					-3.552646159387791
				],
				[
					-6.459394286285487,
					-3.552646159387791
				],
				[
					-6.782343302530535,
					-3.8756247443030816
				],
				[
					-7.10529231877581,
					-3.8756247443030816
				],
				[
					-7.7512494886063905,
					-4.198603329218486
				],
				[
					-8.397206658436971,
					-4.198603329218486
				],
				[
					-8.720155674682246,
					-4.521552345463533
				],
				[
					-9.689061860758102,
					-4.8445309303788235
				],
				[
					-10.335019030588683,
					-4.8445309303788235
				],
				[
					-10.65796804683373,
					-5.167509515294228
				],
				[
					-11.626874232909586,
					-5.490458531539389
				],
				[
					-12.272831402740394,
					-5.490458531539389
				],
				[
					-12.595780418985214,
					-5.813437116454679
				],
				[
					-13.241737588816022,
					-5.813437116454679
				],
				[
					-13.56468660506107,
					-6.459364717615131
				],
				[
					-13.887635621306345,
					-6.459364717615131
				],
				[
					-14.210643774891878,
					-6.459364717615131
				],
				[
					-14.533592791136925,
					-6.459364717615131
				],
				[
					-14.8565418073822,
					-6.459364717615131
				],
				[
					-14.8565418073822,
					-6.782343302530535
				],
				[
					-15.179549960967506,
					-6.782343302530535
				],
				[
					-15.502498977212781,
					-6.782343302530535
				],
				[
					-15.825447993457828,
					-6.782343302530535
				],
				[
					-16.148456147043362,
					-6.782343302530535
				],
				[
					-16.794354179533684,
					-7.105321887445825
				],
				[
					-17.440311349364492,
					-7.428270903690873
				],
				[
					-18.40921753544012,
					-8.074228073521681
				],
				[
					-19.05517470527093,
					-8.397177089766728
				],
				[
					-19.701072737761024,
					-8.720155674682019
				],
				[
					-20.66997892383688,
					-8.720155674682019
				],
				[
					-21.31593609366746,
					-9.043134259597423
				],
				[
					-21.96189326349804,
					-9.366083275842584
				],
				[
					-22.60779129598859,
					-9.689061860757874
				],
				[
					-23.25374846581917,
					-9.689061860757874
				],
				[
					-23.899705635649752,
					-10.012040445673165
				],
				[
					-24.545603668139847,
					-10.334989461918326
				],
				[
					-25.191560837970655,
					-10.65796804683373
				],
				[
					-25.514509854215703,
					-10.65796804683373
				],
				[
					-26.16046702404651,
					-10.65796804683373
				],
				[
					-27.12937321012214,
					-10.98094663174902
				],
				[
					-28.098279396197995,
					-11.626874232909472
				],
				[
					-29.06718558227385,
					-12.272801834069924
				],
				[
					-30.359040784594754,
					-12.595780418985214
				],
				[
					-31.973904140501418,
					-13.24170802014578
				],
				[
					-33.588767496407854,
					-13.88766518997636
				],
				[
					-34.88062269872853,
					-14.533592791136925
				],
				[
					-37.141384087125516,
					-15.179520392297263
				],
				[
					-38.75624744303195,
					-15.825477562128071
				],
				[
					-40.69405981518344,
					-16.47140516328841
				],
				[
					-41.98591501750434,
					-16.794383748203813
				],
				[
					-43.600778373410776,
					-17.117332764448975
				],
				[
					-44.89263357573191,
					-17.763289934279555
				],
				[
					-46.18454791539307,
					-18.086238950524717
				],
				[
					-46.83044594788316,
					-18.73219612035541
				],
				[
					-47.47640311771397,
					-19.05514513660046
				],
				[
					-48.44530930378983,
					-19.05514513660046
				],
				[
					-48.768258320034874,
					-19.378123721515863
				],
				[
					-49.414215489865455,
					-19.701102306431153
				],
				[
					-50.06017265969626,
					-20.347029907591605
				],
				[
					-50.706070692186586,
					-20.347029907591605
				],
				[
					-51.67497687826244,
					-20.67000849250701
				],
				[
					-52.32093404809302,
					-21.31593609366746
				],
				[
					-53.28984023416888,
					-21.63891467858275
				],
				[
					-54.258746420244734,
					-21.961863694827912
				],
				[
					-54.904703590075314,
					-22.284842279743202
				],
				[
					-55.87360977615117,
					-22.607820864658606
				],
				[
					-56.519507808641265,
					-22.930769880903654
				],
				[
					-57.165464978471846,
					-22.930769880903654
				],
				[
					-58.1343711645477,
					-23.253748465819058
				],
				[
					-58.78032833437851,
					-23.57672705073435
				],
				[
					-59.74923452045414,
					-23.89967606697951
				],
				[
					-60.39513255294446,
					-24.2226546518948
				],
				[
					-61.364038739020316,
					-24.545633236810204
				],
				[
					-62.009995908851124,
					-24.545633236810204
				],
				[
					-62.97890209492675,
					-24.545633236810204
				],
				[
					-63.94780828100238,
					-25.191560837970655
				],
				[
					-64.91671446707824,
					-25.514539422885946
				],
				[
					-66.20856966939937,
					-26.160467024046397
				],
				[
					-67.8234330253058,
					-26.4834456089618
				],
				[
					-69.11528822762648,
					-26.80639462520685
				],
				[
					-70.4072025672881,
					-26.80639462520685
				],
				[
					-72.02200678585405,
					-27.452351795037544
				],
				[
					-72.9909129719299,
					-27.452351795037544
				],
				[
					-74.60577632783634,
					-27.775300811282705
				],
				[
					-75.5746825139122,
					-28.098279396197995
				],
				[
					-77.51249488606368,
					-28.421257981113285
				],
				[
					-78.80435008838458,
					-28.421257981113285
				],
				[
					-80.09626442804597,
					-28.421257981113285
				],
				[
					-81.38811963036687,
					-28.744206997358447
				],
				[
					-83.00298298627331,
					-29.06718558227385
				],
				[
					-84.29483818859421,
					-29.39016416718914
				],
				[
					-85.90970154450088,
					-29.713113183434302
				],
				[
					-87.52450576306683,
					-30.359070353264997
				],
				[
					-89.13936911897326,
					-30.359070353264997
				],
				[
					-90.43122432129417,
					-30.682019369510044
				],
				[
					-92.0460876772006,
					-31.004997954425335
				],
				[
					-93.98390004935209,
					-31.6509255555859
				],
				[
					-95.27575525167322,
					-31.97390414050119
				],
				[
					-96.56766959133438,
					-32.29688272541648
				],
				[
					-97.85952479365551,
					-32.61983174166164
				],
				[
					-99.15137999597619,
					-32.61983174166164
				],
				[
					-100.4432943356378,
					-32.942810326577046
				],
				[
					-101.73514953795848,
					-32.942810326577046
				],
				[
					-102.70405572403433,
					-33.265788911492336
				],
				[
					-103.99591092635546,
					-33.265788911492336
				],
				[
					-105.28782526601663,
					-33.91171651265279
				],
				[
					-106.57968046833753,
					-33.91171651265279
				],
				[
					-108.19454382424419,
					-34.23469509756819
				],
				[
					-109.48639902656487,
					-34.23469509756819
				],
				[
					-110.45530521264072,
					-34.23469509756819
				],
				[
					-111.74716041496163,
					-34.55764411381324
				],
				[
					-113.36202377086829,
					-34.88062269872853
				],
				[
					-114.00798094069887,
					-35.203601283643934
				],
				[
					-115.62278515926482,
					-35.526550299889095
				],
				[
					-116.59169134534068,
					-35.526550299889095
				],
				[
					-117.88360568500207,
					-35.849528884804386
				],
				[
					-119.49840990356802,
					-35.849528884804386
				],
				[
					-120.46731608964387,
					-36.172507469719676
				],
				[
					-122.08217944555031,
					-36.172507469719676
				],
				[
					-123.37403464787121,
					-36.49545648596484
				],
				[
					-124.98889800377765,
					-36.49545648596484
				],
				[
					-126.92671037592936,
					-36.49545648596484
				],
				[
					-128.5415737318358,
					-36.49545648596484
				],
				[
					-130.4793861039875,
					-36.49545648596484
				],
				[
					-132.417198476139,
					-36.49545648596484
				],
				[
					-134.35501084829048,
					-36.49545648596484
				],
				[
					-136.2928232204422,
					-36.49545648596484
				],
				[
					-138.2306355925939,
					-36.49545648596484
				],
				[
					-140.49139698099043,
					-36.49545648596484
				],
				[
					-141.78325218331133,
					-36.49545648596484
				],
				[
					-143.07516652297272,
					-36.49545648596484
				],
				[
					-144.36702172529363,
					-36.49545648596484
				],
				[
					-145.98188508120006,
					-36.49545648596484
				],
				[
					-146.95079126727592,
					-36.49545648596484
				],
				[
					-148.24264646959682,
					-36.49545648596484
				],
				[
					-149.53450167191772,
					-36.49545648596484
				],
				[
					-151.14936502782416,
					-36.49545648596484
				],
				[
					-152.76422838373082,
					-36.49545648596484
				],
				[
					-154.37903260229677,
					-36.49545648596484
				],
				[
					-156.6398531280338,
					-36.49545648596484
				],
				[
					-158.25465734659997,
					-36.172507469719676
				],
				[
					-159.8695207025064,
					-35.849528884804386
				],
				[
					-162.4532902444887,
					-35.849528884804386
				],
				[
					-164.06809446305465,
					-35.849528884804386
				],
				[
					-165.36000880271604,
					-35.526550299889095
				],
				[
					-166.65186400503694,
					-35.526550299889095
				],
				[
					-167.9437487760281,
					-35.526550299889095
				],
				[
					-168.58967637718843,
					-35.526550299889095
				],
				[
					-169.55858256326428,
					-35.526550299889095
				],
				[
					-170.52748874934014,
					-35.203601283643934
				],
				[
					-171.496394935416,
					-35.203601283643934
				],
				[
					-172.46530112149185,
					-35.203601283643934
				],
				[
					-173.757185892483,
					-35.203601283643934
				],
				[
					-175.3720196797192,
					-35.203601283643934
				],
				[
					-177.30983205187067,
					-34.88062269872853
				],
				[
					-179.24764442402238,
					-34.88062269872853
				],
				[
					-181.50843538108916,
					-34.88062269872853
				],
				[
					-184.0921753544012,
					-34.88062269872853
				],
				[
					-186.99889391262877,
					-34.55764411381324
				],
				[
					-189.25968486969555,
					-34.55764411381324
				],
				[
					-191.8434248430076,
					-34.55764411381324
				],
				[
					-194.1042158000746,
					-34.23469509756819
				],
				[
					-196.04202817222608,
					-34.23469509756819
				],
				[
					-197.6568619594625,
					-34.23469509756819
				],
				[
					-199.594674331614,
					-34.23469509756819
				],
				[
					-201.20953768752042,
					-34.23469509756819
				],
				[
					-202.50139288984133,
					-34.23469509756819
				],
				[
					-203.79327766083247,
					-34.23469509756819
				],
				[
					-205.08516243182362,
					-33.91171651265279
				],
				[
					-206.37701763414452,
					-33.91171651265279
				],
				[
					-208.31483000629623,
					-33.91171651265279
				],
				[
					-209.92969336220267,
					-33.588737927737384
				],
				[
					-211.86750573435438,
					-33.265788911492336
				],
				[
					-214.1282671227509,
					-32.942810326577046
				],
				[
					-216.38905807981791,
					-32.61983174166164
				],
				[
					-218.3268704519694,
					-32.61983174166164
				],
				[
					-220.91061042528145,
					-32.29688272541648
				],
				[
					-222.84842279743316,
					-32.29688272541648
				],
				[
					-224.78623516958464,
					-32.29688272541648
				],
				[
					-226.0781199405758,
					-32.29688272541648
				],
				[
					-228.0159323127275,
					-31.97390414050119
				],
				[
					-229.30781708371865,
					-31.97390414050119
				],
				[
					-229.95374468487898,
					-31.6509255555859
				],
				[
					-230.92265087095484,
					-31.6509255555859
				],
				[
					-231.8915570570307,
					-31.32797653934074
				],
				[
					-233.5063908442669,
					-31.32797653934074
				],
				[
					-234.79827561525804,
					-31.004997954425335
				],
				[
					-235.7671818013339,
					-30.682019369510044
				],
				[
					-237.38201558857008,
					-30.682019369510044
				],
				[
					-239.6428065456371,
					-30.359070353264997
				],
				[
					-241.58061891778857,
					-30.359070353264997
				],
				[
					-243.19545270502476,
					-30.036091768349593
				],
				[
					-245.13326507717647,
					-29.713113183434302
				],
				[
					-246.7481284330829,
					-29.39016416718914
				],
				[
					-248.3629622203191,
					-29.06718558227385
				],
				[
					-249.9777960075553,
					-29.06718558227385
				],
				[
					-251.59265936346196,
					-28.744206997358447
				],
				[
					-252.88451456578287,
					-28.744206997358447
				],
				[
					-254.176399336774,
					-28.421257981113285
				],
				[
					-255.46828410776516,
					-28.421257981113285
				],
				[
					-256.437190293841,
					-28.421257981113285
				],
				[
					-257.7290454961617,
					-28.098279396197995
				],
				[
					-259.3439088520681,
					-27.775300811282705
				],
				[
					-259.9898364532287,
					-27.775300811282705
				],
				[
					-260.95874263930455,
					-27.775300811282705
				],
				[
					-261.6046702404649,
					-27.452351795037544
				],
				[
					-262.2506274102957,
					-27.452351795037544
				],
				[
					-262.89655501145603,
					-27.129373210122253
				],
				[
					-263.5424826126166,
					-27.129373210122253
				],
				[
					-264.1884397824472,
					-26.80639462520685
				],
				[
					-265.15734596852303,
					-26.80639462520685
				],
				[
					-266.44920117084393,
					-26.80639462520685
				],
				[
					-267.7410859418351,
					-26.80639462520685
				],
				[
					-268.70999212791094,
					-26.4834456089618
				],
				[
					-270.32482591514713,
					-26.160467024046397
				],
				[
					-271.293732101223,
					-25.837488439131107
				],
				[
					-272.2626382872986,
					-25.837488439131107
				],
				[
					-272.9085954571294,
					-25.837488439131107
				],
				[
					-273.23154447337447,
					-25.837488439131107
				],
				[
					-273.55452305828976,
					-25.837488439131107
				],
				[
					-274.2004506594503,
					-25.514539422885946
				],
				[
					-274.8464078292809,
					-25.191560837970655
				],
				[
					-275.1693568455262,
					-25.191560837970655
				],
				[
					-276.13826303160204,
					-24.86858225305525
				],
				[
					-276.4612416165173,
					-24.86858225305525
				],
				[
					-277.10716921767767,
					-24.86858225305525
				],
				[
					-277.10716921767767,
					-24.86858225305525
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 251,
			"versionNonce": 1587563504,
			"isDeleted": false,
			"id": "u9TDY7U5wrCAqspikRqEj",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3227.998820520387,
			"y": -119.71442668110512,
			"strokeColor": "#846358",
			"backgroundColor": "transparent",
			"width": 134.67795986453552,
			"height": 223.8173289835089,
			"seed": 1980419344,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.32294901624504746,
					0
				],
				[
					0.6459571698308082,
					0
				],
				[
					0.9689061860758557,
					-0.6459571698306945
				],
				[
					1.2918552023209031,
					-1.2918552023209031
				],
				[
					1.937812372151484,
					-1.6148633559064365
				],
				[
					1.937812372151484,
					-1.9378123721515976
				],
				[
					2.2607613883967588,
					-2.583769541982292
				],
				[
					2.9067185582273396,
					-3.2296675744725007
				],
				[
					3.2296675744726144,
					-3.8756247443031953
				],
				[
					3.5526757280579204,
					-4.198573760548243
				],
				[
					3.5526757280579204,
					-4.844530930378937
				],
				[
					3.5526757280579204,
					-5.490488100209632
				],
				[
					4.19857376054847,
					-5.813437116454793
				],
				[
					4.19857376054847,
					-6.459394286285374
				],
				[
					4.521581914133776,
					-7.105292318775696
				],
				[
					4.521581914133776,
					-7.428300472361229
				],
				[
					4.844530930379051,
					-7.751249488606277
				],
				[
					5.167479946624098,
					-8.074198504851438
				],
				[
					5.490488100209632,
					-9.04310469092718
				],
				[
					5.490488100209632,
					-9.366112844512827
				],
				[
					5.813437116454907,
					-10.012010877003036
				],
				[
					6.459394286285487,
					-10.65796804683373
				],
				[
					6.782343302530535,
					-11.303925216664425
				],
				[
					7.105292318775582,
					-11.626874232909472
				],
				[
					7.428300472361343,
					-12.27283140274028
				],
				[
					7.7512494886063905,
					-13.241737588816022
				],
				[
					8.074198504851438,
					-13.564686605061183
				],
				[
					8.397206658437199,
					-14.533592791136925
				],
				[
					9.043104690927294,
					-15.17954996096762
				],
				[
					9.366112844512827,
					-15.502498977212667
				],
				[
					9.689061860757874,
					-16.148456147043476
				],
				[
					9.689061860757874,
					-16.471405163288523
				],
				[
					10.335019030588683,
					-16.79435417953357
				],
				[
					10.335019030588683,
					-17.117362333119218
				],
				[
					10.65796804683373,
					-17.763260365609426
				],
				[
					10.980917063079005,
					-18.08626851919496
				],
				[
					11.303925216664311,
					-18.73216655168528
				],
				[
					11.626874232909586,
					-19.055174705270815
				],
				[
					12.272831402740167,
					-19.701072737761024
				],
				[
					12.918729435230489,
					-20.34702990759172
				],
				[
					12.918729435230489,
					-20.9929870774223
				],
				[
					13.887635621306117,
					-21.63888510991262
				],
				[
					14.210643774891878,
					-22.607791295988477
				],
				[
					14.856541807381973,
					-22.93079944957401
				],
				[
					15.179549960967734,
					-23.57669748206422
				],
				[
					15.825447993457828,
					-24.222654651894914
				],
				[
					16.14845614704359,
					-24.54560366813996
				],
				[
					16.47140516328841,
					-25.191560837970655
				],
				[
					16.794354179533684,
					-25.514509854215817
				],
				[
					17.440311349364265,
					-26.160467024046397
				],
				[
					18.086268519195073,
					-26.48341604029156
				],
				[
					18.732166551685395,
					-27.129373210122253
				],
				[
					19.378123721515976,
					-27.775330379952948
				],
				[
					20.66997892383688,
					-28.421228412443156
				],
				[
					21.315936093667688,
					-29.06718558227385
				],
				[
					21.96189326349827,
					-30.036091768349593
				],
				[
					22.607791295988363,
					-30.6820489381804
				],
				[
					23.899705635649752,
					-31.973904140501304
				],
				[
					24.545603668140075,
					-32.619861310331885
				],
				[
					25.837518007801236,
					-33.58876749640774
				],
				[
					26.16046702404651,
					-34.557673682483596
				],
				[
					27.129373210122367,
					-35.52657986855934
				],
				[
					27.775330379952948,
					-36.17247790104955
				],
				[
					28.421228412443043,
					-37.1413840871254
				],
				[
					28.744236566028803,
					-37.78734125695598
				],
				[
					29.390134598518898,
					-38.43329842678679
				],
				[
					30.036091768349706,
					-39.079196459276886
				],
				[
					30.682048938180515,
					-39.725153629107695
				],
				[
					31.650955124256143,
					-40.371110798938275
				],
				[
					31.97390414050119,
					-41.34001698501413
				],
				[
					32.942810326577046,
					-41.66296600125918
				],
				[
					33.58876749640763,
					-42.631872187335034
				],
				[
					34.55767368248348,
					-43.600778373410776
				],
				[
					35.52657986855934,
					-44.24673554324147
				],
				[
					36.495486054635194,
					-45.215641729317326
				],
				[
					37.46439224071105,
					-46.18454791539307
				],
				[
					38.110290273201144,
					-47.15345410146881
				],
				[
					39.079196459277,
					-47.79935213395913
				],
				[
					39.72515362910758,
					-49.09126647362052
				],
				[
					40.37111079893839,
					-49.73716450611062
				],
				[
					41.34001698501402,
					-51.029078845772005
				],
				[
					41.98591501750434,
					-51.67497687826233
				],
				[
					42.954821203580195,
					-52.64388306433807
				],
				[
					43.600778373411,
					-53.289840234168764
				],
				[
					44.89263357573168,
					-54.25874642024462
				],
				[
					45.53859074556249,
					-55.22765260632036
				],
				[
					47.153454101468924,
					-56.519507808641265
				],
				[
					48.12236028754455,
					-57.48841399471701
				],
				[
					49.09126647362041,
					-58.780328334378396
				],
				[
					50.70607069218636,
					-60.0721835366993
				],
				[
					51.674976878262214,
					-61.041089722775155
				],
				[
					52.64388306433807,
					-62.33294492509606
				],
				[
					53.612789250413925,
					-63.30188067984204
				],
				[
					54.904703590075314,
					-64.59376545083319
				],
				[
					55.87360977615094,
					-65.56267163690893
				],
				[
					56.519507808641265,
					-66.53157782298479
				],
				[
					57.48841399471712,
					-67.82343302530569
				],
				[
					58.45732018079275,
					-68.79233921138155
				],
				[
					59.10327735062356,
					-70.08422398237269
				],
				[
					59.749234520454365,
					-70.08422398237269
				],
				[
					60.39513255294446,
					-71.37610875336384
				],
				[
					61.04108972277504,
					-72.02203635452418
				],
				[
					62.33294492509617,
					-73.31392112551532
				],
				[
					62.655953078681705,
					-73.95984872667589
				],
				[
					63.62485926475733,
					-74.92875491275163
				],
				[
					64.59376545083319,
					-76.22063968374277
				],
				[
					65.56267163690904,
					-76.86656728490323
				],
				[
					66.20856966939914,
					-77.83547347097908
				],
				[
					66.85452683922995,
					-78.48140107213942
				],
				[
					67.50048400906076,
					-79.77328584313057
				],
				[
					68.14638204155085,
					-80.74219202920642
				],
				[
					69.43829638121224,
					-82.03407680019757
				],
				[
					70.08419441370256,
					-82.35702581644261
				],
				[
					70.73015158353314,
					-83.64891058743376
				],
				[
					72.02200678585405,
					-84.61781677350962
				],
				[
					72.66796395568485,
					-85.90970154450076
				],
				[
					73.95981915800553,
					-87.20155674682167
				],
				[
					74.60577632783634,
					-88.17046293289741
				],
				[
					75.57468251391197,
					-89.46234770388855
				],
				[
					76.54358869998782,
					-90.108275305049
				],
				[
					77.51249488606368,
					-91.72313866095544
				],
				[
					78.80435008838458,
					-92.6920448470313
				],
				[
					79.45030725821539,
					-93.9839000493522
				],
				[
					80.41921344429124,
					-95.59876340525864
				],
				[
					81.71106864661192,
					-96.2446910064192
				],
				[
					82.03407680019768,
					-97.53657577741035
				],
				[
					83.00298298627354,
					-98.50548196348609
				],
				[
					83.97188917234917,
					-99.47438814956183
				],
				[
					84.9407953584248,
					-101.08922193679814
				],
				[
					85.90970154450065,
					-102.38110670778917
				],
				[
					86.55559957699097,
					-103.35001289386503
				],
				[
					87.52450576306683,
					-104.96484668110122
				],
				[
					88.81642010272822,
					-105.93375286717708
				],
				[
					89.46231813521831,
					-107.22563763816822
				],
				[
					90.7542324748797,
					-108.51749284048913
				],
				[
					91.40013050737002,
					-109.48639902656498
				],
				[
					92.69204484703118,
					-110.77828379755613
				],
				[
					93.66095103310704,
					-112.07016856854727
				],
				[
					94.30684906559736,
					-112.71609616970761
				],
				[
					95.27575525167299,
					-114.33092995694392
				],
				[
					96.24466143774885,
					-115.94579331285047
				],
				[
					96.89061860757965,
					-116.91469949892621
				],
				[
					97.2135676238247,
					-118.20655470124711
				],
				[
					98.18247380990056,
					-118.85251187107781
				],
				[
					98.82843097973114,
					-120.14436707339871
				],
				[
					99.47438814956195,
					-121.43625184438986
				],
				[
					100.44329433563757,
					-122.40515803046571
				],
				[
					101.0891923681279,
					-123.69704280145675
				],
				[
					102.05809855420375,
					-125.31187658869305
				],
				[
					102.70405572403456,
					-126.2807827747688
				],
				[
					103.67296191011019,
					-127.57266754575994
				],
				[
					104.64186809618604,
					-129.18750133299625
				],
				[
					104.96481711243109,
					-130.4793861039874
				],
				[
					105.93372329850695,
					-131.7712413063083
				],
				[
					106.57968046833753,
					-133.06312607729944
				],
				[
					107.22563763816811,
					-134.67795986453564
				],
				[
					107.54858665441338,
					-135.6468660506115
				],
				[
					108.19454382424396,
					-136.93875082160264
				],
				[
					108.19454382424396,
					-138.55358460883883
				],
				[
					108.84044185673429,
					-139.5224907949147
				],
				[
					109.4863990265651,
					-140.81437556590583
				],
				[
					109.80934804281014,
					-141.78328175198158
				],
				[
					110.45530521264072,
					-143.39811553921788
				],
				[
					110.77825422888577,
					-144.36702172529363
				],
				[
					111.74716041496163,
					-146.30483409744522
				],
				[
					112.07016856854739,
					-147.59671886843637
				],
				[
					112.39311758479221,
					-148.88860363942752
				],
				[
					113.03907475462302,
					-150.5034374266637
				],
				[
					114.00798094069887,
					-151.47234361273956
				],
				[
					114.33092995694392,
					-153.08717739997576
				],
				[
					114.9768871267745,
					-154.3790621709669
				],
				[
					115.29983614301977,
					-155.9938959582031
				],
				[
					115.94579331285036,
					-157.28578072919424
				],
				[
					115.94579331285036,
					-158.2546869152701
				],
				[
					116.59169134534068,
					-159.8695207025063
				],
				[
					116.91469949892621,
					-161.16140547349744
				],
				[
					117.5605975314163,
					-162.45329024448858
				],
				[
					117.88360568500207,
					-163.7451454468095
				],
				[
					117.88360568500207,
					-164.71405163288534
				],
				[
					118.52950371749216,
					-166.0059364038765
				],
				[
					119.17546088732297,
					-166.97484258995223
				],
				[
					119.49840990356802,
					-168.26672736094338
				],
				[
					119.82141805715378,
					-169.55858256326428
				],
				[
					120.1443670733986,
					-170.52748874934002
				],
				[
					120.7903242432294,
					-171.49639493541588
				],
				[
					121.11327325947445,
					-172.78827970640702
				],
				[
					121.75923042930526,
					-174.08016447739817
				],
				[
					122.08217944555031,
					-175.37201967971907
				],
				[
					122.08217944555031,
					-176.66390445071022
				],
				[
					122.72813661538089,
					-177.63281063678608
				],
				[
					123.05108563162617,
					-178.92469540777722
				],
				[
					123.37403464787121,
					-180.21655061009812
				],
				[
					123.69704280145675,
					-181.18545679617387
				],
				[
					124.01999181770202,
					-182.1543629822496
				],
				[
					124.01999181770202,
					-183.12326916832546
				],
				[
					124.6659489875326,
					-184.09217535440132
				],
				[
					124.6659489875326,
					-185.06108154047706
				],
				[
					124.98889800377788,
					-185.70703871030776
				],
				[
					125.3118470200227,
					-186.99889391262866
				],
				[
					125.63485517360846,
					-187.64485108245924
				],
				[
					125.9578041898535,
					-188.6137572685351
				],
				[
					126.28075320609855,
					-189.905612470856
				],
				[
					126.60376135968431,
					-190.87451865693185
				],
				[
					127.24965939217441,
					-192.166403427923
				],
				[
					127.24965939217441,
					-193.13530961399874
				],
				[
					127.89561656200499,
					-194.4271943849899
				],
				[
					128.21856557825026,
					-195.7190495873108
				],
				[
					128.86452274808084,
					-196.68795577338653
				],
				[
					129.18747176432612,
					-198.30281912929308
				],
				[
					129.18747176432612,
					-199.27172531536883
				],
				[
					129.8334289341567,
					-200.24063150144468
				],
				[
					130.15637795040197,
					-201.53248670376558
				],
				[
					130.47938610398728,
					-202.17844387359628
				],
				[
					130.80233512023256,
					-203.47029907591718
				],
				[
					131.1252841364776,
					-204.43920526199292
				],
				[
					131.1252841364776,
					-205.40811144806878
				],
				[
					131.44829229006314,
					-206.37701763414464
				],
				[
					131.44829229006314,
					-207.34592382022038
				],
				[
					131.7712413063084,
					-207.66890240513567
				],
				[
					132.09419032255323,
					-209.28373619237198
				],
				[
					132.417198476139,
					-209.60671477728727
				],
				[
					132.74014749238404,
					-210.57562096336312
				],
				[
					133.0630965086291,
					-211.54452714943886
				],
				[
					133.0630965086291,
					-212.83641192043
				],
				[
					133.0630965086291,
					-213.80531810650575
				],
				[
					133.38610466221485,
					-214.45124570766632
				],
				[
					133.7090536784599,
					-215.42015189374206
				],
				[
					134.03200269470494,
					-216.0660794949025
				],
				[
					134.03200269470494,
					-217.03498568097837
				],
				[
					134.3550108482907,
					-217.35796426589366
				],
				[
					134.3550108482907,
					-218.0038918670541
				],
				[
					134.67795986453552,
					-218.3268704519695
				],
				[
					134.67795986453552,
					-218.97279805312985
				],
				[
					134.67795986453552,
					-219.29577663804525
				],
				[
					134.67795986453552,
					-219.61875522296066
				],
				[
					134.67795986453552,
					-219.9417042392057
				],
				[
					134.67795986453552,
					-220.264682824121
				],
				[
					134.67795986453552,
					-220.5876614090364
				],
				[
					134.67795986453552,
					-220.91061042528156
				],
				[
					134.67795986453552,
					-221.23358901019685
				],
				[
					134.67795986453552,
					-222.2024951962727
				],
				[
					134.67795986453552,
					-222.84842279743305
				],
				[
					134.67795986453552,
					-223.17140138234845
				],
				[
					134.67795986453552,
					-223.49437996726385
				],
				[
					134.67795986453552,
					-223.8173289835089
				],
				[
					134.67795986453552,
					-223.8173289835089
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 157,
			"versionNonce": 244403696,
			"isDeleted": false,
			"id": "mFPV_m02k5IAfc_C1cfFw",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3225.565427843905,
			"y": -598.6455585676096,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 53.984528837544076,
			"height": 110.30350075359888,
			"seed": 323922704,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.2917903571565148,
					0.8754245031403229
				],
				[
					1.167214860296781,
					1.7508490062806459
				],
				[
					1.7508490062807596,
					2.918077224495164
				],
				[
					2.3344831522647382,
					3.5016980125612918
				],
				[
					2.9180638665775405,
					4.66892623077581
				],
				[
					3.501698012561519,
					5.544350733916133
				],
				[
					3.7934883697178066,
					6.419775237056456
				],
				[
					4.377122515701785,
					7.295199740196779
				],
				[
					4.668912872858073,
					8.754245031403286
				],
				[
					5.252547018842051,
					9.62966953454361
				],
				[
					5.544337375998339,
					10.79689775275807
				],
				[
					6.127971521982317,
					11.964139328890383
				],
				[
					6.7116056679665235,
					12.839563832030763
				],
				[
					7.295186382279098,
					14.006792050245224
				],
				[
					7.58703017110679,
					14.882216553385547
				],
				[
					8.462454674247056,
					16.049444771600065
				],
				[
					9.04603538855963,
					17.508490062806516
				],
				[
					10.213303680527588,
					18.967535354013023
				],
				[
					11.088728183668081,
					20.42656728730168
				],
				[
					11.964152686808347,
					21.593808863433992
				],
				[
					12.547733401120922,
					22.76103708164851
				],
				[
					13.131367547105128,
					23.92826529986297
				],
				[
					13.715001693089107,
					24.511886087929156
				],
				[
					14.006792050245394,
					25.679114306143617
				],
				[
					14.298582407401682,
					26.262735094209802
				],
				[
					14.590426196229373,
					27.138159597350125
				],
				[
					15.174006910541948,
					27.72178038541631
				],
				[
					15.46585069936964,
					28.305387815564586
				],
				[
					15.757641056525927,
					29.180812318704966
				],
				[
					16.341275202509905,
					29.764433106771094
				],
				[
					16.924855916822708,
					30.931661324985612
				],
				[
					17.508490062806686,
					31.51528211305174
				],
				[
					18.96754871193093,
					32.97432740425825
				],
				[
					19.842973215071197,
					34.14155562247271
				],
				[
					21.010188075367978,
					35.30878384068723
				],
				[
					21.885612578508244,
					36.76782913189368
				],
				[
					22.469246724492223,
					37.935057350108195
				],
				[
					22.76103708164851,
					38.81048185324852
				],
				[
					23.636461584788776,
					39.97772342938083
				],
				[
					23.92825194194529,
					40.85314793252115
				],
				[
					24.51188608792927,
					41.72857243566148
				],
				[
					24.803676445085557,
					42.6039969388018
				],
				[
					25.387310591069536,
					43.77122515701632
				],
				[
					25.679100948225823,
					44.93845337523078
				],
				[
					26.554525451366317,
					45.81387787837116
				],
				[
					27.138159597350295,
					46.981119454503414
				],
				[
					28.01358410049056,
					48.44015138779207
				],
				[
					29.180798960787115,
					49.60739296392444
				],
				[
					30.05622346392761,
					50.77462118213896
				],
				[
					31.223491755895566,
					52.23366647334541
				],
				[
					31.80707247020814,
					53.692698406634065
				],
				[
					32.68249697334841,
					54.85993998276638
				],
				[
					33.266131119332385,
					56.318971916055034
				],
				[
					33.5579214764889,
					57.19439641919536
				],
				[
					34.14155562247288,
					58.36163799532767
				],
				[
					34.433345979629166,
					59.23706249846805
				],
				[
					34.72518976845686,
					60.40429071668245
				],
				[
					35.016980125613145,
					61.27971521982283
				],
				[
					35.30877048276943,
					62.15513972296321
				],
				[
					35.600614271597124,
					63.03056422610348
				],
				[
					36.47603877473739,
					63.905988729243745
				],
				[
					36.767829131893905,
					65.36503402045025
				],
				[
					37.64325363503417,
					66.24045852359063
				],
				[
					38.22688778101815,
					67.40768674180515
				],
				[
					38.51867813817444,
					68.28311124494542
				],
				[
					39.39410264131493,
					69.1585357480858
				],
				[
					39.97773678729891,
					70.3257639663002
				],
				[
					40.26952714445497,
					71.20118846944058
				],
				[
					40.85316129043895,
					72.07661297258096
				],
				[
					41.43674200475175,
					72.95203747572123
				],
				[
					41.72858579357944,
					74.1192790518536
				],
				[
					42.02037615073573,
					74.70288648200187
				],
				[
					42.312166507892016,
					75.28650727006811
				],
				[
					42.312166507892016,
					75.87012805813424
				],
				[
					42.895800653875995,
					76.45373548828252
				],
				[
					43.47943479985997,
					77.62097706441489
				],
				[
					43.77122515701649,
					78.49640156755515
				],
				[
					44.35485930300047,
					79.66362978576967
				],
				[
					44.93844001731304,
					80.83085800398419
				],
				[
					45.52207416329702,
					81.99809958011645
				],
				[
					46.105708309281,
					82.87352408325683
				],
				[
					46.689289023593574,
					84.04075230147134
				],
				[
					46.98113281242149,
					84.62437308953747
				],
				[
					47.27292316957755,
					85.49979759267785
				],
				[
					47.56471352673407,
					86.08340502282613
				],
				[
					48.148347672718046,
					86.37522209581812
				],
				[
					48.148347672718046,
					87.25064659895838
				],
				[
					48.148347672718046,
					87.83425402910677
				],
				[
					48.44013802987433,
					88.12607110209876
				],
				[
					48.44013802987433,
					88.70967853224715
				],
				[
					48.44013802987433,
					89.29329932031328
				],
				[
					48.731981818702025,
					89.87692010837941
				],
				[
					49.02377217585831,
					91.04414832659393
				],
				[
					49.60740632184252,
					91.9195728297343
				],
				[
					49.89919667899858,
					92.50319361780043
				],
				[
					50.19098703615509,
					93.08680104794871
				],
				[
					50.48283082498256,
					93.3786181209407
				],
				[
					50.77462118213907,
					93.96222555108909
				],
				[
					50.77462118213907,
					94.25404262408108
				],
				[
					50.77462118213907,
					94.54584633915522
				],
				[
					50.77462118213907,
					94.83765005422936
				],
				[
					51.06641153929536,
					94.83765005422936
				],
				[
					51.06641153929536,
					95.12946712722135
				],
				[
					51.06641153929536,
					95.71307455736974
				],
				[
					51.06641153929536,
					96.00489163036173
				],
				[
					51.35825532812305,
					96.58849906051
				],
				[
					51.35825532812305,
					96.88031613350199
				],
				[
					51.65004568527934,
					97.75574063664237
				],
				[
					51.941836042435625,
					98.04754435171651
				],
				[
					52.233679831263316,
					98.63116513978275
				],
				[
					52.233679831263316,
					99.21477256993103
				],
				[
					52.525470188419604,
					99.50658964292302
				],
				[
					52.81726054557612,
					99.50658964292302
				],
				[
					52.81726054557612,
					99.79839335799716
				],
				[
					52.81726054557612,
					100.38201414606328
				],
				[
					52.81726054557612,
					100.67381786113754
				],
				[
					52.81726054557612,
					101.25743864920366
				],
				[
					52.81726054557612,
					101.54925572219565
				],
				[
					52.81726054557612,
					102.13286315234404
				],
				[
					53.10910433440358,
					103.00828765548431
				],
				[
					53.4008946915601,
					103.3001047284763
				],
				[
					53.69268504871616,
					103.59189508563259
				],
				[
					53.69268504871616,
					103.88371215862458
				],
				[
					53.69268504871616,
					104.17552923161657
				],
				[
					53.984528837544076,
					104.46731958877297
				],
				[
					53.984528837544076,
					104.75913666176496
				],
				[
					53.984528837544076,
					105.05095373475694
				],
				[
					53.69268504871616,
					105.63456116490534
				],
				[
					53.69268504871616,
					105.92637823789732
				],
				[
					53.69268504871616,
					106.21816859505361
				],
				[
					53.4008946915601,
					106.5099856680456
				],
				[
					53.10910433440358,
					106.5099856680456
				],
				[
					53.10910433440358,
					106.80180274103759
				],
				[
					52.81726054557612,
					106.80180274103759
				],
				[
					52.525470188419604,
					107.09359309819388
				],
				[
					52.525470188419604,
					107.38541017118598
				],
				[
					52.233679831263316,
					107.67722724417797
				],
				[
					51.941836042435625,
					107.96901760133426
				],
				[
					51.65004568527934,
					108.26083467432625
				],
				[
					51.35825532812305,
					108.26083467432625
				],
				[
					51.06641153929536,
					108.55265174731824
				],
				[
					50.77462118213907,
					108.84444210447464
				],
				[
					50.48283082498256,
					108.84444210447464
				],
				[
					50.48283082498256,
					109.13625917746663
				],
				[
					50.48283082498256,
					109.42807625045862
				],
				[
					50.19098703615509,
					109.7198666076149
				],
				[
					49.89919667899858,
					110.0116836806069
				],
				[
					49.60740632184252,
					110.0116836806069
				],
				[
					49.3155625330146,
					110.30350075359888
				],
				[
					49.02377217585831,
					110.30350075359888
				],
				[
					48.731981818702025,
					110.30350075359888
				],
				[
					48.731981818702025,
					110.30350075359888
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "line",
			"version": 132,
			"versionNonce": 1561464816,
			"isDeleted": false,
			"id": "PK87LgABOpuiShRP8U3p2",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3441.503436330738,
			"y": -196.53392126904384,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 74.99466348124042,
			"height": 148.23855810370708,
			"seed": 1483131152,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-74.99466348124042,
					-148.23855810370708
				]
			]
		},
		{
			"type": "freedraw",
			"version": 116,
			"versionNonce": 1646957040,
			"isDeleted": false,
			"id": "SzSuEr6Z6JeecjzDN1cEI",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3439.1690066101446,
			"y": -195.07488933575507,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 69.74216989406978,
			"height": 146.19589202443444,
			"seed": 1087055632,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					-0.2917903571564011
				],
				[
					0,
					-0.8754245031403798
				],
				[
					0,
					-1.4590319332887702
				],
				[
					0,
					-2.042639363437047
				],
				[
					-0.5836341459839787,
					-2.918063866577313
				],
				[
					-0.5836341459839787,
					-3.793488369717693
				],
				[
					-1.4590586491242448,
					-5.252547018842051
				],
				[
					-2.0426927951082234,
					-6.419761879138605
				],
				[
					-2.3344831522647382,
					-7.587003455271088
				],
				[
					-3.2099076554050043,
					-8.754245031403343
				],
				[
					-4.08533215854527,
					-10.505094037683989
				],
				[
					-4.377122515701785,
					-11.380518540824369
				],
				[
					-5.252547018841824,
					-13.131367547104901
				],
				[
					-5.836181164825803,
					-14.298582407401682
				],
				[
					-6.419815310809781,
					-15.757641056525927
				],
				[
					-7.295239813950275,
					-17.508490062806572
				],
				[
					-7.587030171106562,
					-18.96752199609523
				],
				[
					-8.462454674246828,
					-20.426553929383886
				],
				[
					-9.337879177387322,
					-22.17740293566453
				],
				[
					-9.9215133233713,
					-23.92825194194529
				],
				[
					-10.796937826511567,
					-25.679100948225823
				],
				[
					-11.380518540824369,
					-27.721767027498572
				],
				[
					-12.255943043964407,
					-29.764433106771094
				],
				[
					-13.131367547104901,
					-31.223465040059864
				],
				[
					-14.006792050245167,
					-32.68249697334841
				],
				[
					-14.882216553385433,
					-34.433345979629166
				],
				[
					-15.757641056525927,
					-36.1841949859097
				],
				[
					-16.341275202509905,
					-37.64325363503417
				],
				[
					-17.50849006280646,
					-39.10228556832271
				],
				[
					-18.383914565946952,
					-40.561317501611484
				],
				[
					-18.96754871193093,
					-42.312166507892016
				],
				[
					-19.842973215071197,
					-44.063015514172776
				],
				[
					-20.134763572227484,
					-45.52207416329702
				],
				[
					-21.010188075367978,
					-46.397498666437286
				],
				[
					-21.593822221351957,
					-47.85653059972606
				],
				[
					-22.469246724491995,
					-49.60737960600659
				],
				[
					-23.34467122763249,
					-50.77462118213896
				],
				[
					-23.928305373616467,
					-52.233653115427614
				],
				[
					-24.803729876756734,
					-53.69268504871627
				],
				[
					-25.679154379897,
					-55.44353405499692
				],
				[
					-26.84636924019378,
					-56.610775631129286
				],
				[
					-27.43000338617776,
					-58.06980756441794
				],
				[
					-28.305427889318025,
					-59.52886621354219
				],
				[
					-28.8890086036306,
					-60.69608107383897
				],
				[
					-29.764433106771094,
					-62.15513972296321
				],
				[
					-30.348067252755072,
					-63.32235458325988
				],
				[
					-30.63985760991136,
					-64.48959615939225
				],
				[
					-31.515282113051626,
					-65.6568377355245
				],
				[
					-32.39070661619212,
					-67.11586966881316
				],
				[
					-32.9743407621761,
					-67.99129417195354
				],
				[
					-33.55797490816008,
					-69.45032610524208
				],
				[
					-34.14155562247265,
					-70.32575060838246
				],
				[
					-34.72518976845663,
					-71.20117511152284
				],
				[
					-35.600614271597124,
					-72.95202411780349
				],
				[
					-36.1842484175811,
					-74.11926569393586
				],
				[
					-37.05967292072137,
					-74.99469019707612
				],
				[
					-37.64325363503417,
					-76.74553920335677
				],
				[
					-38.51867813817421,
					-77.62096370649715
				],
				[
					-39.3941026413147,
					-79.0799956397857
				],
				[
					-39.97773678729868,
					-80.24723721591806
				],
				[
					-40.85316129043895,
					-81.70626914920672
				],
				[
					-41.436795436422926,
					-82.87351072533897
				],
				[
					-42.02037615073573,
					-83.74893522847935
				],
				[
					-42.60401029671971,
					-85.20796716176801
				],
				[
					-43.187644442703686,
					-86.08339166490828
				],
				[
					-44.06306894584395,
					-87.25063324104076
				],
				[
					-44.35485930300024,
					-88.7096651743293
				],
				[
					-45.23028380614073,
					-90.16872382345366
				],
				[
					-46.10570830928077,
					-91.33593868375033
				],
				[
					-46.68934245526498,
					-92.79499733287457
				],
				[
					-47.564766958405244,
					-94.25402926616334
				],
				[
					-48.44019146154574,
					-95.71306119945189
				],
				[
					-49.315615964685776,
					-97.17211984857624
				],
				[
					-50.19104046782627,
					-98.92296885485689
				],
				[
					-50.774621182138844,
					-100.38200078814555
				],
				[
					-51.9418894741068,
					-102.13284979442619
				],
				[
					-52.525470188419376,
					-103.59188172771485
				],
				[
					-53.40089469155987,
					-105.05094037683921
				],
				[
					-53.98452883754385,
					-106.50997231012786
				],
				[
					-54.56816298352783,
					-108.26082131640851
				],
				[
					-55.44358748666832,
					-109.42806289254077
				],
				[
					-56.027168200980896,
					-110.88709482582954
				],
				[
					-56.31901198980836,
					-112.34612675911808
				],
				[
					-57.19443649294885,
					-113.80518540824244
				],
				[
					-58.06986099608912,
					-115.84782477167937
				],
				[
					-58.06986099608912,
					-117.30688342080373
				],
				[
					-58.945285499229385,
					-119.34952278424066
				],
				[
					-59.82071000236988,
					-121.10037179052142
				],
				[
					-60.696134505510145,
					-123.14303786979406
				],
				[
					-61.57155900865041,
					-124.8938868760747
				],
				[
					-62.155139722962986,
					-126.64473588235535
				],
				[
					-63.32240801493117,
					-128.68740196162798
				],
				[
					-63.905988729243745,
					-130.43825096790863
				],
				[
					-64.78141323238401,
					-131.8972829011973
				],
				[
					-65.6568377355245,
					-133.35631483448594
				],
				[
					-65.6568377355245,
					-134.5235564106183
				],
				[
					-66.24047188150848,
					-135.69079798675057
				],
				[
					-66.53226223866477,
					-136.56622248989095
				],
				[
					-66.82410602749246,
					-137.73343735018761
				],
				[
					-67.11589638464875,
					-138.60886185332788
				],
				[
					-67.40768674180504,
					-139.77610342946025
				],
				[
					-67.40768674180504,
					-140.35971085960864
				],
				[
					-67.69953053063273,
					-141.81876950873288
				],
				[
					-67.99132088778902,
					-142.40237693888116
				],
				[
					-68.574955033773,
					-143.27780144202154
				],
				[
					-68.86674539092951,
					-144.15322594516192
				],
				[
					-69.15853574808557,
					-145.0286504483022
				],
				[
					-69.45037953691349,
					-145.61225787845046
				],
				[
					-69.74216989406978,
					-145.90407495144245
				],
				[
					-69.74216989406978,
					-146.19589202443444
				],
				[
					-69.74216989406978,
					-146.19589202443444
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 384,
			"versionNonce": 1961022448,
			"isDeleted": false,
			"id": "FSh6yVgsvquZoR9oU0mjk",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3360.9643820418282,
			"y": -347.10693580917984,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 219.73155028822157,
			"height": 231.69567625919433,
			"seed": 418628880,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.29181707299198933
				],
				[
					0,
					0.8754245031402661
				],
				[
					0.29184378882746387,
					2.042666079272635
				],
				[
					0.5836341459839787,
					3.2098809395693024
				],
				[
					1.1672682919679573,
					4.668939588693547
				],
				[
					1.4590586491242448,
					5.836154448990328
				],
				[
					1.4590586491242448,
					7.0033960251225835
				],
				[
					1.4590586491242448,
					8.170637601254839
				],
				[
					1.4590586491242448,
					8.75424503140323
				],
				[
					1.4590586491242448,
					9.921486607535599
				],
				[
					1.4590586491242448,
					10.213276964691886
				],
				[
					1.1672682919679573,
					11.088701467832152
				],
				[
					0.8754245031402661,
					11.964125970972532
				],
				[
					0.5836341459839787,
					12.839550474112912
				],
				[
					0.29184378882746387,
					13.714974977253178
				],
				[
					0.29184378882746387,
					14.298609123237156
				],
				[
					0,
					15.174033626377536
				],
				[
					-0.2917903571565148,
					16.049458129517916
				],
				[
					-0.5835807143125749,
					17.50849006280646
				],
				[
					-0.8754245031404935,
					18.675731638938828
				],
				[
					-1.1672148602965535,
					20.134763572227484
				],
				[
					-1.1672148602965535,
					21.30200514835974
				],
				[
					-1.4590052174530683,
					22.46922000865652
				],
				[
					-2.042639363437047,
					23.928278657780766
				],
				[
					-2.3344297205933344,
					25.095493518077433
				],
				[
					-2.6262735094210257,
					26.262735094209802
				],
				[
					-3.2098542237336005,
					27.429976670342057
				],
				[
					-3.793488369717579,
					28.597191530638725
				],
				[
					-4.377122515701558,
					29.764433106771094
				],
				[
					-4.668912872858073,
					30.63985760991136
				],
				[
					-5.252547018842051,
					32.098889543200016
				],
				[
					-5.836127733154626,
					32.974314046340396
				],
				[
					-6.127971521982317,
					34.14155562247265
				],
				[
					-6.419761879138605,
					35.30879719860502
				],
				[
					-7.295186382279098,
					36.76782913189368
				],
				[
					-7.878820528263077,
					37.93507070802593
				],
				[
					-8.170610885419364,
					39.68591971430669
				],
				[
					-8.754245031403343,
					40.853134574603246
				],
				[
					-9.337825745716145,
					41.728559077743625
				],
				[
					-9.62966953454361,
					42.603983580884005
				],
				[
					-10.213250248856184,
					43.77122515701626
				],
				[
					-10.796884394840163,
					44.64664966015653
				],
				[
					-11.088674751996678,
					45.813891236288896
				],
				[
					-11.672308897980656,
					46.397498666437286
				],
				[
					-11.964099255136944,
					47.56474024256954
				],
				[
					-12.547733401120922,
					48.14834767271782
				],
				[
					-12.83952375827721,
					49.3155892488503
				],
				[
					-13.131367547104901,
					49.89919667899858
				],
				[
					-13.714948261417703,
					51.066438255130834
				],
				[
					-14.298582407401682,
					51.94186275827121
				],
				[
					-14.59037276455797,
					52.525470188419604
				],
				[
					-14.88221655338566,
					53.40089469155987
				],
				[
					-15.174006910541948,
					54.568136267692125
				],
				[
					-15.465797267698235,
					55.151743697840516
				],
				[
					-15.757641056525927,
					56.318985273972885
				],
				[
					-16.34122177083873,
					57.48620013426944
				],
				[
					-16.633065559666193,
					58.36162463740982
				],
				[
					-16.924855916822708,
					59.2370491405502
				],
				[
					-17.508490062806686,
					60.69610778967444
				],
				[
					-18.383914565946952,
					61.57153229281471
				],
				[
					-18.67570492310324,
					62.73874715311149
				],
				[
					-19.25933906908722,
					64.19780580223573
				],
				[
					-20.134763572227712,
					65.6568377355245
				],
				[
					-20.426553929383772,
					66.82407931165676
				],
				[
					-21.301978432524265,
					68.28311124494542
				],
				[
					-21.885612578508244,
					69.45035282107779
				],
				[
					-22.17740293566453,
					70.32577732421805
				],
				[
					-22.76103708164851,
					71.78480925750671
				],
				[
					-23.344617795961312,
					72.95205083363908
				],
				[
					-23.636461584788776,
					73.82747533677934
				],
				[
					-24.22004229910135,
					75.286507270068
				],
				[
					-24.51188608792927,
					76.16193177320838
				],
				[
					-25.387310591069536,
					77.32917334934064
				],
				[
					-25.679100948225823,
					78.4963882096373
				],
				[
					-26.262735094209802,
					79.66362978576967
				],
				[
					-27.138159597350295,
					81.12266171905821
				],
				[
					-27.72174031166287,
					82.2899032951907
				],
				[
					-28.597164814803136,
					83.74893522847924
				],
				[
					-29.180798960787115,
					85.49978423476
				],
				[
					-30.05622346392738,
					86.95884288388424
				],
				[
					-30.63985760991136,
					88.12605774418091
				],
				[
					-31.223438324224162,
					89.58511639330527
				],
				[
					-31.515282113051853,
					91.3359653995858
				],
				[
					-32.09886282736443,
					92.79499733287457
				],
				[
					-32.39070661619212,
					94.5458463391551
				],
				[
					-32.68249697334841,
					96.00487827244388
				],
				[
					-33.266131119332385,
					97.46393692156812
				],
				[
					-34.14155562247288,
					98.92296885485689
				],
				[
					-34.43334597962894,
					100.38200078814543
				],
				[
					-35.016980125613145,
					101.84105943726979
				],
				[
					-35.89240462875341,
					103.30009137055845
				],
				[
					-36.1841949859097,
					104.4673329466907
				],
				[
					-37.059619489049965,
					105.92636487997947
				],
				[
					-37.64325363503394,
					107.67721388626
				],
				[
					-38.51867813817444,
					108.55263838940039
				],
				[
					-39.3941026413147,
					110.01167032268904
				],
				[
					-39.977683355627505,
					111.76251932896969
				],
				[
					-41.14495164759546,
					113.22157797809405
				],
				[
					-41.72853236190804,
					114.6806099113827
				],
				[
					-43.18759101103251,
					116.43145891766335
				],
				[
					-43.77122515701649,
					118.182307923944
				],
				[
					-44.64664966015653,
					119.93315693022464
				],
				[
					-45.81386452045331,
					121.68400593650529
				],
				[
					-46.689289023593574,
					123.43485494278593
				],
				[
					-47.56471352673407,
					124.89388687607459
				],
				[
					-48.44013802987433,
					126.64473588235523
				],
				[
					-49.3155625330146,
					128.10379453147948
				],
				[
					-50.19098703615509,
					128.97921903461997
				],
				[
					-50.77462118213907,
					130.7300680409005
				],
				[
					-52.23362639959191,
					132.48091704718126
				],
				[
					-53.10905090273218,
					134.2317660534618
				],
				[
					-54.276319194700136,
					135.39898091375858
				],
				[
					-55.15174369784063,
					136.85803956288282
				],
				[
					-56.6107489152937,
					138.60888856916347
				],
				[
					-57.778017207261655,
					140.6515279326004
				],
				[
					-58.94523206755821,
					142.11058658172476
				],
				[
					-59.8206565706987,
					144.1532259451617
				],
				[
					-60.987871430995256,
					145.32046752129406
				],
				[
					-62.15513972296321,
					147.0713165275747
				],
				[
					-63.32235458325977,
					148.53034846086337
				],
				[
					-64.19777908640026,
					149.69759003699573
				],
				[
					-65.36499394669681,
					151.1566219702844
				],
				[
					-66.2404184498373,
					152.32386354641676
				],
				[
					-67.69947709896132,
					153.49110512254902
				],
				[
					-68.28311124494553,
					154.36652962568928
				],
				[
					-69.1585357480858,
					155.24195412882966
				],
				[
					-70.03396025122629,
					156.11737863197004
				],
				[
					-70.90938475436633,
					156.9928031351103
				],
				[
					-72.07659961466311,
					157.86822763825057
				],
				[
					-72.95202411780338,
					158.74365214139095
				],
				[
					-73.82744862094387,
					159.61907664453133
				],
				[
					-74.99466348124042,
					160.4945011476716
				],
				[
					-76.16193177320838,
					161.66171600796827
				],
				[
					-77.03735627634887,
					162.82895758410064
				],
				[
					-78.20457113664543,
					163.7044088030766
				],
				[
					-79.37178599694198,
					164.87162366337327
				],
				[
					-81.12263500322274,
					166.33068231249763
				],
				[
					-82.58169365234698,
					167.78968752995058
				],
				[
					-84.04075230147146,
					169.24874617907494
				],
				[
					-85.4997575189243,
					170.4159610393715
				],
				[
					-87.25060652520506,
					172.16681004565226
				],
				[
					-88.7096651743293,
					173.3340783376202
				],
				[
					-90.16872382345355,
					174.50129319791677
				],
				[
					-91.33593868375033,
					175.66850805821355
				],
				[
					-92.79499733287457,
					177.1275667073378
				],
				[
					-93.67042183601507,
					178.00299121047806
				],
				[
					-95.12942705346791,
					179.75384021675882
				],
				[
					-96.29669534543586,
					180.62926471989908
				],
				[
					-97.46391020573265,
					181.50468922303946
				],
				[
					-98.6311250660292,
					182.96374787216382
				],
				[
					-100.09018371515367,
					184.13096273246038
				],
				[
					-101.8410327214342,
					185.59002138158473
				],
				[
					-103.59188172771474,
					187.0490265990377
				],
				[
					-105.3427307339955,
					188.79987560531845
				],
				[
					-107.09357974027625,
					190.2589342544427
				],
				[
					-108.84442874655679,
					191.71799290356705
				],
				[
					-112.05433640196179,
					193.76063226700398
				],
				[
					-114.09697576539884,
					195.51148127328474
				],
				[
					-116.43145891766335,
					197.55412063672156
				],
				[
					-118.4740982811004,
					199.30496964300232
				],
				[
					-120.22494728738093,
					200.47223793497028
				],
				[
					-121.97579629366169,
					201.93124315242335
				],
				[
					-123.43485494278593,
					203.3903018015476
				],
				[
					-124.893860160239,
					204.55751666184426
				],
				[
					-126.35291880936325,
					205.72478495381222
				],
				[
					-127.22834331250351,
					206.6002094569526
				],
				[
					-128.3955581728003,
					207.47563396009286
				],
				[
					-129.27098267594056,
					208.35105846323324
				],
				[
					-130.14640717908105,
					208.93463917754593
				],
				[
					-131.02183168222132,
					209.8100636806862
				],
				[
					-131.6054658282053,
					210.68548818382646
				],
				[
					-132.48089033134556,
					211.26912232981044
				],
				[
					-133.06452447732954,
					212.14454683295094
				],
				[
					-133.35631483448606,
					212.72818097893492
				],
				[
					-133.93994898047004,
					213.3117616932475
				],
				[
					-134.5235296947826,
					213.89539583923147
				],
				[
					-134.8153734836103,
					214.47902998521545
				],
				[
					-135.1071638407666,
					215.06261069952814
				],
				[
					-135.39895419792288,
					215.93803520266852
				],
				[
					-135.69079798675057,
					216.2298789914962
				],
				[
					-135.98258834390685,
					216.81345970580878
				],
				[
					-136.56622248989083,
					217.39709385179276
				],
				[
					-136.85801284704712,
					218.27251835493314
				],
				[
					-137.4416469930311,
					219.14794285807352
				],
				[
					-138.3170714961716,
					220.31515771837007
				],
				[
					-138.60886185332788,
					220.89879186435405
				],
				[
					-139.19249599931186,
					222.3578505134784
				],
				[
					-139.77607671362466,
					222.6496408706348
				],
				[
					-139.77607671362466,
					223.52506537377508
				],
				[
					-140.06792050245213,
					223.52506537377508
				],
				[
					-140.06792050245213,
					223.81685573093137
				],
				[
					-140.06792050245213,
					224.10869951975906
				],
				[
					-140.06792050245213,
					224.40048987691534
				],
				[
					-140.06792050245213,
					224.69228023407175
				],
				[
					-140.06792050245213,
					224.98412402289944
				],
				[
					-140.06792050245213,
					225.56770473721213
				],
				[
					-140.06792050245213,
					225.85954852603982
				],
				[
					-140.06792050245213,
					226.4431292403524
				],
				[
					-140.06792050245213,
					227.02676338633637
				],
				[
					-140.06792050245213,
					227.61039753232035
				],
				[
					-140.06792050245213,
					227.90218788947675
				],
				[
					-140.06792050245213,
					228.19397824663304
				],
				[
					-140.06792050245213,
					228.48582203546073
				],
				[
					-140.06792050245213,
					228.77761239261713
				],
				[
					-140.06792050245213,
					229.06940274977342
				],
				[
					-139.77607671362466,
					229.06940274977342
				],
				[
					-139.48428635646815,
					229.06940274977342
				],
				[
					-138.90065221048417,
					229.3612465386011
				],
				[
					-138.60886185332788,
					229.3612465386011
				],
				[
					-138.0252277073439,
					229.6530368957574
				],
				[
					-137.73343735018761,
					229.94482725291368
				],
				[
					-137.14980320420364,
					230.23667104174137
				],
				[
					-136.85801284704712,
					230.52846139889766
				],
				[
					-136.27437870106314,
					230.82025175605395
				],
				[
					-135.98258834390685,
					231.11209554488164
				],
				[
					-135.69079798675057,
					231.11209554488164
				],
				[
					-135.1071638407666,
					231.40388590203804
				],
				[
					-135.1071638407666,
					231.69567625919433
				],
				[
					-134.5235296947826,
					231.69567625919433
				],
				[
					-133.93994898047004,
					231.69567625919433
				],
				[
					-133.35631483448606,
					231.69567625919433
				],
				[
					-133.06452447732954,
					231.69567625919433
				],
				[
					-132.48089033134556,
					231.69567625919433
				],
				[
					-131.89725618536158,
					231.69567625919433
				],
				[
					-131.02183168222132,
					231.40388590203804
				],
				[
					-130.14640717908105,
					231.40388590203804
				],
				[
					-129.27098267594056,
					231.40388590203804
				],
				[
					-128.103767815644,
					231.40388590203804
				],
				[
					-126.64470916651953,
					231.11209554488164
				],
				[
					-125.47749430622298,
					231.11209554488164
				],
				[
					-124.31027944592643,
					231.11209554488164
				],
				[
					-123.14301115395847,
					230.82025175605395
				],
				[
					-121.6840059365054,
					230.82025175605395
				],
				[
					-120.51673764453744,
					230.52846139889766
				],
				[
					-119.34952278424066,
					230.23667104174137
				],
				[
					-117.89046413511642,
					229.6530368957574
				],
				[
					-116.13961512883589,
					229.3612465386011
				],
				[
					-114.38876612255513,
					228.48582203546073
				],
				[
					-112.63791711627437,
					227.90218788947675
				],
				[
					-110.59527775283732,
					226.73497302918008
				],
				[
					-109.13621910371307,
					225.85954852603982
				],
				[
					-107.38537009743254,
					224.69228023407175
				],
				[
					-105.63452109115178,
					223.81685573093137
				],
				[
					-103.88367208487125,
					223.2332750166188
				],
				[
					-102.42466686741818,
					222.6496408706348
				],
				[
					-101.25739857545022,
					222.06600672465083
				],
				[
					-100.09018371515367,
					221.77421636749443
				],
				[
					-99.21475921201318,
					221.19058222151045
				],
				[
					-98.04754435171662,
					220.89879186435405
				],
				[
					-96.88027605974867,
					220.31515771837007
				],
				[
					-95.4212708422956,
					220.0233673612138
				],
				[
					-93.96221219317113,
					219.4397332152298
				],
				[
					-92.2113631868906,
					218.56430871208954
				],
				[
					-90.16872382345355,
					217.98072799777674
				],
				[
					-87.83424067118904,
					217.10530349463647
				],
				[
					-85.4997575189243,
					216.2298789914962
				],
				[
					-83.16532779833096,
					215.35445448835583
				],
				[
					-80.53905428890994,
					214.18718619638776
				],
				[
					-77.62093699066145,
					213.3117616932475
				],
				[
					-75.5782976272244,
					213.0199713360912
				],
				[
					-73.53565826378735,
					212.14454683295094
				],
				[
					-72.07659961466311,
					211.56091268696684
				],
				[
					-69.74211646239837,
					210.97733197265416
				],
				[
					-68.28311124494553,
					210.39369782667018
				],
				[
					-66.82405259582129,
					210.1019074695139
				],
				[
					-65.07320358954053,
					209.22648296637362
				],
				[
					-63.03056422610348,
					208.93463917754593
				],
				[
					-61.571505576979234,
					208.35105846323324
				],
				[
					-59.8206565706987,
					207.47563396009286
				],
				[
					-57.778017207261655,
					207.18379017126517
				],
				[
					-55.735324412153204,
					206.6002094569526
				],
				[
					-53.98447540587267,
					205.72478495381222
				],
				[
					-51.941836042435625,
					205.43294116498464
				],
				[
					-49.607352890171114,
					204.84936045067184
				],
				[
					-47.56471352673407,
					203.97393594753157
				],
				[
					-45.23023037446933,
					203.0985114443913
				],
				[
					-43.18759101103251,
					202.51487729840733
				],
				[
					-40.853107858767544,
					201.93124315242335
				],
				[
					-39.10225885248701,
					201.34766243811055
				],
				[
					-37.059619489049965,
					200.76402829212657
				],
				[
					-35.30877048276943,
					200.47223793497028
				],
				[
					-33.84971183364496,
					199.59681343183001
				],
				[
					-31.80707247020814,
					199.01317928584604
				],
				[
					-29.764433106771094,
					198.42954513986194
				],
				[
					-27.72174031166287,
					197.55412063672156
				],
				[
					-25.679100948225823,
					196.970539922409
				],
				[
					-23.636461584788776,
					196.386905776425
				],
				[
					-21.593768789680553,
					195.51148127328474
				],
				[
					-19.551129426243506,
					194.92784712730065
				],
				[
					-17.216646273978768,
					194.05242262416027
				],
				[
					-14.298582407401682,
					193.17699812102
				],
				[
					-12.255943043964635,
					192.59341740670743
				],
				[
					-10.213250248856184,
					191.42614911473936
				],
				[
					-7.878820528263077,
					190.84256840042667
				],
				[
					-5.544337375998339,
					189.9671438972864
				],
				[
					-3.793488369717579,
					189.09171939414603
				],
				[
					-1.7508490062807596,
					188.50808524816205
				],
				[
					-0.2917903571565148,
					187.92445110217807
				],
				[
					0.8754245031402661,
					187.34087038786538
				],
				[
					2.6262735094210257,
					186.4654458847251
				],
				[
					4.377122515701558,
					185.88181173874113
				],
				[
					6.419815310810009,
					185.29817759275716
				],
				[
					8.17066431709054,
					184.42275308961678
				],
				[
					9.921513323371073,
					183.5473285864764
				],
				[
					12.547786832792099,
					182.96374787216382
				],
				[
					14.298635839072858,
					182.08832336902344
				],
				[
					16.633065559666193,
					181.21289886588306
				],
				[
					18.675758354774416,
					180.3374743627428
				],
				[
					20.718397718211463,
					179.17020607077484
				],
				[
					22.761037081648283,
					178.29478156763446
				],
				[
					24.511886087929042,
					177.41935706449408
				],
				[
					25.970944737053287,
					176.5439325613538
				],
				[
					27.721793743334047,
					175.66850805821355
				],
				[
					29.18085239245829,
					175.08492734390086
				],
				[
					30.348067252755072,
					173.9176590519328
				],
				[
					32.09891625903583,
					173.6258686947765
				],
				[
					32.97434076217587,
					173.04223454879252
				],
				[
					34.72518976845663,
					172.45865383447983
				],
				[
					35.600614271596896,
					171.87501968849585
				],
				[
					37.05967292072137,
					171.29138554251188
				],
				[
					38.22688778101792,
					170.7078048281992
				],
				[
					39.394102641314475,
					170.4159610393715
				],
				[
					40.85316129043895,
					169.54053653623123
				],
				[
					41.728585793579214,
					169.24874617907494
				],
				[
					42.895800653875995,
					168.66511203309096
				],
				[
					43.77122515701626,
					168.08153131877816
				],
				[
					44.64664966015653,
					167.49789717279418
				],
				[
					45.813917952124484,
					167.2061068156379
				],
				[
					46.39749866643706,
					166.62247266965392
				],
				[
					47.564766958405244,
					166.03883852366994
				],
				[
					48.731981818702025,
					165.45525780935725
				],
				[
					49.60740632184206,
					164.87162366337327
				],
				[
					50.774621182138844,
					164.28798951738918
				],
				[
					51.9418894741068,
					163.9961991602329
				],
				[
					52.81731397724707,
					163.7044088030766
				],
				[
					54.276319194700136,
					163.4125650142489
				],
				[
					54.859953340684115,
					163.12077465709262
				],
				[
					56.02716820098067,
					162.82895758410064
				],
				[
					57.194436492948626,
					162.24535015395236
				],
				[
					58.06986099608912,
					162.24535015395236
				],
				[
					58.653441710401694,
					161.95353308096026
				],
				[
					59.52886621354219,
					161.66171600796827
				],
				[
					60.40429071668245,
					161.36992565081187
				],
				[
					61.27971521982272,
					161.07810857781988
				],
				[
					62.44698351179068,
					160.4945011476716
				],
				[
					63.03056422610325,
					160.2026840746796
				],
				[
					63.905988729243745,
					159.91086700168762
				],
				[
					64.78141323238401,
					159.32725957153934
				],
				[
					65.65683773552428,
					159.03544249854735
				],
				[
					66.53226223866477,
					158.74365214139095
				],
				[
					67.40768674180504,
					158.74365214139095
				],
				[
					68.2831112449453,
					158.45183506839896
				],
				[
					69.45037953691326,
					158.16001799540697
				],
				[
					70.32580404005375,
					157.86822763825057
				],
				[
					71.49301890035031,
					157.57641056525858
				],
				[
					72.66023376064686,
					157.2845934922666
				],
				[
					73.24386790663084,
					157.2845934922666
				],
				[
					74.11929240977133,
					156.9928031351103
				],
				[
					74.9947169129116,
					156.9928031351103
				],
				[
					74.9947169129116,
					156.70098606211832
				],
				[
					75.5783510588958,
					156.70098606211832
				],
				[
					76.16193177320838,
					156.40916898912633
				],
				[
					76.16193177320838,
					156.11737863197004
				],
				[
					76.45377556203584,
					156.11737863197004
				],
				[
					76.74556591919236,
					155.82556155897805
				],
				[
					77.03735627634865,
					155.82556155897805
				],
				[
					77.03735627634865,
					155.53374448598606
				],
				[
					77.32920006517634,
					155.53374448598606
				],
				[
					77.32920006517634,
					155.24195412882966
				],
				[
					77.62099042233262,
					155.24195412882966
				],
				[
					77.91278077948891,
					155.24195412882966
				],
				[
					78.2046245683166,
					155.24195412882966
				],
				[
					78.49641492547289,
					154.95013705583767
				],
				[
					79.08004907145687,
					154.95013705583767
				],
				[
					79.37183942861338,
					154.65831998284568
				],
				[
					79.66362978576944,
					154.65831998284568
				],
				[
					79.66362978576944,
					154.36652962568928
				],
				[
					79.66362978576944,
					154.0747125526973
				],
				[
					79.66362978576944,
					154.0747125526973
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 23,
			"versionNonce": 1262671344,
			"isDeleted": false,
			"id": "_7vyMmhVTKAqK8k6GQg-4",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3367.384143920967,
			"y": -342.7298132934783,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.544337375998111,
			"height": 6.711578952130594,
			"seed": 1582867216,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.2917903571562874,
					-0.2917903571562874
				],
				[
					-0.2917903571562874,
					-0.5836074301483904
				],
				[
					-0.5835807143125749,
					-1.1672148602966672
				],
				[
					-1.1672148602965535,
					-1.4590319332886565
				],
				[
					-1.7508490062805322,
					-2.0426393634369333
				],
				[
					-2.042639363437047,
					-2.0426393634369333
				],
				[
					-2.3344297205933344,
					-2.626273509420912
				],
				[
					-2.6262735094210257,
					-2.918063866577313
				],
				[
					-2.918063866577313,
					-3.5016980125612918
				],
				[
					-3.5016980125612918,
					-3.5016980125612918
				],
				[
					-3.793488369717579,
					-3.793488369717693
				],
				[
					-4.085278726874094,
					-4.668912872857959
				],
				[
					-4.377122515701558,
					-4.960729945849948
				],
				[
					-4.668912872858073,
					-5.252547018841938
				],
				[
					-5.252547018842051,
					-6.127971521982204
				],
				[
					-5.544337375998111,
					-6.419761879138605
				],
				[
					-5.544337375998111,
					-6.711578952130594
				],
				[
					-5.544337375998111,
					-6.711578952130594
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 295,
			"versionNonce": 441620464,
			"isDeleted": false,
			"id": "IgbACX7eNlqCnO4uxdXEG",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3221.48009568536,
			"y": -601.2718587928663,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 293.26720855200915,
			"height": 113.22157797809405,
			"seed": 527548688,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.8754245031404935,
					0
				],
				[
					-1.1672682919679573,
					0
				],
				[
					-2.918117298248717,
					0
				],
				[
					-4.377122515701558,
					0.29181707299198933
				],
				[
					-6.127971521982317,
					0.8754245031403229
				],
				[
					-8.17066431709054,
					1.4590319332886565
				],
				[
					-10.213303680527588,
					2.042666079272635
				],
				[
					-12.839577189948614,
					2.918090582413015
				],
				[
					-15.174060342213124,
					3.793515085553281
				],
				[
					-18.092124208790665,
					4.668939588693661
				],
				[
					-21.01018807536775,
					5.252547018841938
				],
				[
					-23.636461584788776,
					5.836154448990328
				],
				[
					-25.970944737053514,
					6.419788594974307
				],
				[
					-28.305427889318253,
					7.0033960251225835
				],
				[
					-30.93170139873905,
					7.587003455270974
				],
				[
					-33.266131119332385,
					7.878820528262963
				],
				[
					-35.600614271597124,
					8.170637601254953
				],
				[
					-38.8105219270019,
					9.046062104395276
				],
				[
					-41.72858579357944,
					9.62966953454361
				],
				[
					-44.64664966015653,
					10.505094037683875
				],
				[
					-48.44019146154551,
					11.380518540824255
				],
				[
					-51.65004568527911,
					12.547760116956567
				],
				[
					-55.15174369784063,
					13.42318462009689
				],
				[
					-58.94528549922961,
					14.882216553385547
				],
				[
					-62.15513972296321,
					16.341248486674203
				],
				[
					-65.36504737836822,
					17.216672989814526
				],
				[
					-68.86674539092951,
					18.38391456594684
				],
				[
					-71.78480925750682,
					19.25933906908716
				],
				[
					-74.11929240977133,
					19.842946499235495
				],
				[
					-76.16193177320838,
					20.426580645219474
				],
				[
					-77.62099042233285,
					20.718371002375818
				],
				[
					-79.66362978576967,
					21.302005148359854
				],
				[
					-80.24726393175365,
					21.59379550551614
				],
				[
					-81.99811293803441,
					21.88561257850813
				],
				[
					-82.87353744117468,
					22.17742965150012
				],
				[
					-84.33259609029892,
					22.46922000865652
				],
				[
					-86.08344509657968,
					23.344644511796787
				],
				[
					-87.83429410286044,
					23.928278657780766
				],
				[
					-90.16872382345355,
					24.803703160921145
				],
				[
					-92.211416618562,
					25.387310591069422
				],
				[
					-94.5458463391551,
					26.55455216720179
				],
				[
					-97.17211984857613,
					27.138159597350068
				],
				[
					-98.92296885485689,
					28.013584100490448
				],
				[
					-100.96566164996511,
					28.88900860363077
				],
				[
					-103.00830101340216,
					29.18082567662276
				],
				[
					-104.46735966252663,
					30.056250179763083
				],
				[
					-105.92636487997947,
					30.348040536919427
				],
				[
					-107.67721388626023,
					30.931674682903406
				],
				[
					-109.13627253538448,
					31.51528211305174
				],
				[
					-110.30348739568126,
					32.09888954320007
				],
				[
					-111.76254604480528,
					32.39070661619206
				],
				[
					-113.22160469392975,
					32.974314046340396
				],
				[
					-114.97245370021028,
					33.84973854948072
				],
				[
					-117.01509306364733,
					34.433372695464755
				],
				[
					-119.05773242708437,
					35.30879719860502
				],
				[
					-121.10042522219283,
					36.1842217017454
				],
				[
					-123.43485494278593,
					37.05964620488567
				],
				[
					-126.64476259819094,
					37.935070708026046
				],
				[
					-127.81197745848749,
					38.81049521116631
				],
				[
					-130.43825096790852,
					39.3941026413147
				],
				[
					-131.897309617033,
					40.26952714445497
				],
				[
					-133.64815862331352,
					41.14495164759535
				],
				[
					-135.107217272438,
					41.43676872058734
				],
				[
					-136.85806627871852,
					42.020376150735615
				],
				[
					-138.3170714961716,
					42.603983580884005
				],
				[
					-140.06792050245213,
					42.895800653875995
				],
				[
					-141.5269791515766,
					43.77122515701626
				],
				[
					-142.98603780070084,
					44.06304223000831
				],
				[
					-145.0286771641379,
					44.64664966015664
				],
				[
					-147.0713165275747,
					45.52207416329696
				],
				[
					-149.11400932268316,
					46.397498666437286
				],
				[
					-151.4484390432765,
					47.27292316957761
				],
				[
					-154.0747125526973,
					48.14834767271793
				],
				[
					-156.40919570496203,
					48.731955102866266
				],
				[
					-158.45183506839908,
					49.89919667899858
				],
				[
					-161.07810857781988,
					50.48280410914691
				],
				[
					-162.82895758410064,
					51.358228612287235
				],
				[
					-164.28801623322488,
					52.23365311542756
				],
				[
					-166.03886523950564,
					52.52547018841955
				],
				[
					-167.7897142457864,
					53.10907761856788
				],
				[
					-169.24877289491064,
					53.9845021217082
				],
				[
					-170.99962190119118,
					54.27631919470019
				],
				[
					-172.75047090747194,
					55.151743697840516
				],
				[
					-174.79311027090898,
					55.73535112798885
				],
				[
					-176.8357496343458,
					56.318985273972885
				],
				[
					-178.87844242945425,
					57.486200134269495
				],
				[
					-181.50471593887505,
					58.36162463740982
				],
				[
					-183.5473553023121,
					59.2370491405502
				],
				[
					-185.58999466574915,
					60.40429071668245
				],
				[
					-187.92447781801366,
					60.987898146830844
				],
				[
					-190.2589609702784,
					61.863322649971224
				],
				[
					-192.00980997655915,
					63.03056422610348
				],
				[
					-193.7606589828397,
					63.32238129909547
				],
				[
					-195.21969091612846,
					64.19780580223573
				],
				[
					-196.3869324922607,
					64.78141323238412
				],
				[
					-198.13778149854124,
					65.36502066253252
				],
				[
					-199.59681343183001,
					65.6568377355245
				],
				[
					-201.05584536511878,
					66.24044516567278
				],
				[
					-202.80669437139932,
					66.53226223866477
				],
				[
					-204.84936045067207,
					67.69950381479703
				],
				[
					-207.18381688710087,
					68.28311124494542
				],
				[
					-209.5183000393656,
					69.1585357480858
				],
				[
					-211.85275647579465,
					70.03396025122606
				],
				[
					-213.89542255506717,
					70.61756768137434
				],
				[
					-216.2298789914962,
					71.78480925750671
				],
				[
					-217.98072799777674,
					72.66023376064709
				],
				[
					-219.4397599310655,
					72.95205083363908
				],
				[
					-221.19060893734604,
					73.82747533677934
				],
				[
					-222.06603344048654,
					74.11926569393563
				],
				[
					-223.2332750166188,
					74.41108276692773
				],
				[
					-224.10869951975928,
					74.99469019707601
				],
				[
					-225.56773145304783,
					75.5783243430601
				],
				[
					-226.73497302918008,
					75.87011470021639
				],
				[
					-227.90221460531257,
					76.45374884620037
				],
				[
					-229.06942946560912,
					77.03735627634865
				],
				[
					-230.52848811473336,
					77.62096370649704
				],
				[
					-231.69570297503014,
					78.20459785248102
				],
				[
					-233.1547616241544,
					79.0800223556214
				],
				[
					-234.03018612729466,
					79.37181271277768
				],
				[
					-235.78103513357541,
					79.95544685876166
				],
				[
					-236.0728254907317,
					80.24723721591795
				],
				[
					-236.65645963671568,
					80.53905428890994
				],
				[
					-237.24006706686396,
					80.83087136190193
				],
				[
					-237.53188413985617,
					81.12266171905833
				],
				[
					-237.82367449701223,
					81.41447879205032
				],
				[
					-238.11549157000445,
					81.41447879205032
				],
				[
					-238.11549157000445,
					81.7062958650423
				],
				[
					-238.40730864299644,
					81.7062958650423
				],
				[
					-238.11549157000445,
					81.7062958650423
				],
				[
					-237.82367449701223,
					81.99808622219871
				],
				[
					-236.94824999387197,
					82.2899032951907
				],
				[
					-236.65645963671568,
					82.58172036818269
				],
				[
					-236.3646425637237,
					82.58172036818269
				],
				[
					-236.0728254907317,
					82.87351072533897
				],
				[
					-236.0728254907317,
					83.45714487132295
				],
				[
					-235.78103513357541,
					83.74893522847924
				],
				[
					-235.19740098759144,
					84.33256937446322
				],
				[
					-234.90561063043515,
					84.33256937446322
				],
				[
					-234.61379355744293,
					84.62435973161962
				],
				[
					-234.32197648445117,
					84.91617680461161
				],
				[
					-233.44655198131068,
					85.2079938776036
				],
				[
					-232.5711274781704,
					85.2079938776036
				],
				[
					-231.69570297503014,
					85.49978423476
				],
				[
					-230.82027847188965,
					85.79160130775199
				],
				[
					-229.3612465386011,
					85.79160130775199
				],
				[
					-228.48582203546084,
					85.79160130775199
				],
				[
					-227.02679010217207,
					86.08341838074398
				],
				[
					-225.85954852603982,
					86.08341838074398
				],
				[
					-224.69230694990756,
					86.08341838074398
				],
				[
					-223.2332750166188,
					86.37520873790027
				],
				[
					-221.77424308333025,
					86.66702581089226
				],
				[
					-220.60700150719777,
					86.95884288388424
				],
				[
					-218.85615250091723,
					87.25063324104053
				],
				[
					-217.10530349463647,
					87.25063324104053
				],
				[
					-215.64627156134793,
					87.83426738702462
				],
				[
					-213.60360548207518,
					87.83426738702462
				],
				[
					-211.85275647579465,
					87.83426738702462
				],
				[
					-209.8100903965219,
					87.83426738702462
				],
				[
					-208.35105846323336,
					87.83426738702462
				],
				[
					-206.01660202680432,
					87.83426738702462
				],
				[
					-203.68211887453958,
					87.83426738702462
				],
				[
					-200.47223793497028,
					87.83426738702462
				],
				[
					-197.84596442554948,
					87.83426738702462
				],
				[
					-194.92787384313647,
					87.83426738702462
				],
				[
					-191.71796618773146,
					87.83426738702462
				],
				[
					-188.79990232115415,
					87.83426738702462
				],
				[
					-185.29820430859286,
					87.83426738702462
				],
				[
					-183.2555649451558,
					87.54245031403252
				],
				[
					-180.3374476469071,
					87.25063324104053
				],
				[
					-178.29480828347027,
					86.66702581089226
				],
				[
					-175.96032513120554,
					86.37520873790027
				],
				[
					-173.3340516217845,
					86.08341838074398
				],
				[
					-170.99962190119118,
					85.79160130775199
				],
				[
					-168.37334839177038,
					85.49978423476
				],
				[
					-166.03886523950564,
					85.2079938776036
				],
				[
					-163.12080137292833,
					84.91617680461161
				],
				[
					-160.78631822066382,
					84.62435973161962
				],
				[
					-158.1600447112428,
					84.04075230147123
				],
				[
					-155.24198084466548,
					84.04075230147123
				],
				[
					-152.90749769240074,
					84.04075230147123
				],
				[
					-150.2812241829797,
					83.74893522847924
				],
				[
					-147.3631603164024,
					83.45714487132295
				],
				[
					-144.15325266099762,
					83.16532779833096
				],
				[
					-141.81876950873288,
					82.87351072533897
				],
				[
					-139.48433978813955,
					82.58172036818269
				],
				[
					-136.56622248989083,
					82.2899032951907
				],
				[
					-133.64815862331352,
					81.99808622219871
				],
				[
					-131.0218851138925,
					81.7062958650423
				],
				[
					-128.68740196162798,
					81.41447879205032
				],
				[
					-126.06112845220696,
					81.12266171905833
				],
				[
					-123.43485494278593,
					80.83087136190193
				],
				[
					-120.8085814333649,
					80.83087136190193
				],
				[
					-118.18230792394388,
					80.83087136190193
				],
				[
					-115.2642440573668,
					80.83087136190193
				],
				[
					-112.92976090510206,
					80.83087136190193
				],
				[
					-110.88712154166524,
					80.53905428890994
				],
				[
					-108.26084803224421,
					80.53905428890994
				],
				[
					-105.92636487997947,
					80.24723721591795
				],
				[
					-103.88372551654265,
					80.24723721591795
				],
				[
					-101.8410861531056,
					80.24723721591795
				],
				[
					-99.21481264368458,
					79.95544685876166
				],
				[
					-97.75575399456011,
					79.95544685876166
				],
				[
					-95.4212708422956,
					79.95544685876166
				],
				[
					-92.79499733287457,
					79.95544685876166
				],
				[
					-90.16872382345355,
					79.95544685876166
				],
				[
					-87.25065995687646,
					79.95544685876166
				],
				[
					-84.62438644745544,
					79.95544685876166
				],
				[
					-81.99811293803441,
					79.95544685876166
				],
				[
					-79.37183942861338,
					79.95544685876166
				],
				[
					-77.32920006517634,
					79.95544685876166
				],
				[
					-75.28650727006811,
					79.95544685876166
				],
				[
					-72.95207754947478,
					79.95544685876166
				],
				[
					-71.20122854319425,
					80.24723721591795
				],
				[
					-68.57495503377322,
					80.24723721591795
				],
				[
					-66.82410602749246,
					80.24723721591795
				],
				[
					-64.48962287522772,
					80.24723721591795
				],
				[
					-62.44698351179068,
					80.53905428890994
				],
				[
					-60.40429071668268,
					80.53905428890994
				],
				[
					-58.06986099608912,
					80.83087136190193
				],
				[
					-55.73537784382461,
					80.83087136190193
				],
				[
					-53.10910433440358,
					81.12266171905833
				],
				[
					-50.48283082498256,
					81.12266171905833
				],
				[
					-48.148347672718046,
					81.12266171905833
				],
				[
					-45.813917952124484,
					81.12266171905833
				],
				[
					-43.187644442703686,
					81.41447879205032
				],
				[
					-40.85316129043895,
					81.7062958650423
				],
				[
					-39.102312284158415,
					81.99808622219871
				],
				[
					-37.35146327787788,
					82.2899032951907
				],
				[
					-35.89240462875341,
					82.58172036818269
				],
				[
					-34.43339941130034,
					82.87351072533897
				],
				[
					-33.266131119332385,
					83.16532779833096
				],
				[
					-31.807125901879317,
					83.16532779833096
				],
				[
					-30.63985760991136,
					83.45714487132295
				],
				[
					-28.597218246474313,
					84.04075230147123
				],
				[
					-26.554578883037493,
					84.62435973161962
				],
				[
					-23.928305373616467,
					84.91617680461161
				],
				[
					-21.885612578508244,
					85.49978423476
				],
				[
					-19.25933906908722,
					86.37520873790027
				],
				[
					-16.924909348493884,
					86.95884288388424
				],
				[
					-14.298635839072858,
					87.54245031403252
				],
				[
					-12.255943043964635,
					88.12605774418091
				],
				[
					-10.213303680527588,
					88.709691890165
				],
				[
					-8.462454674247056,
					89.29329932031328
				],
				[
					-6.419815310810009,
					89.58511639330527
				],
				[
					-4.9607566616855365,
					90.16872382345355
				],
				[
					-2.918117298248717,
					90.46054089644554
				],
				[
					-1.4590586491244721,
					91.33596539958592
				],
				[
					0.2917903571562874,
					91.6277557567422
				],
				[
					1.7508490062805322,
					92.2113899027263
				],
				[
					4.377122515701558,
					93.08681440586656
				],
				[
					6.12797152198209,
					93.67042183601484
				],
				[
					8.754245031403116,
					94.54584633915522
				],
				[
					10.796884394840163,
					95.12945376930361
				],
				[
					13.714948261417476,
					96.00487827244388
				],
				[
					16.049431413682214,
					97.17211984857613
				],
				[
					18.67570492310324,
					97.75572727872452
				],
				[
					21.301978432524265,
					98.92296885485689
				],
				[
					23.344617795961085,
					99.79839335799716
				],
				[
					25.679100948225823,
					100.09021043098915
				],
				[
					27.138159597350068,
					100.96563493412941
				],
				[
					29.180798960786888,
					101.5492423642778
				],
				[
					30.63985760991136,
					101.84105943726979
				],
				[
					32.09886282736443,
					102.42466686741818
				],
				[
					33.84971183364496,
					103.00827429756646
				],
				[
					34.725136336785454,
					103.30009137055845
				],
				[
					35.60056083992572,
					103.59190844355044
				],
				[
					36.475985343065986,
					103.88369880070672
				],
				[
					37.059619489049965,
					104.17551587369871
				],
				[
					37.93504399219046,
					104.46733294669082
				],
				[
					38.8104684953305,
					105.0509403768391
				],
				[
					39.97768335562728,
					105.3427574498312
				],
				[
					41.144951647595235,
					105.63454780698748
				],
				[
					42.6039568650483,
					106.50997231012775
				],
				[
					43.77122515701626,
					106.80178938311974
				],
				[
					45.2302303744691,
					107.38539681326802
				],
				[
					46.98107938074986,
					107.96903095925211
				],
				[
					48.148347672718046,
					108.5526383894005
				],
				[
					49.3155625330146,
					108.84445546239249
				],
				[
					50.190987036154866,
					109.42806289254077
				],
				[
					51.06641153929513,
					109.71987996553275
				],
				[
					51.06641153929513,
					110.01167032268904
				],
				[
					51.35820189645165,
					110.59530446867302
				],
				[
					51.65004568527911,
					110.59530446867302
				],
				[
					52.525470188419604,
					111.17891189882141
				],
				[
					52.81726054557589,
					111.7625193289698
				],
				[
					53.40089469155987,
					112.05433640196179
				],
				[
					54.276319194700136,
					112.34615347495378
				],
				[
					54.56810955185665,
					112.92976090510206
				],
				[
					54.85989990901271,
					113.22157797809405
				],
				[
					54.85989990901271,
					113.22157797809405
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 24,
			"versionNonce": 907680240,
			"isDeleted": false,
			"id": "rag386mEs1oijb8rnAN_8",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2785.0246277238275,
			"y": -214.62296371158652,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 19.6561650346066,
			"height": 20.32624019065065,
			"seed": 1538727696,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.22337201847813049,
					0
				],
				[
					0.4467440369560336,
					0.44672358726108996
				],
				[
					1.1168396426951404,
					1.3401912114782135
				],
				[
					1.5635632299561166,
					2.4570104044784102
				],
				[
					2.680382422956427,
					4.0205736344346406
				],
				[
					3.7972220656515674,
					5.80748843317383
				],
				[
					5.584136864390757,
					7.5944236816080775
				],
				[
					7.371051663129947,
					9.381338480347267
				],
				[
					9.8280825173033,
					11.61499731604249
				],
				[
					11.838369334520621,
					13.625284133259811
				],
				[
					14.072007720520787,
					15.412198931999
				],
				[
					15.635570950477131,
					16.97576216195523
				],
				[
					17.199134180433248,
					17.869209336477297
				],
				[
					18.315973823128388,
					18.762676960694535
				],
				[
					19.209420997650568,
					19.432772566433528
				],
				[
					19.6561650346066,
					19.879496153694618
				],
				[
					19.6561650346066,
					20.102868172172634
				],
				[
					19.6561650346066,
					20.32624019065065
				],
				[
					19.6561650346066,
					20.32624019065065
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 21,
			"versionNonce": 832658416,
			"isDeleted": false,
			"id": "gY_CROlFpfFD753H-RQ_G",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2804.680792758434,
			"y": -194.29672352093587,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 27.027175798346434,
			"height": 14.742103326259894,
			"seed": 1671478544,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.2233515687828458,
					0
				],
				[
					1.1167987433050257,
					-0.4467440369560336
				],
				[
					2.4569899547832392,
					-1.5635632299561166
				],
				[
					4.69066924017352,
					-2.457030854173354
				],
				[
					7.594403231912793,
					-3.7972220656514537
				],
				[
					10.051434086086147,
					-4.91404125865165
				],
				[
					13.8486152523476,
					-6.70095605739084
				],
				[
					16.305646106520953,
					-8.041147268869054
				],
				[
					19.656124135216487,
					-10.05143408608626
				],
				[
					21.666410952433807,
					-11.391625297564474
				],
				[
					23.6766977696509,
					-12.508464940259614
				],
				[
					25.016888981129114,
					-13.40191211478168
				],
				[
					26.133728623824254,
					-14.072007720520787
				],
				[
					27.027175798346434,
					-14.51875175747682
				],
				[
					27.027175798346434,
					-14.742103326259894
				],
				[
					27.027175798346434,
					-14.742103326259894
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 24,
			"versionNonce": 2129681904,
			"isDeleted": false,
			"id": "Zrh142jEbn8PfFQYwIw13",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2831.7079685567805,
			"y": -209.03882684719576,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 7.371051663129947,
			"height": 7.594423681607964,
			"seed": 950442768,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.22335156878307316,
					0
				],
				[
					-0.6700956057391068,
					-0.2233720184780168
				],
				[
					-1.1168396426951404,
					-0.4467440369560336
				],
				[
					-2.0102868172173203,
					-0.6700956057391068
				],
				[
					-2.457030854173354,
					-1.3401912114782135
				],
				[
					-3.1271264599124606,
					-1.7869352484342471
				],
				[
					-3.5738295974783796,
					-2.457030854173354
				],
				[
					-4.243925203217486,
					-3.127126459912347
				],
				[
					-4.914020808956593,
					-3.7972220656514537
				],
				[
					-5.5841164146957,
					-4.4673176713905605
				],
				[
					-6.0308604516517335,
					-5.137413277129667
				],
				[
					-6.254212020434807,
					-5.584136864390757
				],
				[
					-6.70095605739084,
					-6.25423247012975
				],
				[
					-6.924307626173913,
					-6.70095605739084
				],
				[
					-7.147700094346874,
					-6.924328075868857
				],
				[
					-7.371051663129947,
					-7.147700094346874
				],
				[
					-7.371051663129947,
					-7.371051663129947
				],
				[
					-7.371051663129947,
					-7.594423681607964
				],
				[
					-7.371051663129947,
					-7.594423681607964
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 25,
			"versionNonce": 252649456,
			"isDeleted": false,
			"id": "nn4PVZ678aAS3dGIJK7F8",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2783.237712925088,
			"y": -218.64353734602093,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.40191211478168,
			"height": 10.27480610456439,
			"seed": 1832958224,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.22337201847813049,
					0
				],
				[
					0.6700956057391068,
					-0.22337201847813049
				],
				[
					0.8934676242170099,
					-0.8934676242171236
				],
				[
					1.5635632299561166,
					-1.3401912114782135
				],
				[
					2.680382422956427,
					-2.0102868172173203
				],
				[
					3.79720161595651,
					-2.680382422956427
				],
				[
					4.91404125865165,
					-3.350478028695534
				],
				[
					5.807488433173603,
					-4.243945652912544
				],
				[
					7.1476796446518165,
					-5.137392827434724
				],
				[
					8.48787085613003,
					-6.030860451651847
				],
				[
					9.828062067608244,
					-6.924328075868971
				],
				[
					10.944901710303384,
					-7.817775250391037
				],
				[
					11.838348884825564,
					-8.487870856130144
				],
				[
					12.731816509042574,
					-9.381338480347267
				],
				[
					12.955188527520704,
					-9.604710498825284
				],
				[
					13.17854009630355,
					-9.828062067608244
				],
				[
					13.17854009630355,
					-10.051434086086374
				],
				[
					13.17854009630355,
					-10.27480610456439
				],
				[
					13.40191211478168,
					-10.27480610456439
				],
				[
					13.40191211478168,
					-10.27480610456439
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 11,
			"versionNonce": 1912971760,
			"isDeleted": false,
			"id": "QN6n0p5dmmM8iwZXuaihF",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 2797.533092664087,
			"y": -228.47159941362918,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 0.8934471745221799,
			"height": 0.8934471745220662,
			"seed": 82253584,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.22335156878307316,
					0.22335156878295948
				],
				[
					0.6700956057393341,
					0.4467235872609763
				],
				[
					0.6700956057393341,
					0.6700956057389931
				],
				[
					0.8934471745221799,
					0.8934471745220662
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
			"version": 183,
			"versionNonce": 1994122224,
			"isDeleted": false,
			"id": "JiK6E6yxHFZa6KdvnNLe1",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3776.5938425364684,
			"y": -27.060860954184022,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 32.71179040720972,
			"height": 30.375166718256196,
			"seed": 1410446608,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.9346494755814092,
					0
				],
				[
					-2.336580905401661,
					-1.401931429820479
				],
				[
					-3.27123038098307,
					-2.336538121850026
				],
				[
					-5.140443765042164,
					-4.205794289460982
				],
				[
					-7.009657149101258,
					-5.140400981490529
				],
				[
					-8.878956100264531,
					-7.94426384113126
				],
				[
					-11.682818959905035,
					-11.215451438562695
				],
				[
					-14.019314298202971,
					-14.019314298203199
				],
				[
					-17.290544679186496,
					-16.823177157843702
				],
				[
					-20.561689493065842,
					-20.56164670951398
				],
				[
					-22.898270398467503,
					-22.898184831364006
				],
				[
					-25.23476573676544,
					-24.767440998974962
				],
				[
					-28.038628596405943,
					-26.63669716658592
				],
				[
					-29.907927547569216,
					-28.038628596406397
				],
				[
					-31.77714093162831,
					-28.973235288435944
				],
				[
					-32.24442288586715,
					-29.90784198046549
				],
				[
					-32.71179040720972,
					-30.375166718256196
				],
				[
					-32.71179040720972,
					-30.375166718256196
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 191,
			"versionNonce": 1268377072,
			"isDeleted": false,
			"id": "xX36W0yB-gmCcsTBD7QUj",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3744.3494196505994,
			"y": -57.436027672440446,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 99.0697639958994,
			"height": 6.542332411310781,
			"seed": 1614320400,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0.46728195423884245,
					0
				],
				[
					0.9345639084776849,
					0
				],
				[
					1.869213384059094,
					0
				],
				[
					2.803862859640958,
					0
				],
				[
					3.738426768118188,
					0
				],
				[
					4.673076243699597,
					0
				],
				[
					6.075007673520304,
					0
				],
				[
					7.944221057579398,
					0
				],
				[
					10.280801962981059,
					0.4673247377907046
				],
				[
					12.61738286838272,
					1.4019314298202517
				],
				[
					16.355809636500908,
					1.8692561676111836
				],
				[
					20.094321971723275,
					2.8038628596405033
				],
				[
					25.234765736765894,
					3.2711875974314353
				],
				[
					31.777055364524585,
					4.205794289460982
				],
				[
					39.254080034968865,
					5.140400981490529
				],
				[
					49.06760004371108,
					5.607725719281234
				],
				[
					58.8811200524533,
					5.607725719281234
				],
				[
					69.16192201543436,
					6.075050457071939
				],
				[
					77.57351059435632,
					6.075050457071939
				],
				[
					85.05044969769642,
					6.542332411310781
				],
				[
					90.65817541697788,
					6.542332411310781
				],
				[
					94.86396970643864,
					6.542332411310781
				],
				[
					97.66783256607914,
					6.542332411310781
				],
				[
					98.602482041661,
					6.542332411310781
				],
				[
					99.0697639958994,
					6.542332411310781
				],
				[
					99.0697639958994,
					6.542332411310781
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 185,
			"versionNonce": 491235312,
			"isDeleted": false,
			"id": "xU0B1ulTK_mF7ehxpMUhp",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3849.4942768871238,
			"y": -49.024439093518254,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 20.561689493065842,
			"height": 15.888570465814155,
			"seed": 1070838032,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.9346494755814092,
					0.4673247377907046
				],
				[
					-1.4019314298202517,
					0.4673247377907046
				],
				[
					-2.8038628596405033,
					0.934606692029547
				],
				[
					-4.205794289460755,
					2.3365381218497987
				],
				[
					-6.075093240624028,
					3.7384695516700504
				],
				[
					-7.009657149101713,
					5.140400981490529
				],
				[
					-9.813520008742216,
					6.542332411310781
				],
				[
					-11.682818959905035,
					8.878913316712442
				],
				[
					-13.552032343964129,
					10.280844746532921
				],
				[
					-15.421245728023223,
					11.682776176353173
				],
				[
					-16.355895203605087,
					13.084707606173424
				],
				[
					-17.290544679186496,
					13.551989560412267
				],
				[
					-17.75782663342534,
					14.486639035993903
				],
				[
					-18.225108587663726,
					14.486639035993903
				],
				[
					-18.225108587663726,
					14.953920990232518
				],
				[
					-18.692476109006748,
					15.421245728023223
				],
				[
					-19.15975806324559,
					15.421245728023223
				],
				[
					-20.094407538827,
					15.888570465814155
				],
				[
					-20.561689493065842,
					15.888570465814155
				],
				[
					-20.561689493065842,
					15.888570465814155
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 190,
			"versionNonce": 938289648,
			"isDeleted": false,
			"id": "UFj_SbZZ4nG-A1GXExFoP",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3827.9979379184765,
			"y": -27.99546764621425,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 6.075007673519849,
			"height": 80.8446981917873,
			"seed": 2052787984,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.934606692029547
				],
				[
					0,
					1.8692561676109563
				],
				[
					0,
					3.7384695516700504
				],
				[
					0,
					6.075050457071939
				],
				[
					-0.46728195423884245,
					8.878913316712442
				],
				[
					-0.46728195423884245,
					11.682776176353173
				],
				[
					-0.46728195423884245,
					14.953920990232518
				],
				[
					-0.46728195423884245,
					18.692433325454658
				],
				[
					-0.9345639084776849,
					23.365509569154483
				],
				[
					-1.4019314298202517,
					28.03862859640617
				],
				[
					-2.3364953382979365,
					32.71174762365786
				],
				[
					-2.8038628596405033,
					37.38482386735768
				],
				[
					-3.738426768118188,
					42.05794289460937
				],
				[
					-4.20579428946121,
					47.1983438760999
				],
				[
					-5.14035819793844,
					52.33878764114206
				],
				[
					-5.607725719281461,
					57.01186388484189
				],
				[
					-6.075007673519849,
					61.684982912093574
				],
				[
					-6.075007673519849,
					65.89077720155456
				],
				[
					-6.075007673519849,
					69.62924675322483
				],
				[
					-6.075007673519849,
					73.36775908844675
				],
				[
					-6.075007673519849,
					76.17162194808748
				],
				[
					-6.075007673519849,
					78.04083533214657
				],
				[
					-6.075007673519849,
					79.91009149975775
				],
				[
					-6.075007673519849,
					80.8446981917873
				],
				[
					-6.075007673519849,
					80.8446981917873
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 188,
			"versionNonce": 647130096,
			"isDeleted": false,
			"id": "K-JOqq9G6T6l1SqNtBLuP",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3773.7899796768274,
			"y": -30.33200576806405,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 3.7385123352219125,
			"height": 69.16192201543413,
			"seed": 1749462288,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.934606692029547
				],
				[
					0,
					2.8038628596407307
				],
				[
					0,
					5.607725719281234
				],
				[
					0.46728195423884245,
					9.346195270951512
				],
				[
					0.9345639084776849,
					13.084664822621562
				],
				[
					1.4019314298202517,
					17.75778384987325
				],
				[
					1.869213384059094,
					21.496253401543527
				],
				[
					1.869213384059094,
					26.63669716658592
				],
				[
					1.869213384059094,
					31.309773410285743
				],
				[
					1.869213384059094,
					36.450217175328135
				],
				[
					0.9345639084776849,
					41.12329341902796
				],
				[
					0.46728195423884245,
					45.796412446279646
				],
				[
					-0.46736752134256676,
					50.0022067357404
				],
				[
					-0.9346494755814092,
					53.74067628741068
				],
				[
					-0.9346494755814092,
					57.47918862263282
				],
				[
					-1.4019314298202517,
					60.75033343651239
				],
				[
					-1.4019314298202517,
					63.554196296152895
				],
				[
					-1.4019314298202517,
					65.42345246376408
				],
				[
					-1.4019314298202517,
					66.82538389358433
				],
				[
					-1.4019314298202517,
					67.75999058561388
				],
				[
					-1.8692989511628184,
					68.69464006119529
				],
				[
					-1.8692989511628184,
					69.16192201543413
				],
				[
					-1.8692989511628184,
					69.16192201543413
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 188,
			"versionNonce": 1396665840,
			"isDeleted": false,
			"id": "9FBtMzDmWo2Mpwk__Io8g",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3770.0514673416055,
			"y": 44.9049667044427,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 40.65601146478912,
			"height": 10.748126700771536,
			"seed": 319720208,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					1.4019314298202517
				],
				[
					0.4672819542392972,
					2.3365381218497987
				],
				[
					1.8692133840595488,
					4.205794289460755
				],
				[
					2.803862859640958,
					5.607725719281007
				],
				[
					4.673076243700052,
					7.009657149101486
				],
				[
					7.009657149101713,
					8.411588578921737
				],
				[
					8.878870533160807,
					9.346195270951284
				],
				[
					10.74816948432408,
					9.813520008741989
				],
				[
					13.084664822622017,
					10.280844746532694
				],
				[
					14.953963773784835,
					10.748126700771536
				],
				[
					16.82317715784393,
					10.748126700771536
				],
				[
					18.22510858766418,
					10.748126700771536
				],
				[
					20.561689493066297,
					10.748126700771536
				],
				[
					22.43090287712539,
					10.748126700771536
				],
				[
					24.300116261184485,
					10.280844746532694
				],
				[
					26.636697166586146,
					9.813520008741989
				],
				[
					29.44056002622665,
					8.878913316712442
				],
				[
					32.24442288586761,
					8.411588578921737
				],
				[
					35.04828574550811,
					7.944263841131033
				],
				[
					37.38486665090977,
					7.47698188689219
				],
				[
					39.254080034968865,
					7.47698188689219
				],
				[
					40.65601146478912,
					7.47698188689219
				],
				[
					40.65601146478912,
					7.47698188689219
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 312,
			"versionNonce": 654061552,
			"isDeleted": false,
			"id": "qB6clSQEcDHhhUoSa6Ab2",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3769.5841853873653,
			"y": -58.837959102260925,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 135.98734869257032,
			"height": 90.19093624629068,
			"seed": 355117328,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.934649475581864,
					0
				],
				[
					-1.8692989511632732,
					0
				],
				[
					-3.271230380983525,
					-0.467324737790932
				],
				[
					-3.7385123352223673,
					-0.467324737790932
				],
				[
					-5.140443765042619,
					-0.934606692029547
				],
				[
					-6.542375194862871,
					-0.934606692029547
				],
				[
					-7.47702467044428,
					-1.4019314298202517
				],
				[
					-9.346238054503374,
					-1.8692561676111836
				],
				[
					-11.215451438562923,
					-3.7384695516702777
				],
				[
					-13.552032343964584,
					-4.673119027251687
				],
				[
					-16.355895203605087,
					-6.075050457071939
				],
				[
					-18.692476109006748,
					-7.476981886892418
				],
				[
					-21.496338968647706,
					-9.346195270951512
				],
				[
					-23.3655523527068,
					-10.280844746532921
				],
				[
					-26.169415212347303,
					-11.215451438562468
				],
				[
					-28.038628596406397,
					-12.617382868382947
				],
				[
					-28.973278071987806,
					-13.084707606173652
				],
				[
					-30.8424914560469,
					-14.486639035993903
				],
				[
					-31.77714093162831,
					-15.42124572802345
				],
				[
					-32.711790407210174,
					-15.888570465814155
				],
				[
					-33.64635431568786,
					-17.290501895634634
				],
				[
					-34.113721837030425,
					-18.22510858766418
				],
				[
					-34.113721837030425,
					-19.159715279693728
				],
				[
					-35.04828574550811,
					-21.028971447304684
				],
				[
					-35.04828574550811,
					-21.96357813933423
				],
				[
					-35.51565326685068,
					-23.832834306945415
				],
				[
					-35.51565326685068,
					-26.169372428795214
				],
				[
					-35.98293522108952,
					-27.571303858615465
				],
				[
					-35.98293522108952,
					-29.44056002622665
				],
				[
					-35.98293522108952,
					-31.309816193837605
				],
				[
					-35.98293522108952,
					-32.711747623658084
				],
				[
					-35.98293522108952,
					-34.58096100771718
				],
				[
					-35.98293522108952,
					-35.98289243753743
				],
				[
					-35.98293522108952,
					-37.38482386735768
				],
				[
					-35.04828574550811,
					-38.78675529717793
				],
				[
					-34.58100379126927,
					-40.18868672699841
				],
				[
					-34.113721837030425,
					-41.590618156818664
				],
				[
					-32.711790407210174,
					-43.45987432442962
				],
				[
					-32.24442288586761,
					-44.8618057542501
				],
				[
					-30.375209501808058,
					-46.731061921861055
				],
				[
					-29.44056002622665,
					-47.6656686138906
				],
				[
					-27.571346642167555,
					-50.00220673574063
				],
				[
					-26.169415212347303,
					-51.871462903351585
				],
				[
					-24.30020182828821,
					-54.675325762992316
				],
				[
					-21.963620922886548,
					-57.011863884842114
				],
				[
					-20.094407538827,
					-59.348444790244
				],
				[
					-18.22510858766418,
					-61.2176581743031
				],
				[
					-15.421245728023678,
					-63.554239079704985
				],
				[
					-13.084750389725741,
					-65.89077720155478
				],
				[
					-10.280887530085238,
					-67.76003336916574
				],
				[
					-7.944306624683122,
					-69.1619647989861
				],
				[
					-5.140443765042619,
					-70.56389622880647
				],
				[
					-1.4019314298202517,
					-71.96582765862672
				],
				[
					1.869213384059094,
					-72.90043435065627
				],
				[
					5.14035819793844,
					-74.30236578047663
				],
				[
					7.944221057578943,
					-75.23697247250618
				],
				[
					11.68273339280131,
					-75.704297210297
				],
				[
					14.953878206680656,
					-76.1716219480877
				],
				[
					19.15967249614141,
					-77.10622864011725
				],
				[
					23.36546678560262,
					-77.10622864011725
				],
				[
					26.63669716658569,
					-77.57355337790796
				],
				[
					29.907841980465037,
					-78.0408353321468
				],
				[
					32.24442288586715,
					-78.5081600699375
				],
				[
					35.048285745507656,
					-78.5081600699375
				],
				[
					37.85214860514816,
					-78.5081600699375
				],
				[
					40.65601146478912,
					-78.5081600699375
				],
				[
					43.45987432442962,
					-78.5081600699375
				],
				[
					47.665668613890375,
					-77.57355337790796
				],
				[
					50.93681342776972,
					-76.63890390232655
				],
				[
					54.20795824164907,
					-75.704297210297
				],
				[
					58.413752531110276,
					-73.83504104268582
				],
				[
					63.55419629615244,
					-71.96582765862672
				],
				[
					68.69464006119506,
					-68.69464006119529
				],
				[
					72.90043435065581,
					-66.35810193934549
				],
				[
					77.57351059435587,
					-63.554239079704985
				],
				[
					81.31202292957778,
					-60.750376220064254
				],
				[
					84.58316774345712,
					-58.413795314662366
				],
				[
					87.38703060309808,
					-56.54458193060327
				],
				[
					89.72361150849974,
					-53.27339433317184
				],
				[
					91.59282489255884,
					-51.40413816556088
				],
				[
					93.46203827661793,
					-49.534924781501786
				],
				[
					94.3966877521998,
					-47.1983438760999
				],
				[
					95.33133722778075,
					-44.394481016459395
				],
				[
					96.26590113625844,
					-42.5252676324003
				],
				[
					97.2005506118403,
					-40.18868672699841
				],
				[
					97.66783256607914,
					-37.38482386735768
				],
				[
					98.60248204166055,
					-35.04828574550788
				],
				[
					99.0697639958994,
					-32.24442288586715
				],
				[
					99.53713151724196,
					-29.44056002622665
				],
				[
					99.53713151724196,
					-27.104021904376623
				],
				[
					100.0044134714808,
					-25.234765736765667
				],
				[
					100.0044134714808,
					-23.36550956915471
				],
				[
					100.0044134714808,
					-21.496296185095616
				],
				[
					100.0044134714808,
					-19.627040017484433
				],
				[
					100.0044134714808,
					-18.22510858766418
				],
				[
					99.53713151724196,
					-16.82317715784393
				],
				[
					99.0697639958994,
					-15.42124572802345
				],
				[
					98.13520008742171,
					-13.084707606173652
				],
				[
					97.66783256607914,
					-12.617382868382947
				],
				[
					96.26590113625844,
					-10.748126700771763
				],
				[
					95.79861918202005,
					-9.346195270951512
				],
				[
					94.86396970643818,
					-7.94426384113126
				],
				[
					93.46203827661793,
					-7.009657149101713
				],
				[
					92.99475632237909,
					-5.607725719281234
				],
				[
					92.06010684679768,
					-4.673119027251687
				],
				[
					91.12554293832,
					-3.7384695516702777
				],
				[
					90.19089346273859,
					-2.8038628596407307
				],
				[
					89.25624398715718,
					-1.8692561676111836
				],
				[
					88.32168007867949,
					-1.4019314298202517
				],
				[
					87.38703060309808,
					-0.934606692029547
				],
				[
					85.51781721903899,
					0
				],
				[
					84.58316774345712,
					0.934606692029547
				],
				[
					82.71395435939849,
					1.4019314298202517
				],
				[
					81.31202292957778,
					1.8692561676109563
				],
				[
					79.44272397841496,
					2.3365381218497987
				],
				[
					78.50816006993728,
					3.2711875974314353
				],
				[
					76.63886111877446,
					3.7384695516700504
				],
				[
					75.23692968895375,
					4.205794289460755
				],
				[
					73.8349982591335,
					5.140400981490529
				],
				[
					73.36771630489511,
					5.140400981490529
				],
				[
					72.43306682931325,
					5.607725719281234
				],
				[
					71.49850292083556,
					6.542332411310781
				],
				[
					71.031135399493,
					6.542332411310781
				],
				[
					70.09657149101531,
					6.542332411310781
				],
				[
					69.1619220154339,
					7.009657149101486
				],
				[
					68.22727253985249,
					7.009657149101486
				],
				[
					66.82534111003224,
					7.47698188689219
				],
				[
					65.89077720155456,
					7.47698188689219
				],
				[
					64.4888457717343,
					7.47698188689219
				],
				[
					63.08691434191405,
					7.944263841131033
				],
				[
					62.15226486633219,
					7.944263841131033
				],
				[
					60.75033343651194,
					8.411588578921737
				],
				[
					59.348402006691686,
					8.411588578921737
				],
				[
					57.946470576871434,
					8.411588578921737
				],
				[
					57.011821101290025,
					8.878913316712442
				],
				[
					55.60988967146977,
					8.878913316712442
				],
				[
					54.67532576299209,
					9.346195270951284
				],
				[
					53.27339433317184,
					9.346195270951284
				],
				[
					51.87146290335113,
					9.813520008742216
				],
				[
					50.93681342776972,
					10.280844746532921
				],
				[
					49.06760004371063,
					10.748126700771763
				],
				[
					47.19830109254781,
					10.748126700771763
				],
				[
					46.26373718407012,
					11.215451438562468
				],
				[
					44.394438232907305,
					11.215451438562468
				],
				[
					43.45987432442962,
					11.682776176353173
				],
				[
					42.525224848847756,
					11.682776176353173
				],
				[
					42.525224848847756,
					11.682776176353173
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 324,
			"versionNonce": 701542896,
			"isDeleted": false,
			"id": "4U-_2SV6twqTx1HLlHfv3",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3746.21863303466,
			"y": -64.44568482154284,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 213.56094485403037,
			"height": 29.44056002622642,
			"seed": 2048067344,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.9346494755814092,
					0
				],
				[
					-1.4019314298202517,
					0
				],
				[
					-2.336580905401661,
					0
				],
				[
					-3.2711448138793457,
					0
				],
				[
					-4.673076243699597,
					0
				],
				[
					-5.140443765042164,
					0
				],
				[
					-6.075007673519849,
					0
				],
				[
					-7.476939103340101,
					0
				],
				[
					-8.41158857892151,
					0
				],
				[
					-9.813520008742216,
					0
				],
				[
					-10.748169484323626,
					0
				],
				[
					-12.150100914143877,
					0
				],
				[
					-14.019314298202971,
					0
				],
				[
					-16.355895203604632,
					0
				],
				[
					-18.22510858766418,
					0
				],
				[
					-20.09432197172282,
					0
				],
				[
					-21.963620922886093,
					0.4673247377907046
				],
				[
					-24.30011626118403,
					0.934606692029547
				],
				[
					-25.70204769100428,
					1.8692561676109563
				],
				[
					-28.038628596405943,
					2.3365381218497987
				],
				[
					-30.375209501808058,
					3.7384695516700504
				],
				[
					-32.711704840105995,
					4.673119027251687
				],
				[
					-34.58100379126881,
					5.607725719281234
				],
				[
					-36.91749912956675,
					6.542332411310781
				],
				[
					-38.78679808072957,
					7.944263841131033
				],
				[
					-39.72136198920725,
					8.411588578921737
				],
				[
					-40.65601146478912,
					8.87891331671267
				],
				[
					-41.590660940370526,
					9.346195270951284
				],
				[
					-42.05794289460937,
					9.346195270951284
				],
				[
					-42.52522484884821,
					10.280844746532921
				],
				[
					-42.99259237019078,
					10.748126700771763
				],
				[
					-42.99259237019078,
					11.215451438562468
				],
				[
					-42.52522484884821,
					12.150058130592015
				],
				[
					-40.65601146478912,
					12.61738286838272
				],
				[
					-39.72136198920725,
					13.084707606173424
				],
				[
					-38.319430559387,
					13.551989560412267
				],
				[
					-36.91749912956675,
					13.551989560412267
				],
				[
					-35.5155676997465,
					14.019314298202971
				],
				[
					-33.646354315687404,
					14.486639035993676
				],
				[
					-31.77714093162831,
					14.486639035993676
				],
				[
					-30.8424914560469,
					15.42124572802345
				],
				[
					-28.973278071987806,
					15.42124572802345
				],
				[
					-27.571346642167555,
					15.888570465814155
				],
				[
					-25.23476573676544,
					16.355852420052997
				],
				[
					-22.89818483136378,
					16.355852420052997
				],
				[
					-20.09432197172282,
					16.355852420052997
				],
				[
					-17.290459112082317,
					16.823177157843702
				],
				[
					-13.552032343964129,
					17.75778384987325
				],
				[
					-9.346238054503374,
					18.692433325454658
				],
				[
					-4.205794289460755,
					19.627040017484205
				],
				[
					0.46728195423884245,
					20.094364755275137
				],
				[
					6.542375194862871,
					21.028971447304684
				],
				[
					13.084664822621562,
					22.430902877124936
				],
				[
					19.15975806324559,
					23.365509569154483
				],
				[
					25.234765736765894,
					23.832834306945188
				],
				[
					31.77714093162831,
					24.767440998974735
				],
				[
					36.917499129567204,
					25.234765736765667
				],
				[
					42.99259237019123,
					25.70209047455637
				],
				[
					48.13295056812967,
					26.169372428794986
				],
				[
					53.74067628741068,
					26.169372428794986
				],
				[
					58.8811200524533,
					26.63669716658592
				],
				[
					64.02156381749592,
					27.104021904376623
				],
				[
					68.69464006119551,
					27.104021904376623
				],
				[
					72.90043435065627,
					27.104021904376623
				],
				[
					77.57351059435587,
					27.571303858615465
				],
				[
					82.71395435939849,
					28.03862859640617
				],
				[
					85.51781721903899,
					28.03862859640617
				],
				[
					91.12554293832045,
					28.03862859640617
				],
				[
					94.86405527354236,
					28.03862859640617
				],
				[
					98.60248204166055,
					28.03862859640617
				],
				[
					103.74292580670317,
					28.505953334196874
				],
				[
					107.01407062058252,
					28.505953334196874
				],
				[
					111.21986491004373,
					28.505953334196874
				],
				[
					115.42565919950448,
					28.505953334196874
				],
				[
					119.16417153472685,
					28.505953334196874
				],
				[
					122.4353163486062,
					28.505953334196874
				],
				[
					125.70654672958926,
					28.973235288435717
				],
				[
					128.51040958923022,
					28.973235288435717
				],
				[
					131.31427244887072,
					28.973235288435717
				],
				[
					134.11813530851123,
					28.973235288435717
				],
				[
					136.45463064680916,
					28.973235288435717
				],
				[
					138.79121155221128,
					29.44056002622642
				],
				[
					141.59507441185178,
					29.44056002622642
				],
				[
					144.3989372714923,
					29.44056002622642
				],
				[
					147.2028001311328,
					29.44056002622642
				],
				[
					149.5393810365349,
					29.44056002622642
				],
				[
					152.3432438961754,
					29.44056002622642
				],
				[
					154.2124572802345,
					29.44056002622642
				],
				[
					155.61438871005475,
					29.44056002622642
				],
				[
					157.48360209411385,
					29.44056002622642
				],
				[
					158.8855335239341,
					29.44056002622642
				],
				[
					159.82018299951596,
					29.44056002622642
				],
				[
					161.22211442933622,
					28.973235288435717
				],
				[
					162.62404585915647,
					28.505953334196874
				],
				[
					163.55869533473788,
					28.03862859640617
				],
				[
					165.42790871879697,
					27.571303858615465
				],
				[
					165.8951906730358,
					27.571303858615465
				],
				[
					167.7644896241991,
					27.104021904376623
				],
				[
					168.69905353267632,
					27.104021904376623
				],
				[
					169.16642105401934,
					26.169372428794986
				],
				[
					169.63370300825773,
					26.169372428794986
				],
				[
					170.10098496249702,
					25.70209047455637
				],
				[
					170.5683524838396,
					25.70209047455637
				],
				[
					170.5683524838396,
					24.767440998974735
				],
				[
					170.5683524838396,
					24.300159044735892
				],
				[
					170.5683524838396,
					22.89822761491564
				],
				[
					170.5683524838396,
					22.430902877124936
				],
				[
					170.10098496249702,
					21.96357813933423
				],
				[
					169.63370300825773,
					21.028971447304684
				],
				[
					169.16642105401934,
					20.56164670951398
				],
				[
					168.23177157843747,
					20.094364755275137
				],
				[
					167.7644896241991,
					19.627040017484205
				],
				[
					166.82984014861722,
					19.627040017484205
				],
				[
					165.8951906730358,
					19.1597152796935
				],
				[
					164.96062676455813,
					18.692433325454658
				],
				[
					164.02597728897672,
					18.225108587663954
				],
				[
					163.09132781339486,
					17.75778384987325
				],
				[
					162.15676390491717,
					17.290501895634407
				],
				[
					161.22211442933622,
					16.823177157843702
				],
				[
					160.28746495375435,
					16.823177157843702
				],
				[
					159.35290104527667,
					16.355852420052997
				],
				[
					158.4182515696957,
					15.888570465814155
				],
				[
					157.016320139875,
					15.42124572802345
				],
				[
					156.0816706642936,
					14.953920990232518
				],
				[
					154.67973923447335,
					14.486639035993676
				],
				[
					153.2778078046531,
					14.019314298202971
				],
				[
					152.3432438961754,
					14.019314298202971
				],
				[
					151.87587637483284,
					14.019314298202971
				],
				[
					150.4739449450126,
					13.551989560412267
				],
				[
					150.0066629907733,
					13.551989560412267
				],
				[
					149.07201351519188,
					13.084707606173424
				],
				[
					148.13744960671465,
					13.084707606173424
				],
				[
					147.2028001311328,
					13.084707606173424
				],
				[
					145.80086870131254,
					13.084707606173424
				],
				[
					145.3335867470737,
					12.61738286838272
				],
				[
					144.3989372714923,
					12.61738286838272
				],
				[
					143.46428779591088,
					12.150058130592015
				],
				[
					142.5297238874332,
					12.150058130592015
				],
				[
					142.06235636609017,
					11.682776176353173
				],
				[
					140.66042493626992,
					11.682776176353173
				],
				[
					139.72586102779223,
					11.215451438562468
				],
				[
					139.25849350644967,
					11.215451438562468
				],
				[
					138.32392959797198,
					11.215451438562468
				],
				[
					137.38928012239057,
					11.215451438562468
				],
				[
					136.92199816815173,
					10.748126700771763
				],
				[
					135.0526992169889,
					10.748126700771763
				],
				[
					133.65076778716866,
					10.748126700771763
				],
				[
					132.2488363573484,
					10.748126700771763
				],
				[
					130.37962297328886,
					10.748126700771763
				],
				[
					128.9776915434686,
					10.280844746532921
				],
				[
					127.10847815940997,
					10.280844746532921
				],
				[
					126.1738286838281,
					10.280844746532921
				],
				[
					125.2391792082467,
					9.813520008741989
				],
				[
					124.77189725400785,
					9.813520008741989
				],
				[
					124.30461529976901,
					9.346195270951284
				],
				[
					123.83724777842644,
					9.346195270951284
				],
				[
					123.83724777842644,
					8.87891331671267
				],
				[
					123.3699658241876,
					8.87891331671267
				],
				[
					123.3699658241876,
					8.87891331671267
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 183,
			"versionNonce": 583332848,
			"isDeleted": false,
			"id": "GR7XdRk-slEol7Z5xHLr4",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3702.026685436729,
			"y": -60.43166240278072,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 49.173007011364234,
			"height": 37.21195433456569,
			"seed": 507487504,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.6644589888355767,
					0.6644589888355767
				],
				[
					-1.3290396511724794,
					0.6644589888355767
				],
				[
					-1.993498640008056,
					2.657957628843633
				],
				[
					-3.986997280016112,
					3.986997280015885
				],
				[
					-6.644954908859745,
					7.309474734445757
				],
				[
					-10.631952188875857,
					10.631952188875402
				],
				[
					-14.618949468891515,
					14.618949468891515
				],
				[
					-18.605946748907627,
					18.605946748907627
				],
				[
					-23.921983680095764,
					21.928485040087708
				],
				[
					-29.238020611284355,
					25.91548232010382
				],
				[
					-33.889476880136044,
					29.237959774533692
				],
				[
					-39.205513811324636,
					31.89597824012776
				],
				[
					-43.19251109134029,
					33.88947688013582
				],
				[
					-45.850468720183926,
					35.21845569455763
				],
				[
					-47.84396736019198,
					36.54743450897945
				],
				[
					-48.508426349027786,
					37.21195433456569
				],
				[
					-49.173007011364234,
					37.21195433456569
				],
				[
					-49.173007011364234,
					37.21195433456569
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 180,
			"versionNonce": 937489904,
			"isDeleted": false,
			"id": "pnCN7JvnEq4B9N0AE6Q-i",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3919.9824961864356,
			"y": -45.8127129338892,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 39.205513811324636,
			"height": 31.895978240127988,
			"seed": 254313232,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.6645198255860123
				],
				[
					1.3290396511724794,
					3.322538291180308
				],
				[
					3.986997280016112,
					6.645015745610181
				],
				[
					7.973994560032224,
					10.632013025626293
				],
				[
					12.625572502384784,
					15.283530131228417
				],
				[
					17.94148776007205,
					18.606007585658062
				],
				[
					21.928485040088162,
					21.928485040087935
				],
				[
					25.915482320104275,
					23.92198368009599
				],
				[
					29.902479600120387,
					27.2445219712763
				],
				[
					33.889476880136044,
					29.238020611284355
				],
				[
					36.54755618248055,
					30.566999425705944
				],
				[
					37.876474160152156,
					31.23151925129241
				],
				[
					38.541054822488604,
					31.895978240127988
				],
				[
					39.205513811324636,
					31.895978240127988
				],
				[
					39.205513811324636,
					31.895978240127988
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 183,
			"versionNonce": 237811696,
			"isDeleted": false,
			"id": "f9s_KogHREGl6Zkh7edGJ",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3961.1815086377683,
			"y": -15.910233333769952,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.65157794235256,
			"height": 101.66843064040768,
			"seed": 1799725328,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.6644589888355767,
					6.645015745610181
				],
				[
					-0.6644589888355767,
					7.309535571196193
				],
				[
					-0.6644589888355767,
					10.632013025626293
				],
				[
					-1.3290396511720246,
					15.283530131228417
				],
				[
					-1.9934986400076014,
					21.928485040087935
				],
				[
					-2.657957628843633,
					28.573500785698116
				],
				[
					-3.3225382911800807,
					37.212015171316125
				],
				[
					-3.3225382911800807,
					47.17950837135618
				],
				[
					-3.3225382911800807,
					57.81146056023181
				],
				[
					-3.3225382911800807,
					68.4434735858581
				],
				[
					-3.3225382911800807,
					79.07548661148417
				],
				[
					-2.657957628843633,
					87.04948117151616
				],
				[
					-1.9934986400076014,
					93.0299770915401
				],
				[
					0,
					97.01697437155599
				],
				[
					0.6644589888355767,
					100.33945182598609
				],
				[
					1.3290396511724794,
					101.0039716515721
				],
				[
					1.3290396511724794,
					101.66843064040768
				],
				[
					1.3290396511724794,
					101.66843064040768
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 228,
			"versionNonce": 1773156848,
			"isDeleted": false,
			"id": "I1KojNYP2kBKz_p4OK8Sy",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3652.8536784253643,
			"y": -25.21320670822331,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 330.9207742413273,
			"height": 114.9584012948776,
			"seed": 1108279056,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					0,
					0.6645198255860123
				],
				[
					0,
					1.993498640008056
				],
				[
					0,
					5.315976094437701
				],
				[
					0,
					10.632013025626293
				],
				[
					-0.6644589888358041,
					17.27696793448581
				],
				[
					-1.3289179776713809,
					27.908980960111876
				],
				[
					-1.3289179776713809,
					38.54099398573817
				],
				[
					-1.3289179776713809,
					49.17294617461357
				],
				[
					-1.3289179776713809,
					57.146940734645796
				],
				[
					-1.3289179776713809,
					64.45647630584199
				],
				[
					-1.3289179776713809,
					69.77245240027969
				],
				[
					-1.3289179776713809,
					73.7594496802958
				],
				[
					-1.3289179776713809,
					76.41746814588987
				],
				[
					-1.3289179776713809,
					77.08192713472567
				],
				[
					-1.3289179776713809,
					78.41096678589793
				],
				[
					-1.3289179776713809,
					79.0754257747335
				],
				[
					-1.3289179776713809,
					79.73994560031997
				],
				[
					-1.3289179776713809,
					80.40446542590598
				],
				[
					-1.3289179776713809,
					81.06892441474156
				],
				[
					-1.3289179776713809,
					81.7334442403278
				],
				[
					-1.3289179776713809,
					83.06242305474962
				],
				[
					-1.3289179776713809,
					84.3914627059221
				],
				[
					-1.3289179776713809,
					85.05592169475767
				],
				[
					-1.3289179776713809,
					85.72044152034368
				],
				[
					-1.993498640008056,
					85.72044152034368
				],
				[
					-2.65795762884386,
					85.72044152034368
				],
				[
					-2.65795762884386,
					86.38496134592992
				],
				[
					-1.3289179776713809,
					86.38496134592992
				],
				[
					1.329039651172252,
					87.71394016035174
				],
				[
					3.322538291180308,
					88.37845998593798
				],
				[
					5.980495920023941,
					89.04291897477378
				],
				[
					9.967493200039598,
					89.7074388003598
				],
				[
					14.619071142392613,
					90.37195862594581
				],
				[
					18.60606842240827,
					91.70093744036785
				],
				[
					23.921983680095536,
					92.36545726595386
				],
				[
					31.89597824012776,
					93.69443608037591
				],
				[
					39.869972800159985,
					95.0234148947975
				],
				[
					53.160004291380346,
					96.35245454596998
				],
				[
					67.11449477143628,
					97.6814333603918
				],
				[
					87.04948117151594,
					99.67493200039962
				],
				[
					106.98446757159604,
					102.33295046599392
				],
				[
					130.9064512516918,
					103.66192928041573
				],
				[
					153.49939528061554,
					105.65542792042379
				],
				[
					181.40837624072742,
					106.9844067348456
				],
				[
					208.65289821200372,
					108.31344638601786
				],
				[
					231.9104229032639,
					110.30694502602591
				],
				[
					251.845409303344,
					112.30044366603397
				],
				[
					267.1288177610711,
					113.62942248045579
				],
				[
					277.09631096111093,
					114.9584012948776
				],
				[
					283.07680688113555,
					114.9584012948776
				],
				[
					286.39934517231563,
					114.9584012948776
				],
				[
					289.7218834634957,
					114.9584012948776
				],
				[
					291.71538210350377,
					114.9584012948776
				],
				[
					295.7023793835199,
					114.9584012948776
				],
				[
					299.68937666353554,
					114.9584012948776
				],
				[
					305.00529192122326,
					114.9584012948776
				],
				[
					310.98578784124743,
					114.9584012948776
				],
				[
					316.30182477243557,
					114.9584012948776
				],
				[
					320.95328104128725,
					114.9584012948776
				],
				[
					325.6048589836398,
					114.9584012948776
				],
				[
					327.59835762364787,
					114.9584012948776
				],
				[
					328.26281661248345,
					114.9584012948776
				],
				[
					328.26281661248345,
					114.9584012948776
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 179,
			"versionNonce": 1299414000,
			"isDeleted": false,
			"id": "e_oB-ig2uJq-OJwvwFxuS",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3959.1880099977598,
			"y": 77.78420274660664,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 17.94148776007205,
			"height": 9.967493200040053,
			"seed": 1945935120,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.9934986400085108,
					-1.3289788144220438
				],
				[
					-3.986997280016112,
					-3.3224774544301
				],
				[
					-5.980495920024168,
					-3.986997280016112
				],
				[
					-7.973994560032224,
					-5.315976094437929
				],
				[
					-9.303034211204249,
					-6.644954908859745
				],
				[
					-11.29653285121276,
					-7.309474734445985
				],
				[
					-11.960991840048337,
					-8.638453548867801
				],
				[
					-13.954490480055938,
					-8.638453548867801
				],
				[
					-14.61894946889197,
					-9.302973374453813
				],
				[
					-15.947989120064449,
					-9.302973374453813
				],
				[
					-16.612448108900026,
					-9.967493200040053
				],
				[
					-17.277028771236473,
					-9.967493200040053
				],
				[
					-17.94148776007205,
					-9.967493200040053
				],
				[
					-17.94148776007205,
					-9.967493200040053
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 180,
			"versionNonce": 461274608,
			"isDeleted": false,
			"id": "Mhv7zC7hiMINwq4WzX6tH",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3919.9824961864365,
			"y": 62.500733452127974,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 29.23789893778303,
			"height": 5.980495920023941,
			"seed": 310803216,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.657957628843178,
					0
				],
				[
					-3.986997280016112,
					-0.6645198255860123
				],
				[
					-5.9804959200237136,
					-1.3289788144218164
				],
				[
					-7.97399456003177,
					-1.3289788144218164
				],
				[
					-8.638453548867801,
					-1.3289788144218164
				],
				[
					-10.631952188875402,
					-1.993498640008056
				],
				[
					-11.960991840047882,
					-2.6580184655940684
				],
				[
					-13.28990981771949,
					-2.6580184655940684
				],
				[
					-15.283408457727091,
					-3.322477454429645
				],
				[
					-17.276907097735148,
					-3.986997280015885
				],
				[
					-19.270405737743204,
					-3.986997280015885
				],
				[
					-22.59294402892374,
					-4.6515171056021245
				],
				[
					-25.91548232010382,
					-5.315976094437701
				],
				[
					-29.23789893778303,
					-5.980495920023941
				],
				[
					-29.23789893778303,
					-5.980495920023941
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 180,
			"versionNonce": 886652912,
			"isDeleted": false,
			"id": "5Uv1GG4sIiGwBjUE2b5oP",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3875.461067117424,
			"y": 50.539741612080775,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.618949468891515,
			"height": 3.986997280016112,
			"seed": 1076140304,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.3290396511724794,
					-0.6645198255862397
				],
				[
					-2.657957628843633,
					-0.6645198255862397
				],
				[
					-3.3225382911800807,
					-1.3289788144218164
				],
				[
					-4.651456268851689,
					-1.993498640008056
				],
				[
					-5.3160369311885916,
					-1.993498640008056
				],
				[
					-5.980495920024168,
					-2.6580184655940684
				],
				[
					-7.309535571196193,
					-3.3224774544298725
				],
				[
					-7.97399456003177,
					-3.3224774544298725
				],
				[
					-8.638453548867346,
					-3.3224774544298725
				],
				[
					-9.96749320004028,
					-3.3224774544298725
				],
				[
					-11.296532851212305,
					-3.3224774544298725
				],
				[
					-11.960991840047882,
					-3.3224774544298725
				],
				[
					-13.954490480055938,
					-3.986997280016112
				],
				[
					-14.618949468891515,
					-3.986997280016112
				],
				[
					-14.618949468891515,
					-3.986997280016112
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 177,
			"versionNonce": 428589552,
			"isDeleted": false,
			"id": "n9jPOU3vSFFMIBu2X0Qxg",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3751.199692448093,
			"y": 33.262773677594964,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.290031491219906,
			"height": 2.657957628843633,
			"seed": 273610512,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.3290396511724794,
					0.6644589888358041
				],
				[
					-1.993498640008056,
					0.6644589888358041
				],
				[
					-3.3225382911800807,
					1.3289788144218164
				],
				[
					-4.65157794235256,
					1.3289788144218164
				],
				[
					-5.980495920024168,
					1.9934986400078287
				],
				[
					-7.309535571196193,
					2.657957628843633
				],
				[
					-7.97399456003177,
					2.657957628843633
				],
				[
					-9.303034211204249,
					2.657957628843633
				],
				[
					-9.967493200039826,
					2.657957628843633
				],
				[
					-11.960991840047882,
					2.657957628843633
				],
				[
					-13.290031491219906,
					2.657957628843633
				],
				[
					-13.290031491219906,
					2.657957628843633
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 179,
			"versionNonce": 144573424,
			"isDeleted": false,
			"id": "3Qu_kGNV5Yd3jhXTCLPYk",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3694.717149865533,
			"y": 37.24977095761062,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 21.928485040087708,
			"height": 3.3224774544298725,
			"seed": 1736283408,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-0.6644589888355767,
					0
				],
				[
					-1.9934986400076014,
					0
				],
				[
					-2.657957628843178,
					0
				],
				[
					-3.986997280016112,
					0
				],
				[
					-5.9804959200237136,
					0
				],
				[
					-7.97399456003177,
					0
				],
				[
					-9.302912537703378,
					0.6644589888358041
				],
				[
					-11.960991840047427,
					0.6644589888358041
				],
				[
					-13.954490480055938,
					1.993498640008056
				],
				[
					-15.94798912006354,
					1.993498640008056
				],
				[
					-18.605946748907627,
					1.993498640008056
				],
				[
					-20.59944538891523,
					2.657957628843633
				],
				[
					-21.928485040087708,
					3.3224774544298725
				],
				[
					-21.928485040087708,
					3.3224774544298725
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": true,
			"pressures": []
		},
		{
			"type": "freedraw",
			"version": 176,
			"versionNonce": 538445296,
			"isDeleted": false,
			"id": "v54-v0GtCFRoYZjAYmA0P",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 3653.5182590877002,
			"y": 49.21076279765987,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.316036931188137,
			"height": 4.651456268851462,
			"seed": 1529377552,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.329039651172252,
					0.6644589888355767
				],
				[
					-1.329039651172252,
					1.3289788144218164
				],
				[
					-1.9934986400078287,
					1.3289788144218164
				],
				[
					-1.9934986400078287,
					1.9934986400078287
				],
				[
					-2.658079302344504,
					1.9934986400078287
				],
				[
					-2.658079302344504,
					2.657957628843633
				],
				[
					-3.986997280015885,
					3.3224774544298725
				],
				[
					-3.986997280015885,
					3.986997280015885
				],
				[
					-5.316036931188137,
					4.651456268851462
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
			"type": "text",
			"version": 392,
			"versionNonce": 2097268720,
			"isDeleted": false,
			"id": "zPXtDgqV",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5222.740257873133,
			"y": -1857.1661637563338,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 278.90625,
			"height": 33.6,
			"seed": 298291472,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"fontSize": 28,
			"fontFamily": 3,
			"text": "Micro-controllers",
			"rawText": "Micro-controllers",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Micro-controllers",
			"lineHeight": 1.2,
			"baseline": 27
		},
		{
			"type": "image",
			"version": 327,
			"versionNonce": 1533233648,
			"isDeleted": false,
			"id": "SkKo4nw1ilu_D4Y8h-0Id",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5222.740257636804,
			"y": -1724.6081373832876,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"width": 1440,
			"height": 308,
			"seed": 584249104,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"status": "saved",
			"fileId": "101a012f112bb18a111fd006f1f71ca3c312a903",
			"scale": [
				1,
				1
			]
		},
		{
			"type": "text",
			"version": 98,
			"versionNonce": 910461936,
			"isDeleted": false,
			"id": "BSU3MdP8",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "dashed",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 5043.104627699953,
			"y": -1613.1545236075249,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 147.65625,
			"height": 777.5999999999999,
			"seed": 1992461584,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1714260690851,
			"link": null,
			"locked": false,
			"fontSize": 36,
			"fontFamily": 3,
			"text": "Jai\n\n\n\n\n\n\n\nBradley\n\n\n\n\n\n\n\n\nRowan",
			"rawText": "Jai\n\n\n\n\n\n\n\nBradley\n\n\n\n\n\n\n\n\nRowan",
			"textAlign": "center",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Jai\n\n\n\n\n\n\n\nBradley\n\n\n\n\n\n\n\n\nRowan",
			"lineHeight": 1.2,
			"baseline": 769
		}
	],
	"appState": {
		"theme": "dark",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#2f9e44",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "cross-hatch",
		"currentItemStrokeWidth": 4,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 0,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 2,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 186.55215445226952,
		"scrollY": 2124.378907431311,
		"zoom": {
			"value": 0.30000000000000004
		},
		"currentItemRoundness": "round",
		"gridSize": null,
		"gridColor": {
			"Bold": "#C9C9C9FF",
			"Regular": "#EDEDEDFF"
		},
		"currentStrokeOptions": null,
		"previousGridSize": null,
		"frameRendering": {
			"enabled": true,
			"clip": true,
			"name": true,
			"outline": true
		}
	},
	"files": {}
}
```
%%