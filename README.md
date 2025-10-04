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