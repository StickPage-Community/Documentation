# JSON Schema: StickPage Entry

## Before you dive in

* Every StickPage entry must contain data from the [StickPage Wiki](https://stickpage.fandom.com).
* Please take a look at this page on how to read the JSON schema docs.

## `characterName`

**Type**: String

**Description**: The name of a stick character registered on the wiki.

## `characterPhoto`

**Type**: String

**Description**: An valid URL to the photo of a stick character.

## `characterMeta`

**Type**: JSON Object

**Description**: This object holds important metadata about a character, such as `animator` and `powersAndAbilities`.

### `powersAndAbilities`

**Type**: JSON Object

**Description**: This object holds metadata about the character's weapons, strengths, and weaknesses.

#### `weapons`

**Type**: JSON Array

**Description**: Array of strings containing the weapons a character uses.

#### `strength`

**Type**: JSON Array

**Description**:

#### `weaknesses`

**Type**: JSON Array

**Description**:

### `creator`

**Type**: JSON Object

Description:

## `battles`

**Type**: JSON Object

**Description**:

{% code title="examples/stickpage-templates/battles.json" %}
```javascript
{
   "opponent": "Name Here",
   "result": "WIN|LOSE|DRAW",
   "reference": "https://domain.tld/path/to/ref"
}
```
{% endcode %}

## A complete example

Here's the full example on how a new StickPage entry should be like.

{% code title="templates/stickpage.json" %}
```javascript
{
    "characterName": "Insert name here",
    "characterPhoto": "https://link.to/the/photo/of/the-character.png",
    "generalInfo": {
        "gender": "male|female|other",
        "status": "active|inactive|retired",
        "color": "hex format or description"
    },
    "characterMeta": {
        "powersAndAbilities": {
            "weapons": [
                "stuff1",
                "stuff2"
            ],
            "strength": [
                "stuff1",
                "stuff2"
            ],
            "weaknesses": [
                "stuff1",
                "stuff2"
            ]
        },
        "animator": {
            "name": "Name here, either real name or screen name",
            "yt": "https://youtube.com/channel/id or https://youtube.com/user/usernameGoesHere",
            "twitch": "https://twitch.tv/stuffHere",
            "twitter": "https://twitter.com/username",
            "stickpageForum": "",
            "hyunsDojoForum": ""
        },
        "clan": "clan-name-here-REEEEEEEEEEEEEEEEEEEEEE"
    },
    "battles": [
        {
            "opponent": "name1",
            "result": "WIN",
            "reference": "https://youtu.be/ABCD1234EFG"
        },
        {
            "opponent": "name2",
            "result": "LOSE",
            "reference": "https://youtu.be/ABCD1234EFG"
        },
        {
            "opponent": "name3",
            "result": "DRAW",
            "reference": "https://youtu.be/ABCD1234EFG"
        }
    ]
}
```
{% endcode %}

