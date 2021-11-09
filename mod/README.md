# Overview

Are you a mod developer who is wishing for a quieter `error.log` while you debug with the Ascendant Shipset active?  Then this mod is for you (and me)!  This mod does **NOT** redistribute any of the graphics from the Ascendant Shipset, but does redefine and replace entity asset files in order to eliminate many error messages.

# Changes

Many entity definitions were tweaked to remove animations.  "Removed" code was commented out rather than deleted.  Garyx Starlight, please feel free to harvest any of these adjustments for use in your mod directly.

* `common\component_templates\00_RIG_ASC_utilities_race_roles.txt` blank file to remove RIG:US computers in order to stop error messages
* `common\component_templates\00_RIG_ASC_weapons.txt` blank file to remove RIG:US weapons in order to stop error messages
* `common\technology\RIG_ASC_species_tech.txt`:
    * add missing tech icon (reuses the same one as the built-in corvette technology)
    * add missing description for prerequisite
    * enable global flag check for RIG: Unique Shipset Mod so the technology does not appear when it is not installed
* `common\section_templates\asc_battleship_RIG.txt` remove section `RIG_ASC_BATTLESHIP_BOW_1X2M` to reduce many error messages
* `gfx\models\portraits\ascendant\_ascendant_portrait_animations.asset` blank file to remove unnecessary animation redefinitions
* `gfx\models\ships\ascendant_01\battleship\ascendant_01_battleship.asset`:
    * add missing locators to `ascendant_01_battleship_entity`: `part2`, `part3`
    * add missing locator to `ascendant_01_battleship_bow_M1S2SHB_entity`: `strike_craft_locator_01`
* `gfx\models\ships\ascendant_01\cruiser\ascendant_01_cruiser.asset`:
    * add missing locators to `ascendant_01_cruiser_entity`: `part2`, `part3`
    * add missing locator to `ascendant_01_cruiser_mid_S2HB_entity`: `strike_craft_locator_01`
* `gfx\models\ships\ascendant_01\destroyer\ascendant_01_destroyer.asset`:
    * add missing locator to `ascendant_01_destroyer_entity`: `part2`
    * add missing locators to `ascendant_01_destroyer_stern_RIG_entity`: `pd_01`, `pd_02`, `pd_03`, `pd_04`
* `gfx\models\ships\ascendant_01\juggernaut\ascendant_01_juggernaut.asset`:
    * remove unnecessary animation redefinitions
    * remove animations from `ascendant_01_juggernaut_entity` (mesh is not animated)
* `gfx\models\ships\ascendant_01\juggernaut\ascendant_01_juggernaut.gfx`:
    * remove animations from `ascendant_01_juggernaut_mesh` (not compatible with mesh)
    * remove animations from `ascendant_01_juggernaut_mesh_2` (not compatible with mesh)
* `gfx\models\ships\ascendant_01\megastructures\gateway\ascendant_01_gateway.asset`:
    * remove unnecessary animation redefinitions
    * remove animations from `ascendant_01_gateway_entity` (mesh is not animated)
    * remove animations from `ascendant_01_deactivated_gateway_entity` (mesh is not animated)
    * remove animations from `ascendant_01_reactivated_gateway_entity` (mesh is not animated)
* `gfx\models\ships\ascendant_01\megastructures\gateway\ascendant_01_gateway.gfx`
    * remove animations from `ascendant_01_gateway_mesh` (not compatible with mesh)
* `gfx\models\ships\ascendant_01\megastructures\science_nexus\ascendant_01_nexus_assets.asset`:
    * remove animations from `ascendant_01_thinktank_phase_01_entity` (mesh is not animated)
    * remove animations from `ascendant_01_thinktank_phase_02_entity` (mesh is not animated)
    * remove animations from `ascendant_01_thinktank_phase_03_entity` (mesh is not animated)
* `gfx\models\ships\ascendant_01\megastructures\shipyard\ascendant_01_shipyard_assets.asset`:
    * remove animations from `ascendant_01_mega_shipyard_01_stage_1_section_entity` (mesh is not animated)
    * remove animations from `ascendant_01_mega_shipyard_01_stage_2_section_entity` (mesh is not animated)
    * remove animations from `ascendant_01_mega_shipyard_01_stage_3_section_entity` (mesh is not animated)
* `gfx\models\ships\ascendant_01\megastructures\spy_orb\ascendant_01_sensor_array_assets_supplemental.asset`
    * add file with missing construction entities (otherwise the sentry array uses the original outlines while under construction)
    * add entity `ascendant_01_spyorb_phase_01_construction_entity`
    * add entity `ascendant_02_spyorb_phase_01_construction_entity`
    * add entity `ascendant_03_spyorb_phase_01_construction_entity`
    * add entity `ascendant_04_spyorb_phase_01_construction_entity`
