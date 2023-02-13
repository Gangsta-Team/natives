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
