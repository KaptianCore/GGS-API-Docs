![GGS.SX Logo](https://ggs.sx/storage/images/svg/logo_white.svg)
# Discord ID Query

Get the details of the requested verified User from the GGS API.

**URL** : `/api/v2/user/discord/{discord_id}?api_token={token}`

**Method** : `GET`

**AUTH required** : YES

**Permissions required** : None

## Success Response

**Code** : `200 OK`

**Content examples**

When a request goes through these are all the datapoints in the object that it provides.

```json
{
  "steam_64": "string",
  "nickname": "Example",
  "intel_status": "string",
  "bio": "string",
  "signature": "string",
  "realname": "string",
  "avatar": "string",
  "steam_created_at": "string",
  "updated_by": "string",
  "meta": "json",
  "created_at": "string",
  "updated_at": "string",
  "discord_id": "integer",
  "timezone": "string",
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
    "created_by": "integer",
    "updated_by": "integer",
    "created_at": "string",
    "updated_at": "string",
    "laravel_through_key": "integer"
  },
  "groups": [
    {
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
      "created_by": "integer",
      "updated_by": "integer",
      "created_at": "string",
      "updated_at": "string",
      "pivot": "json"
    }
  ],
  "current_ban": "json",
  "character": {
    "steamID": "string",
    "character_id": "integer",
    "first_name": "string",
    "last_name": "string",
    "sex": "string",
    "model": "string",
    "model_override": "string",
    "model_bgroups": "json",
    "skin": "integer",
    "money_held": "integer",
    "money_bank": "integer",
    "vehicles": "array",
    "autobills": "json",
    "bank_items": "json",
    "bills":"json",
    "buddies":"json",
    "current_arrest":"json",
    "current_warrant": "string",
    "jailtime": "string",
    "jobtimes": "json",
    "last_drivingtest_time": "string",
    "license":"json",
    "limb_damage":"json",
    "lostandfound":"json",
    "needs": "json",
    "rapsheet":"json",
    "savedammo": "json",
    "skills": "json",
    "tickets":"json",
    "equipped_items": "array",
    "character_inventory": "json",
    "mailbox":"json",
    "created": "string",
    "total_time": "integer",
    "last_played": "string",
    "cop_level": "integer",
    "org": "integer",
    "disabled": "boolean",
    "wealth": "integer",
    "wealth_formatted": "string",
    "full_name": "string",
    "owned_organisation":"json",
    "organisation": {Object}
  }
  "bans": [
    {
      "id": "integer",
      "steam_64": "string",
      "reason": "string",
      "thread_id": "integer",
      "exiled": "boolean",
      "is_pending": "integer",
      "banned_at": "string",
      "unbanned_at": "string",
      "banned_by": {
        "steam_64": "string",
        "nickname": "string",
        "intel_status": "string",
        "bio": "string",
        "signature": "string",
        "realname": "string",
        "avatar": "string",
        "steam_created_at": null,
        "updated_by": "json",
        "meta": null,
        "created_at": "string",
        "updated_at": "string",
        "discord_id": "string",
        "timezone": "string",
        "steam_profile_url": "string",
        "discord_profile_url": "string",
        "is_author": "boolean",
        "steam_32": "string"
      },
    "unbanned_by": "json",
    "updated_by": "string",
    "created_at": "string",
    "updated_at": "string",
    "is_permanent": "boolean",
    "duration": "string",
    "duration_from_now": "string"
    },
}
```

## Notes

* If the User Has Not Verified Through The Website The Query Will Fail.