* `gfx\models\ships\ascendant_01\megastructures\spy_orb\ascendant_01_sensor_array_assets.asset`:
    * remove animations from `ascendant_01_spyorb_phase_01_entity` (mesh is not animated)
    * remove animations from `ascendant_01_spyorb_phase_02_entity` (mesh is not animated)
    * remove animations from `ascendant_01_spyorb_phase_03_entity` (mesh is not animated)
    * remove animations from `ascendant_01_spyorb_phase_04_entity` (mesh is not animated)
* `gfx\models\ships\ascendant_01\military_stations\ascendant_01_military_stations.asset`:
    * add missing locators to `ascendant_01_military_station_section_light_entity`: `small_gun_01`, `small_gun_02`, `small_gun_03`, `small_gun_04`
    * add missing locators to `ascendant_01_military_station_section_medium_entity`: `medium_gun_01`, `medium_gun_02`
    * add missing locators to `ascendant_01_military_station_section_heavy_entity`: `large_gun_01`
* `gfx\models\ships\ascendant_01\starbases\ascendant_starbase_entities.asset`:
    * remove animations from `ascendant_01_orbital_station_core_entity` (mesh is not animated)
    * add missing locators to `ascendant_01_starbase_citadel_section_entity`: `medium_gun_010`, `medium_gun_011`, `medium_gun_012`, `medium_gun_013`
* `gfx\models\ships\ascendant_01\starbases\ascendant_starbase_meshes.gfx`:
    * remove animations from `ascendant_01_starport_mesh` (not compatible with mesh)
    * remove animations from `ascendant_01_citadel_mesh` (not compatible with mesh)
    * remove animations from `ascendant_01_starfort_mesh` (not compatible with mesh)
    * remove animations from `ascendant_01_starhold_mesh` (not compatible with mesh)
    * remove animations from `ascendant_01_outpost_mesh` (not compatible with mesh)
* `gfx\models\ships\ascendant_01\titan\ascendant_01_titan.asset`
    * remove animations from `ascendant_01_titan_bow_entity` (mesh is not animated)
    * remove animations from `ascendant_01_titan_mid_entity` (mesh is not animated)
    * remove animations from `ascendant_01_RIG_titan_mid_entity` (mesh is not animated)
    * remove animations from `ascendant_01_titan_stern_entity` (mesh is not animated)
    * remove animations from `ascendant_01_RIG_titan_stern_entity` (mesh is not animated)
    * add missing locators to `ascendant_01_RIG_titan_stern_entity`: `hangar_01`, `hangar_02`, `hangar_03`, `hangar_04`, `hangar_05`, `hangar_06`
* `gfx\models\ships\ascendant_01\ascendant_01_RIG_ascendant_destroyer.asset` blank file to remove duplicate entity `RIG_ascendant_corvette_mid_M1S2_entity`
* localisation - add the second `£` to the alloy icons for correct syntax

## Compatibility

Removes some compatibility with [Unique Shipset Mod](https://steamcommunity.com/sharedfiles/filedetails/?id=2286837494) because I don't use it and I don't want to see all the false-positive error messages.  The battleship bow XL1M2 section (`RIG_ASC_BATTLESHIP_BOW_1X2M`) complained that each built-in game battleship bow XL1 entity did not have the locators added by that section.  The RIG:US role computers and weapons were removed in order to avoid error messages regarding missing component sets, ship sizes, component tags, projectile graphics, and technologies.

Built for Stellaris version 3.1.\* "Lem."  Not compatible with achievements.

### Required Dependency Mods

[Ascendant Shipset](https://steamcommunity.com/sharedfiles/filedetails/?id=2130588320) for the original graphics and other ship-related code.

### Recommended Companion Mods

[Aesthetic Terraform Stations](https://steamcommunity.com/sharedfiles/filedetails/?id=2622411084) will give you back the very old-school terraform stations as visual markers for terraforming planets.

[Ascendant Shipset Add-on: Aesthetic Terraform Station Compatibility](https://steamcommunity.com/sharedfiles/filedetails/?id=) this compatibility patch ensures the correct Ascendant Shipset graphics are used for the above terraform stations.

## Changelog

* 1.0.0 Initial version

## Source Code

Hosted on [GitHub](https://github.com/corsairmarks/ascendant_shipset_no_error_logs)

### Development Notes

It is best to clone this repository into `<Stellaris User's Directory>/Paradox Interactive/Stellaris/mod`, and then make a connection to the `mod` folder via a `*.mod` file's `path` property.  That will ensure the game can see the files, and also that CWTools will parse them.  Also note that the README.md file exists in the `mod` directory but is symbolically linked in the root directory.