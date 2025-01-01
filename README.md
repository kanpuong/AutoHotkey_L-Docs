SetCapsLockState "AlwaysOff"

CapsLock::
{
    SetCapsLockState !GetKeyState("CapsLock", "T")
    if GetKeyState("CapsLock", "T")
        Send "{Up}"
}

#HotIf GetKeyState("CapsLock", "T")

i::SendInput "{Up}"
j::SendInput "{Left}"
k::SendInput "{Down}"
l::SendInput "{Right}"
o::SendInput "{PgUp}"
u::SendInput "{PgDn}"
y::SendInput "{Home}"
h::SendInput "{End}"
^i::SendInput "^{Up}"
^j::SendInput "^{Left}"
^k::SendInput "^{Down}"
^l::SendInput "^{Right}"
^o::SendInput "^{PgUp}"
^u::SendInput "^{PgDn}"
^y::SendInput "^{Home}"
^h::SendInput "^{End}"
s::SendInput "{Backspace}"
d::SendInput "^{Backspace}"
Space::
{
    SendInput "{Space}"
    SetCapsLockState "Off"
}
#HotIf
