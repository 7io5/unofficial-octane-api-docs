# TCDN

## GET /{hash}

Host: tcdn.octane.wtf

Returns a 3D asset material file. Content type varies by asset.

Response (captured):

    newmtl Mrgrey1Mtl
    Material Color
    Ka 1 1 1
    Kd 1 1 1
    Ks 0.0627451 0.0627451 0.0627451 
    
    d 1
    
    Ns 0
    
    map_Ka a08f2c186d0a9a3481dc551efb235520
    map_Kd a08f2c186d0a9a3481dc551efb235520
    map_d a08f2c186d0a9a3481dc551efb235520

## GET /asset_{assetId}_{version}_thumbnail3d.json

Host: tcdn.octane.wtf

Query params: v.

Returns a 3D thumbnail manifest for an asset.

Response (captured):

    {
      "targetId": 410241,
      "camera": {
        "position": { "x": 2.0279, "y": 4.5279, "z": 3.59576 },
        "direction": { "x": 0.40558, "y": 0.40558, "z": 0.819152 },
        "fov": 70
      },
      "aabb": {
        "min": { "x": -2, "y": 0, "z": -1.09892 },
        "max": { "x": 2, "y": 5.10121, "z": 0.0989245 }
      },
      "mtl": "4fa5249fce5abdbc4af218b9f16b00d8",
      "obj": "575a2db01715084249b504a719d826df",
      "textures": ["a08f2c186d0a9a3481dc551efb235520"]
    }
