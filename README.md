# MSage's Follower Pet System 6

MSage's Follower Pet System 6 is a Unity Editor tool for installing and managing follower pets on VRChat avatars.

The installer helps add the follower pet system prefab, animator controllers, expression menu, and expression parameters to a selected VRChat avatar. It can also assign compatible follower pets into pet slots and configure the required slot-specific settings automatically.

## Get Follower Pets

Follower pets are acquired separately from the pet system itself.

You can get compatible MSage follower pets from my shop:

https://www.payhip.com/msage

## Requirements

- Unity project using the VRChat SDK3 Avatar SDK
- A VRChat avatar with a `VRCAvatarDescriptor`
- MSage's Follower Pet System 6 imported into the Unity project
- Compatible MSage follower pet packages imported into the same project

The installer script must remain inside a Unity `Editor` folder.

## Installing the Pet System

1. Import `MSageFollowerPets6-v6.0.0.unitypackage` into your Unity project.
2. Open the installer from the Unity top menu:

   `MSage > Follower Pets > 2.Follower Pet Installer Tool`

3. Drag your VRChat avatar GameObject into the `Avatar` slot.
4. Click `Install Follower Pet System`.

The installer will:

- Add the `Follower Pets` prefab to your avatar.
- Merge the follower pet FX controller into your avatar's FX layer.
- Merge the follower pet Action controller into your avatar's Action layer.
- Create missing avatar FX or Action controllers if needed.
- Add the follower pet menu to your avatar's main expressions menu.
- Add required follower pet expression parameters to your avatar's expression parameters asset.

If your avatar's main expression menu is already full, remove one main menu option before installing the system.

## Assigning Pets

Follower pets must be imported into the project separately.

After importing one or more compatible pet packages:

1. Open the installer.
2. Select your avatar.
3. Click `Refresh Pet Listings`.
4. Under `Follower Pet Selection`, choose a pet for each slot.
5. Click `Assign Pets`.

The installer will:

- Place each selected pet prefab into the correct pet slot.
- Configure slot-specific contact receiver parameters.
- Configure slot-specific PhysBone parameters.
- Configure pet station settings.
- Merge the selected pet's animation controller into the avatar FX controller.
- Apply ridable/grounded settings from the pet's identification file.

Selecting `(None)` means no pet will be assigned to that slot.

## Removing Pets

To remove assigned pets without removing the whole pet system:

1. Select your avatar in the installer.
2. Click `Remove Pets`.

This removes assigned pet prefabs and pet animation layers while keeping the main follower pet system installed.

## Removing the Pet System

To remove the full follower pet system from your avatar:

1. Select your avatar in the installer.
2. Click `Remove Pet System`.

This removes the follower pet system prefab, installed pet animation layers, follower pet menu entry, and follower pet expression parameters.

## Quest Mode

Quest Mode is available in the installer.

When `Quest Mode` is enabled:

- Only Pet Slot 1 is available.
- Pet Slots 2, 3, and 4 are disabled.
- The installer uses the pet prefab inside the pet's `Quest` folder.
- The remote camera point is removed from the installed follower pet system.

Example Quest prefab path:

`Assets/MSage's Follower Pets 6/Example Pet/Prefabs/1.Default/Quest/Follower Pet.prefab`

## Follower Pet Settings

The installer includes quick selection buttons for adjusting pet settings in the scene.

For each pet slot, you can select:

- `Location`
- `Scale`
- `Station Point`

These buttons select the correct object on the avatar and activate the appropriate Unity transform tool.

## General Pet Settings

The installer also includes general setting buttons:

- `Remote Screen`
- `Other Player Tracker`
- `Reset Pet Settings`

`Reset Pet Settings` restores pet setting transforms back to their default values.

## Updating

This package is updater-ready.

The latest version information is available from:

https://raw.githubusercontent.com/MSage3D/FollowerPets6/main/update.json

Future versions may allow the installer to check for updates automatically from this GitHub repository.

## Support

For MSage assets and compatible follower pets, visit:

https://www.payhip.com/msage

## Notes

Do not move the installer script out of the `Editor` folder.

Do not rename or move the core system folders unless an update specifically says it is safe to do so, since the installer depends on known asset paths.

## Version

Current version:

`6.0.0`
