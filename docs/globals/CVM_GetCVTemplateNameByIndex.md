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

There is a third CV Template but that has been lost...
While shipping the release.

And if none of that matches a default template return value is getting returned.
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
