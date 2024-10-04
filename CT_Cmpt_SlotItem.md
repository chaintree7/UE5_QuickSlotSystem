
# CT_Cmpt_SlotItem
#### You only need to add this component to your Actor
![image](https://github.com/user-attachments/assets/5d2a211c-63fe-4f48-95cb-9f9ec92c2afd)


# Configuration
![image](https://github.com/user-attachments/assets/cb357a62-a00a-4903-b0dc-338160847b89)
| Name| Description |
| ----------- | ----------- |
| `Tags` |  `Gameplay Tags` 
| `Key` |  `The purpose is to quickly find Actor by Key` 
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
| `RequiredTag` |  `Contain any tag to activated` 
| `BlockedTag` |  `If it contains any tag, it will be blocked` 
| `RequiredTags` |  `All tags must be contains to be activated` 
| `BlockedTags` | `If it contains all Tags, it will be blocked.` 


# Functions

| Name| Description |
| ----------- | ----------- |
| `Set Stack` |  `Set stack number` 
| `Inc Stack` |  `Increase or decrease stack number` 
| `Get Stack` |  `Get stack number` 
| `Get Slot Type` | `Get current SlotType` 
| `IsActivated` | `Returns if the current Actor is activated` 
| `Get Tags` | `Get GameplayTags (Config)` 
| `Get Texture ` | `Get Texture (Config)` 
| `Set Available` | `Change the current Actor available status` 
| `SetAvailableAfterDelay` | `Put current Actor on cooldown Not available` 
| `IsAvailable` | `Returns if the current Actor is available` 
| `GetAvailableDelayTimeLeft` | `Get cooldown remaining time` 

# Events

| Name| Description |
| ----------- | ----------- |
| `Event_OnAdded` |  `When current Actor is added to slot` 
| `Event_OnRemoved` |  `When current Actor is removed from slot` 
| `Event_OnUsed` |  `When current Actor is selected` 
| `Event_OnUnused` | `When current Actor is deselected` 
| `Event_OnMessage` | `When a message is received` 
| `Event_OnTriggered ` | `When trying to use the current slot` 
| `Event_OnSlotTypeChanged` | `When current Actor swaps with another Actor and changes SlotType` 
| `Event_OnAvailableChanged` | `When available status changes` 
| `Event_OnActivationChanged` | `When active status changes` 
| `Event_OnStackChanged` | `When stack number changes` 
| `Event_OnBeginAvailableDelayTimer` | `When cooldown starts` 
| `Event_OnEndAvailableDelayTimer` | `When cooldown ends` 

#### Example
![image](https://github.com/user-attachments/assets/d9fb3448-56b0-434f-8312-3408bb4bb566)


