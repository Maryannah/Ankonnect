## Ankonnect ⚡️

Don't waste your time connecting to Ankama APIs...

- [Description](#description)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Docs](./docs)

## Description

This small project is made to avoid to write time-consuming code about a non-consistent API.

Works on Window, Unix, OSX.

## Dependencies

None.
You just have to have `curl` installed on your system.

## Installation

Using npm:
`npm i --save ankonnect`

Using yarn:
`yarn add ankonnect`

## Usage

You have to construct the Ankonnect and use the SDK.

```javascript
import Ankonnect from "ankonnect";

const ankonnect = new Ankonnect();
const response = await ankonnect.Api.createApiKey({
  login: "myLogin",
  password: "*******",
  long_life_token: true
});
console.log(response.key);
```

To find all the APIs, check the [Docs](./docs)
