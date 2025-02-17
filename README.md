# Scratch-File-Research
A page dedicated to things I found out about https://scratch.mit.edu/

# project.json
The heart of the project. It contains sprites, variables, code blocks, and the stage.
## Targets
```json
  {
    "targets":[]
  }
```
Contains sprites, stage, with their code and information.

## Sprites
```json
  {
    "targets":[
      {
        "isStage":true,
        "name":"Stage",
        "variables":{},
        "lists":{},
        "broadcasts":{},
        "blocks":{},
        "comments":{},
        "currentCostume":0,
        "costumes":[{}],
        "sounds":[{}],
        "volume":100,
        "layerOrder":0,
        "tempo":60,
        "videoTransparency":50,
        "videoState":"on",
        "textToSpeechLanguage":null
      }
    ]
  }
```

The structure for a sprite.
### isStage
``` json
"isStage":true,
```

Determines if a sprite is the stage. Two sprites can not have this on naturally. It is garenteed that one sprite will have this tag on.
When false, this tag is not present.

### Blocks

![Screenshot 2025-02-11 10 43 50 AM](https://github.com/user-attachments/assets/040e6ece-b0ba-4a2d-a01f-8d40ca235e6f)

``` json
"blocks":{
  "B0wNcnplc18^o$.Zy$A": {
    "opcode": "control_forever",
    "next": null,
    "parent": null,
    "inputs": {
      "SUBSTACK": [2, "GCZl0vxW?`_$^.U3wm;"]
    },
    "fields": {

    },
    "shadow": false,
    "topLevel": true,
    "x": 154,
    "y": 261
  },
}
```

#### opcode
Usually structured like "category_blockname". 
Describes the block type.

#### next
Tells what the next block is.
Mainly used for blocks in nests, like forever.

#### parent
Tells what main block this is apart of.
Mainly used to determine 

#### inputs
At this time, I have not figured out this function.

#### feilds
At this time, I have not figured out this function.

#### shadow
At this time, I have not figured out this function.

#### toplevel
If the block is an orphan

#### x
X coordinate of the block in the code viewer.

#### y
Y coordinate of the block in the code viewer.
