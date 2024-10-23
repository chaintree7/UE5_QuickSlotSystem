# Quick Slot System (Coming Soon)

![image](https://github.com/user-attachments/assets/c613fd79-3f7a-4713-9b1c-be7c85e67c30)

# Introduction

#### This is a very flexible system. With it, you can make your game compatible with both Keyboard and Gamepad and make the logic of your project very clear and uncoupled.
#### It is an event-driven architecture (no parent class, no interface). All communication is done through events. You only need to add a component. In simple terms, all items in the game (Weapon, Skills, Props etc.) are Actor basic types. You don't need to care about the specific type of Actor, so there is no need to use ugly things like Cast to XXX.

# [CT_Cmpt_QuickSlot](https://github.com/chaintree7/UE5_QuickSlotSystem/blob/main/CT_Cmpt_QuickSlot.md)
#### https://github.com/chaintree7/UE5_QuickSlotSystem/blob/main/CT_Cmpt_QuickSlot.md
#### QuickSlot needs to be added to Character. Its main function is to manage slots. The component provides 5 slots, namely Top, Right, Bottom, Left, and Center. You can use these slots to implement functions similar to the Elden Ring. Center is reserved and you can use it at will according to your needs.
#### This is made in imitation of the Elden Ring. It is very suitable for Gamepad
![image](https://github.com/user-attachments/assets/4a69250d-c070-4ccd-9582-e52836c56517)
#### In addition, the Demo also provides a UI version for PC
![image](https://github.com/user-attachments/assets/2d22edfc-7bc5-4d3d-b3a1-8c9adefe4b1d)

# [CT_Cmpt_SlotItem](https://github.com/chaintree7/UE5_QuickSlotSystem/blob/main/CT_Cmpt_SlotItem.md)
#### https://github.com/chaintree7/UE5_QuickSlotSystem/blob/main/CT_Cmpt_SlotItem.md
#### SlotItem needs to be added to an Actor such as Weapon, Props, Skills etc. After adding, you can listen to events and then interact with CT_Cmpt_QuickSlot
![image](https://github.com/user-attachments/assets/7606f323-c36f-451a-86c4-89db625b12f6)

****
# requires extra work
## GameplayTags
#### Due to market limitations, When adding this product from Marketplace, GameplayTags will not be added to project. You need to download this file and copy it to your project directory /Config/Tags/

## Montage Replication
#### Montages in the Demo is not replicated by default, You need to add another product of mine [NetworkMontageSystem (Free)](https://github.com/chaintree7/UE5_NetworkMontageSystem) , and open /Content/CT_Components/Demos/QuickSlotSystem/Items/BP_Item and find the following code
![image](https://github.com/user-attachments/assets/e751760f-3101-4512-8485-c86efc85f043)
#### change it to the following 
![image](https://github.com/user-attachments/assets/365687c8-2747-4d29-88f1-24ed15b0881a)



