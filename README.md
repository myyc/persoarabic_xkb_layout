# persoarabic_xkb_layout
An xkb QWERTY phonetic layout to input Arabic and Persian

# Installation
Copy `persoarabic` to `/usr/share/X11/xkb/symbols/`, then edit
`/usr/share/X11/xkb/rules/evdev.xml`, add this after any of the
layouts.

```
    <layout>
      <configItem>
        <name>persoarabic</name>
        <shortDescription>ض</shortDescription>
        <description>Perso-arabic</description>
        <languageList>
          <iso639Id>ara</iso639Id>
          <iso639Id>fas</iso639Id>
        </languageList>
      </configItem>
    </layout>
```

Then restart X by logging out and back in and add the layout 
the way you usually do (GNOME settings or anything else).

# Features

* No IBus or other complicated stuff
* Phonetic. Q key outputs ق, M outputs م and so on
* If you have used the MacOS Arabic QWERTY (best on the market)
  this will be very familiar to you, at least the basics
* There are differences because I did this in an hour and
  I couldn't be bothered to replicate it fully.
* It should include everything, including vocalisation,
  shadda, sukun, آ أ إ ئ ژ etc.
* Vocalisation + shadda / sukun are all triggered by alt plus
  simple letter (a, i, o, u, k, w). I don't like O and K
  but U is crowded right now. Alt+shift for tanwin.
* There is some redundancy (two ways for و, two for ص, etc).
  It's not too bad but it's inefficient. 
  
# TODO

* Very ambitious, but since many QWERTY layouts can be used to
  write many European languages, e.g. the Finnish one can be
  used without issues to type correct French, German, Spanish,
  Italian, Swedish etc.; would be good to push this to the 
  edge and see how many languages one can include (Urdu?
  Kurdish? Uyghur?)
* Some characters might be missing - please let me know!
* If you have any suggestion, also, let me know.
