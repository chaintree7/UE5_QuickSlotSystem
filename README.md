# Quick Slot System (Coming Soon)
### This `Component` has two forms ( `Soul Like` and `General RPG Like` ) , The good news is that they are just differences in UI presentation, and you don’t need any coding

![image](https://github.com/user-attachments/assets/c613fd79-3f7a-4713-9b1c-be7c85e67c30)

# Introduction
#### There are 4 containers named (Top, Right, Bottom, Left). You can add any `Actor` to the `Container`, such as `weapons`, `potions`, `skills`, `Ammo`, It uses an `Event-Driven` architecture, so you don't need to extend any `parent class` or `interface`, you just need to add a `component` to your `Actor`

# CT_Cmpt_QuickSlot_Item
#### You only need to add this component to your Actor and listen to these main events as needed.
![image](https://github.com/user-attachments/assets/cbcb9060-3352-4677-9257-7435a9b5e83b)
#### Configuration
![image](https://github.com/user-attachments/assets/cb357a62-a00a-4903-b0dc-338160847b89)
| Name| Description |
| ----------- | ----------- |
| `Tags` |  `Gameplay Tags` 
| `Key` |  `Unique identifier` 
| `Stack` |  `Number of stacks` 
| `Activation Tags` | `Activate rules` 
| `Textures` | `Icons used to display on the UI`  
#### In the end it looks like this
![image](https://github.com/user-attachments/assets/162f0c3a-6556-4666-a289-7c6b2c67b01f)

### `Activation Tags`
#### Sometimes you want an Actor to only work in certain situations, like shield only working with sword, arrow only working with bow, or some skills only working with a specific weapon. Activation Tags are very useful in this case.
#### If you have a skill that can only be activated when you equipped sword and shield , you can configure it like this
![image](https://github.com/user-attachments/assets/c57dfe06-c9b0-494c-b1c3-a7ef7ae31c7e)

![image](https://github.com/user-attachments/assets/1e1f4313-e450-4d33-b7b6-724a14e95863)
#### This skill is not available when dual swords
![image](https://github.com/user-attachments/assets/306f98e7-2a83-4be3-9db8-cf3ebb8b23f7)
| Name| Description |
| ----------- | ----------- |
| `RequiredTag` |  `Contain any tag to activate` 
| `BlockedTag` |  `If it contains any tag, it will be blocked` 
| `RequiredTags` |  `All tags must be contains to be activated` 
| `BlockedTags` | `If it contains all Tags, it will be blocked.` 

#### Others Function & Events
![image](https://github.com/user-attachments/assets/85bc16b3-9501-4e67-80dd-e661bbebef7e)
#### The following are mainly used for skill cooldowns, but this is not essential, if you have your own skill system you can not use them
![image](https://github.com/user-attachments/assets/d30737b9-b040-4f99-bda5-c5689f982eec)
