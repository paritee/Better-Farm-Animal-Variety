# Paritee's Better Farm Animal Variety

Customize the types and species of farm animals you can raise without needing to replace the default farm animal types

## Contents

- [Get Started](#get-started)
- [Configure](#configure)
- [Extend](#extend)

## Get Started

### Install

1. Install the latest version of [SMAPI](https://smapi.io/)
2. Install the latest version of [Content Patcher](https://www.nexusmods.com/stardewvalley/mods/1915)
3. Download the Paritee's Better Farm Animal Variety (BFAV) mod files from [Nexus Games](https://www.nexusmods.com/stardewvalley/mods/3273)
4. Unzip the mod files into `Stardew Valley/Mods`
5. Run the game using SMAPI

### Add New Farm Animal

In this example we will be using [Paritee's White Bull](https://www.nexusmods.com/stardewvalley/mods/3298) mod

1. Make sure you following the [installation instructions](#install)
2. Unzip the [Paritee's White Bull](https://www.nexusmods.com/stardewvalley/mods/3298) folder into `Stardew Valley/Mods`
3. Add "White Bull" to the `Cows.Types` array inside BFAV's `config.json`
4. Run the game using SMAPI

Your `Cows` section of the `config.json` should now look like the following:

```json
"Cows": {
  "Name": "default",
  "Description": "default",
  "ShopIcon": "default",
  "Types": [
    "White Cow",
    "Brown Cow",
    "White Bull"
  ]
},
```


## Configure

You can configure your mod at `Stardew Valley/Mods/Paritee's Better Farm Animal Variety/config.json`

### Fields

#### VoidFarmAnimalsInShop

| Value  | Description |
| ------------- | ------------- |
| `0` | Void farm animals will never be available in [Marnie's animal shop](https://stardewvalleywiki.com/Marnie%27s_Ranch#Livestock) (default) |
| `1` | Void farm animals will only be available in [Marnie's animal shop](https://stardewvalleywiki.com/Marnie%27s_Ranch#Livestock) if the player has completed the [Goblin Problem](https://stardewvalleywiki.com/Quests#Goblin_Problem) quest |
| `2` | Void farm animals are always availabe in [Marnie's animal shop](https://stardewvalleywiki.com/Marnie%27s_Ranch#Livestock) |

#### FarmAnimals

##### Chickens, Cows, Dinosaurs, Ducks, Goats, Pigs, Rabbits, Sheep

| Name | Type | Description |
| ------------- | ------------- | ------------- |
| `Name` | `string` | `default` for no change or a custom display name of the species (ex. `"Dairy Cow"`) |
| `Description` | `string` | `default` for no change or a custom description of the farm animal's species (ex. `"Adults can be milked daily. A milk pail is required to harvest the milk."`) |
| `ShopIcon` | `string` | `default` for no change or the filename of your file in `Stardew Valley/Mods/Paritee's Better Farm Animal Variety/assets`. These icons are used for the species options in [Marnie's animal shop](https://stardewvalleywiki.com/Marnie%27s_Ranch#Livestock) menu. The vanilla icons are saved in the `assets` directory for your use (ex. `"animal_shop_dairy_cows.png"`) |
| `Types` | `string []` | The types of farm animals that exist in the game for this species. The types must exist in `Stardew Valley/Content/Data/FarmAnimals` (ex. `["White Cow", "Brown Cow"]`) |

### Default

Here is a sample of a default `config.json` file:

```json
{
  "VoidFarmAnimalsInShop": 0,
  "FarmAnimals": {
    "Chickens": {
      "Name": "default",
      "Description": "default",
      "ShopIcon": "default",
      "Types": [
        "White Chicken",
        "Brown Chicken",
        "Blue Chicken",
        "Void Chicken"
      ]
    },
    "Cows": {
      "Name": "default",
      "Description": "default",
      "ShopIcon": "default",
      "Types": [
        "White Cow",
        "Brown Cow"
      ]
    },
    "Dinosaurs": {
      "Name": "default",
      "Description": "default",
      "ShopIcon": "default",
      "Types": [
        "Dinosaur"
      ]
    },
    "Ducks": {
      "Name": "default",
      "Description": "default",
      "ShopIcon": "default",
      "Types": [
        "Duck"
      ]
    },
    "Goats": {
      "Name": "default",
      "Description": "default",
      "ShopIcon": "default",
      "Types": [
        "Goat"
      ]
    },
    "Pigs": {
      "Name": "default",
      "Description": "default",
      "ShopIcon": "default",
      "Types": [
        "Pig"
      ]
    },
    "Rabbits": {
      "Name": "default",
      "Description": "default",
      "ShopIcon": "default",
      "Types": [
        "Rabbit"
      ]
    },
    "Sheep": {
      "Name": "default",
      "Description": "default",
      "ShopIcon": "default",
      "Types": [
        "Sheep"
      ]
    }
  }
}
```

### Extend

- [Generate Farm Animal Data](https://paritee.github.io/#generate-data-farmanimals-entry)
- [Paritee's Gender-Neutral Farm Animals](https://www.nexusmods.com/stardewvalley/mods/3289)
