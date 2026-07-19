# MSage's Follower Pet System 6

MSage's Follower Pet System 6 is a Unity Editor tool for installing follower pets onto VRChat avatars.

Follower pets are acquired separately from the pet system itself. You can get compatible pets from my shop:

https://www.payhip.com/msage

## Requirements

- Unity project with the VRChat SDK3 Avatar SDK
- A VRChat avatar with a `VRCAvatarDescriptor`
- MSage's Follower Pet System 6 imported into the project
- Compatible MSage follower pet packages imported into the project

## Opening the Installer

After importing the package, open the installer from the Unity top menu:

`MSage > Follower Pets > 2.Follower Pet Installer Tool`

Drag your avatar GameObject into the `Avatar` slot.

## Installing the Follower Pet System

1. Select your avatar in the installer.
2. Click `Install Follower Pet System`.

The installer will add the required follower pet system to your avatar.

If your avatar's main expressions menu is full, remove one option from the main menu before installing.

## Adding Pets to Your Avatar

Before assigning pets, make sure you have imported compatible MSage follower pet packages into the same Unity project.

1. Open the installer.
2. Select your avatar.
3. Click `Refresh Pet Listings`.
4. Choose a pet from the dropdown for each pet slot.
5. Click `Assign Pets`.

Choosing `(None)` means no pet will be assigned to that slot.

## Quest Mode

Enable `Quest Mode` if you are setting up a Quest-compatible version.

When Quest Mode is enabled:

- Only Pet Slot 1 can be used.
- Pet Slots 2, 3, and 4 are disabled.
- The installer uses the Quest version of the selected pet prefab.

## Adjusting Pet Settings

The `Follower Pet Settings` section lets you quickly select important pet setup objects on your avatar.

Each pet slot includes:

- `Location`
- `Scale`
- `Station Point`

Clicking one of these buttons selects the related object in the hierarchy and activates the correct transform tool.

## General Pet Settings

The `General Pet Settings` section includes:

- `Remote Screen`
- `Other Player Tracker`
- `Reset Pet Settings`

Use `Reset Pet Settings` to return pet setting objects back to their default positions, rotations, and scales.

## Removing Pets

To remove assigned pets while keeping the pet system installed:

1. Select your avatar.
2. Click `Remove Pets`.

## Removing the Pet System

To remove the full follower pet system from your avatar:

1. Select your avatar.
2. Click `Remove Pet System`.

## Getting More Pets

Compatible follower pets can be purchased separately from my shop:

https://www.payhip.com/msage
