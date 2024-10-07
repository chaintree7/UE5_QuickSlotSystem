### Add a Component to Character
![image](https://github.com/user-attachments/assets/beebe54e-1383-4da8-8bd8-389cc8dcc35c)

## The confusing part: `Index` is activated list index And `Array Index` is the real index
#### For Example：LeftSlots = [Shield, Arrow1, Arrow2, Arrow3], If current weapon is Bow, only Arrows activated
#### Index1 = [Arrow1, Arrow2, Arrow3].get(1) = Arrow2
#### RealIndex1 = [Shield, Arrow1, Arrow2, Arrow3].get(1) = Arrow1

# Config
![image](https://github.com/user-attachments/assets/4ef3b0bf-7dcf-4661-ad7a-40fa60903782)

| Name| Description |
| ----------- | ----------- |
| `Slot Type Priority` |  The following Slot activation rule can be the above Slot, otherwise it will be an infinite loop
| `Allow Empty` |  If configured, SetIndex can select empty slot, and if the class exists it will receive all events.

# Actor Functions

| Name| Description |
| ----------- | ----------- |
| `Add Actor` |  `Add by object` 
| `Add Actor By Class` |  `Add by class (auto spawn)` 
| `Get Actor` |  `Get current selected actor` 
| `Get Actor By Class` |  `Get by class` 
| `Get Actor By Key` |  `Get By Key` 
| `Get Actor By Index` |  `Get By Index` 
| `Get Actor By Array Index` |  `Get By Array Index` 
| `Get Actors` |  `Get all actors` 
| `Get Active Actors` |  `Activated actors` 
| `Remove Actor` |  `Remove by object` 
| `Remove Actor By Class` | `Remove by class` 
| `Remove Actor By Key` | `Remove by key`  
| `Remove Actor By Index` | `Remove by Index`  
| `Remove Actor By Array Index` | `Remove by Array Index`  

#### Example
![image](https://github.com/user-attachments/assets/488c7e34-1cea-40ee-866b-1e4d1a42ca2a)

![image](https://github.com/user-attachments/assets/51df2ddb-6e56-4c15-87d1-dd2fa7cc1417)


# Index Functions 
| Name| Description |
| ----------- | ----------- |
| `Inc Index` |  `Increase or decrease index` 
| `Set Index` |  `Set slot index` 
| `Get Index` |  `Get current index` 
| `Get Index By Actor` |  `Get index based on Object` 
| `Get Index By Key` |  `Get index based on key` 
| `Get Array Index` |  `Get current real index` 
| `Get Array Index By Actor` |  `Get real index based on Object` 
| `Get Array Index By Key` | `Get real index based on key`  
| `Swap Array Index` | `swap actors`  

#### Example
![image](https://github.com/user-attachments/assets/34a38c6a-5855-4192-9807-385660fa2b8a)
![image](https://github.com/user-attachments/assets/5f1895ee-c281-4c82-8240-6f6e12b00ff8)


# Interaction 
| Name| Description |
| ----------- | ----------- |
| `Send Message` |  `Send a message to Actor` 
| `Trigger` |  `Similar to SendMessage, except that it is only sent when the Actor is available.` 
| `Trigger By Key` |  `---` 
| `Trigger By Index` |  `---` 


#### Example: This will send a message to Slot, which can then do something based on the name of the message, such as playing a montage.
![image](https://github.com/user-attachments/assets/eba5ba1e-7ee6-45d3-916e-5e69520db7ce)



# Event

#### This event is triggered when the slot array changes. It is mainly used to refresh the UI.
![image](https://github.com/user-attachments/assets/0a8e4b68-0cfa-4243-a75f-289ce81e1c17)

