![GGS.SX Logo](https://ggs.sx/images/final-small.png)
# Servers Query

Get the details of the requested verified User from the GGS API.

**URL** : `/api/v1/servers`

**Method** : `GET`

**Auth required** : NO

**Permissions required** : None

## Success Response

**Code** : `200 OK`

**Content examples**

When a request goes through these are all the datapoints in the object that it provides.

```json
{
  "servers": {
    "gmod.ggs.sx:27015": {
      "name": "string",
      "address": "string",
      "online": "boolean",
      "joinlink": "string",
      "hostname": "string",
      "mapname": "string",
      "numplayers": "integer",
      "maxplayers": "integer"
    },
    "mc.ggs.sx:25565": {
      "name": "string",
      "address": "string",
      "online": "boolean",
      "joinlink": "string",
      "hostname": "string",
      "mapname": "string",
      "numplayers": "integer",
      "maxplayers": "integer"
    },
    "discord.gg/ggs": {
      "name": "string",
      "address": "string",
      "online": "boolean",
      "joinlink": "string",
      "hostname": "string",
      "mapname": "string",
      "numplayers": "integer",
      "maxplayers": "integer"
    }
  },
  "updated_at": "string"
}

```

## Notes

* If the User Has Not Verified Through The Website The Query Will Fail.
