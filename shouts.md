![GGS.SX Logo](https://ggs.sx/images/final-small.png)
# Shouts Query

Get the details of the requested verified User from the GGS API.

**URL** : `/api/v1/shouts`

**Method** : `GET`

**Auth required** : NO

**Permissions required** : None

## Success Response

**Code** : `200 OK`

**Content examples**

When a request goes through these are all the datapoints in the object that it provides.

```json
[
    {
      "id": "integer",
      "content": "string",
      "hide": "integer",
      "created_by": "string",
      "updated_by": "string",
      "created_at": "string",
      "updated_at": "string",
      "author": {
        "steam_64": "string",
        "nickname": "string",
        "avatar": "string",
        "steam_profile_url": "string",
        "discord_profile_url": "string",
        "is_author": "boolean",
        "bio_html": "string",
        "signature_html": "string",
        "steam_32": "string",
        "group": {
          "id": "integer",
          "name": "string",
          "guard_name": "string",
          "special": "integer",
          "priority": "integer",
          "features": "json",
          "description": "string",
          "max_cost": "integer",
          "min_cost": "integer",
          "color_primary": "string",
          "color_secondary": "string",
          "created_by": "string",
          "updated_by": "string",
          "created_at": "string",
          "updated_at": "string",
          "laravel_through_key": "integer"
        },
        "current_ban": "json"
      }
    }
  ]
```

## Notes

* If the User Has Not Verified Through The Website The Query Will Fail.
