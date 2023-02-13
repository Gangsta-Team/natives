# StatePropObject
## Functions
| Function | Note |
|----------|------|
|[AddHealth](AddHealth.md)| |
|[ApplyDamage](ApplyDamage.md)| |
|[CarriedByPlayer](CarriedByPlayer.md)| |
|[CarriedObjectIsSafeToDrop](CarriedObjectIsSafeToDrop.md)| |
|[CarriedObjectSetOffset](CarriedObjectSetOffset.md)| |
|[CarriedObjectSetRotationSpeed](CarriedObjectSetRotationSpeed.md)| |
|[DestroyPropObject](DestroyPropObject.md)| |
|[EnableCollision](EnableCollision.md)| |
|[GetCurrentHealth](GetCurrentHealth.md)| |
|[GetStateIndex](GetStateIndex.md)| |
|[GetWorldLocatorPosition](GetWorldLocatorPosition.md)| |
|[IsDestroyed](IsDestroyed.md)| |
|[IsState](IsState.md)| |
|[PlayPickupSound](PlayPickupSound.md)| |
|[RegisterForStateCallbacks](RegisterForStateCallbacks.md)| |
|[RequestStateSound](RequestStateSound.md)| |
|[ResetHealth](ResetHealth.md)| |
|[SetIsHighestPriorityForCuller](SetIsHighestPriorityForCuller.md)| |
|[SetPriorityScale](SetPriorityScale.md)| |
|[SetRemoveInNIS](SetRemoveInNIS.md)| |
|[SetState](SetState.md)| |
|[SetStateIndex](SetStateIndex.md)| |
## Description
```
Functions: 22
```

## Usage examples

### Spawn Way Point
```c#
// Create new instance of StatePropObject.
$delivery_prop_last = new StatePropObject("DELIVERY_PROP_LAST");
// Find main character object.
$maincharacter = FindObject("MainCharacter");
if($delivery_prop_last){
	// Set delivery_prop_last object position in the same position than the main character.
	$delivery_prop_last.position = $maincharacter.position;
	// Set delivery_prop_last object direction in the same direction than the main character.
	$delivery_prop_last.direction = $maincharacter.direction;
	$delivery_prop_last.roll = "2.9649200";
	$delivery_prop_last.name = "DELIVERY_PROP_LAST";
	$delivery_prop_last.scriptClass = "";
	$delivery_prop_last.modelName = "wayPoint";
	Echo("DBG", "StatePropObject: DELIVERY_PROP_LAST new object has been created!");
}	
```
![image](https://user-images.githubusercontent.com/44430306/218584682-0743d175-d3a7-4dea-a9ff-82dc04af0c25.png)

### Spawn Box
```c#
	
$m_a1a_goodspickup = new StatePropObject("M_A1A_GoodsPickup");
$maincharacter = FindObject("MainCharacter");
if($m_a1a_goodspickup){
	$m_a1a_goodspickup.position = $maincharacter.position;
	$m_a1a_goodspickup.direction = $maincharacter.direction;
	$m_a1a_goodspickup.roll = "2.9649200";
	$m_a1a_goodspickup.name = "M_A1A_GoodsPickup";
	$m_a1a_goodspickup.scriptClass = "";
	$m_a1a_goodspickup.modelName = "crateGenericA";
	Echo("DBG", "StatePropObject: M_A1A_GoodsPickup new object has been created!");
}
```
![image](https://user-images.githubusercontent.com/44430306/218595589-2ac15369-eb5d-46df-9beb-528a74046291.png)
