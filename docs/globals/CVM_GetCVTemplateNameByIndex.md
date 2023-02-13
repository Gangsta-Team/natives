# CVM_GetCVTemplateNameByIndex
```c
// 0x004f4e80
string CVM_GetCVTemplateNameByIndex(string cvTemplateRegister, int index)
```
## Description
```
CV Templates:
- character
- boat
- car

```
## Usage examples

```c#
// Print in the console the whole list of character templates.
$idx = 0;
while ($idx < 306)
{
	Echo("DBG", "Template index: " @ $idx @ " | Template name: " @ CVM_GetCVTemplateNameByIndex("character", $idx));
	$idx = $idx + 1;
}
```
