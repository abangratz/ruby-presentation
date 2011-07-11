!SLIDE 
# Ruby: RUN #
!SLIDE 
# Ruby VM's im Vergleich #

!SLIDE smbullets incremental

# MRI/YARV#


* älteste Implementation
* Spezifikation/Basis (1.8.7)
* in C geschrieben (sehr sauber)
* Problem: Geschwindigkeit, GC
* Wurde als YARV für 1.9.2 neu implementiert

!SLIDE smbullets incremental

# JRuby #

* komplette Implementation in Java™ VM
* kompatibel mit 1.8.7 und 1.9.2
* schnell
* kann auf alle Java Objekte zugreifen
* kann Objekte zur Laufzeit ändern

!SLIDE smbullets incremental
# Rubinius #

* Neuimplementation
* Ziele: schneller, kein GIL, native Threads
* in C++ und Ruby implementiert
* hat noch Kompatibilitätsprobleme
* schneidet in Benchmarks gut ab

!SLIDE smbullets incremental
# IronRuby #

* Microsoft .NET Framework Implementation
* Läuft auf DLR/CLI
* Limitierte Unterstützung für .NET Klassen


!SLIDE smbullets incremental
# MacRuby #

* Objective-C runtime/CoreFoundation framework
* Basiert auf Ruby 1.9
* LLVM unterstützt AOT und JIT


!SLIDE smbullets incremental
# MagLev #

* GemStone's Smalltalk VM als Basis
* Bytecode to JIT Compiler
* Alpha Test läuft

!SLIDE 

# Zusammenfassung #
