# TranslateLens (Localization Add-on)
This repository is meant for those who would like to publish their own alternate lanugage translations for the S.T.A.L.K.E.R. 2 Mod TranslateLens.

It contains all of the raw assets needed to create a localized translation database which can be used to override the default English translations that come default with the TranslateLens mod.

## Prerequisites
In order to create your localization add-on you will need the following:
* __ZoneKit SDK__ Installed on local machine
* Fluency in __Target Language__ (which will be shown in-game)
* Fluency in __English__
* Understanding and __ability to modify CSV__ (Comma-Separated Values) files.

## Overview
The basic steps that will be required to make an alternate language add-on mod look like the following:
1. Create a new __Mod Project__ in the ZoneKit
2. Clone this repository into your newly created mod's `Content` folder.
3. Open and edit the `data\translations.csv` file
4. Open the `data\DT_Translations_LCL` datatable asset in the ZoneKit and reimport the modified `translations.csv`
5. Package and test mod.

## Modifying `translations.csv`
Within the `data\` folder you will find a CSV dump of the `DT_translations` DataTable asset.  A sample of which is shown below:

|Row Name|AssetType|Orig|EN|LCL|FontSize|
|--------|---------|----|--|---|--------|
|`MI_dec_grouping_01_bandits_01`|Decal|шо,<br>не фартанулр?|What,<br>No Luck?||70|
|`MI_dec_grouping_01_bandits_02`|Decal|твій хабар - мій хабар|Your loot - My Loot|Your loot is mine now|0|
|`MI_dec_grouping_01_bandits_03`|Decal|шо ти,<br>дядя?|What are you up to,<br>Uncle?|What up,<br>Cos?|70|

### Columns Guide
|Column|Description|Example|Notes|
|-|-|-|-|
|Row Name|Reflects the name of the target asset as it is referred to in game|`MI_dec_grouping_01_bandits_01`| Should not be modified or changed |
|AssetType|Type of asset which will be targeted|Decal|currently only decal assets are in-scope for the early version of TranslateLens, however the ability to show translations for StaticMeshes (Signs,Posters) and other assets is planned|