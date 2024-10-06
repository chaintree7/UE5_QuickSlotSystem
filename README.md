# Quick Slot System (Coming Soon)
### This `Component` has two forms ( `Soul Like` and `General RPG Like` ) , The good news is that they are just differences in UI presentation, and you don’t need any coding

![image](https://github.com/user-attachments/assets/c613fd79-3f7a-4713-9b1c-be7c85e67c30)

# Introduction
#### There are 4 containers named (Top, Right, Bottom, Left). You can add any `Actor` to the `Container`, such as `weapons`, `potions`, `skills`, `Ammo`, It uses an `Event-Driven` architecture, so you don't need to extend any `parent class` or `interface`, you just need to add a `component` to your `Actor`

# Prerequisites
## GameplayTags
#### When adding this product from the Marketplace, GameplayTags will not be added to the project. You need to download this file and copy it to your project directory /Config/Tags/

## Montage Replication
#### Montages in the Demo is not replicated by default, you need to replace some things, open /Content/CT_Components/Demos/QuickSlotSystem/Items/BP_Item and find the following code
![image](https://github.com/user-attachments/assets/e751760f-3101-4512-8485-c86efc85f043)
#### Add NetworkMontageSystem to project and change it to the following https://github.com/chaintree7/UE5_NetworkMontageSystem
![image](https://github.com/user-attachments/assets/7040a3a7-6570-4a15-ae43-82317edb2315)

