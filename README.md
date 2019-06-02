# WinTouch-to-PulseIRLib




You can use this library to play cyclon with any Windows compatible Touchscreen, work with windows8 8.1 and 10

Usage: Backup and Overwrite \cyclon_Data\Plugins\PulseIRLib.dll

Need to modify \Cyclon_Data\Managed\Assembly-CSharp.dll manual 

If using dnSpy, find  "iPhoneToMouse.pos GetTouch(int ID)"  function and delete


    if (GameData.FLIP)
     {
     result.position.x = (float)Screen.width - result.position.x;
     result.position.y = (float)Screen.height - result.position.y;
     }


to bypass MousePositionRotate issues

Known issue: need double click when select mode
