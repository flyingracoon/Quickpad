#NoEnv  ; Recommended for performance and compatibility with future AutoHotkey releases.
#Warn  ; Enable warnings to assist with detecting common errors.
SendMode Input  ; Recommended for new scripts due to its superior speed and reliability.
SetWorkingDir %A_ScriptDir%  ; Ensures a consistent starting directory.

CapsLock::return

CapsLock & i::
	If (GetKeyState("Control", "P") && GetKeyState("Shift", "P"))
		send +^{UP}
 	Else If GetKeyState("Shift", "P")
		send +{UP}
	Else If GetKeyState("Control", "P")
		send ^{UP}
	Else If GetKeyState("LAlt", "P")
		send !{UP}
	Else
		send {UP}
return
CapsLock & j::
	If (GetKeyState("Control", "P") && GetKeyState("Shift", "P"))
		send +^{LEFT}
 	Else If GetKeyState("Shift", "P")
		send +{LEFT}
	Else If GetKeyState("Control", "P")
		send ^{LEFT}
	Else If GetKeyState("LAlt", "P")
		send !{LEFT}
	Else
		send {LEFT}
return
CapsLock & k::
	If (GetKeyState("Control", "P") && GetKeyState("Shift", "P"))
		send +^{DOWN}
 	Else If GetKeyState("Shift", "P")
		send +{DOWN}
	Else If GetKeyState("Control", "P")
		send ^{DOWN}
	Else If GetKeyState("LAlt", "P")
		send !{DOWN}
	Else
		send {DOWN}
return
CapsLock & l::
	If (GetKeyState("Control", "P") && GetKeyState("Shift", "P"))
		send +^{RIGHT}
 	Else If GetKeyState("Shift", "P")
		send +{RIGHT}
	Else If GetKeyState("Control", "P")
		send ^{RIGHT}
	Else If GetKeyState("LAlt", "P")
		send !{RIGHT}
	Else
		send {RIGHT}
return

F5::Reload
