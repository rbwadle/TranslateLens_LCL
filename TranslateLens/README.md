# Localization Support Assets

Move the contents of this folder (TranslateLens) to your `SDK\Stalker2\Mods\` folder so that it is at the same level as your  `TranslateLens_LCL` mod folder.
You should end up with two registered mods in the file structure below (Resource Folder can be omitted)

```
SDK/
└── Stalker2/
    └── Mods/
        ├── TranslateLens/
        │   ├── Content/
        │   │   └── Data/
        │   │       ├── EAssetType.uasset
        │   │       └── S_TranslationItem.uasset
        │   └── TranslateLens.uplugin
        └── TranslateLens_LCL/
            ├── Content/
            │   └── Data/
            │       ├── DT_Translations_LCL.uasset
            │       └── Translations.csv
            └── TranslateLens_LCL.uplugin
```

