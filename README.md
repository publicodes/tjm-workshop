# publicodes-tjm-simulator

A simulator for estimating the TJM in publicodes

## Installation

```sh
npm install publicodes-tjm-simulator publicodes
```

## Usage

```typescript
import { Engine } from 'publicodes'
import rules from 'publicodes-tjm-simulator'

const engine = new Engine(rules)

console.log(engine.evaluate('salaire net').nodeValue)
// 1957.5

engine.setSituation({ 'salaire brut': 4000 })
console.log(engine.evaluate('salaire net').nodeValue)
// 3120
```

## Development

```sh
// Install the dependencies
npm install

// Compile the Publicodes rules
npm run compile

// Run the tests
npm run test

// Run the documentation server
npm run doc
```
