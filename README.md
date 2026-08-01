# ESO Add-on Mirror — Shard 01

This public repository is one storage shard of the [ESO Add-on Mirror](https://github.com/the-jolly-green-bryant/eso-addon-mirror). It keeps unpacked Elder Scrolls Online add-ons browsable on GitHub without forcing catalog and website builds to clone the whole archive.

## Layout

```text
addons/AUTHOR/TITLE__SOURCE_ID/
```

The author and title make the tree readable. The immutable Bethesda UUID or ESOUI numeric ID is the identity, so renaming or transferring an add-on moves its folder instead of creating a duplicate. A stable hash of `bethesda:UUID` or `esoui:ID` assigns the shard.

Each leaf includes `addon.json`, whose shape follows the Bethesda catalog model and adds normalized source/archive fields. The root catalog and sync software live in the control repository linked above.

## Stewardship

This is an unofficial preservation project and is not endorsed by Bethesda Softworks, ZeniMax Online Studios, or ESOUI/MMOUI. Add-ons remain the work of their respective authors and retain their own licenses. Inclusion here does not grant a new redistribution license. Attribution and takedown concerns should be reported through the control repository.

The transparency-only license in the control repository applies to the mirroring software, not automatically to archived add-on content.
