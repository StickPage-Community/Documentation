# JSON Schema: StickPage Entry

## Before you dive in

* Every StickPage entry must contain data from the [StickPage Wiki](https://stickpage.fandom.com).
* Please take a look at this page on how to read the JSON schema docs.

## `characterName`

**Type**: String

**Description**: The name of a stick character registered on the wiki.

## `characterPhoto`

**Type**: String

**Description**: An valid URL to the photo of an stick character.

## `characterMeta`

**Type**: JSON Object

**Description**: This object holds important metadata about a character, such as `animator` and `powersAndAbilities`.

### `powersAndAbilities`

**Type**: JSON Object

**Description**: This object holds metadata about character's weapons, strengths and weaknesses.

#### `weapons`

**Type**: JSON Array

**Description**: Array of strings containing the weapons a character uses.

#### `strength`

**Type**: JSON Array

**Description**:

#### `weaknesses`

**Type**: JSON Array

**Description**:

