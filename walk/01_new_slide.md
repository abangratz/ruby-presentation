!SLIDE

# Ruby: WALK

!SLIDE smbullets incremental

# Geschichte

* Erfinder: Yukihiro "matz" Matsumoto (erste Release 1995)
* POLS: Prinzip der "kleinstmöglichen Überraschung"
* "... versuche, Ruby natürlich, nicht einfach zu machen ..."
* Wurzeln in vielen Sprachen (Perl, Smalltalk, Eiffel, Ada, Lisp)
* Massenakzeptanz 2006 - Ruby on Rails

!SLIDE left

# Alles ist ein Objekt #

### Code ###

    @@@ ruby
    5.times do 
      puts "Whee"
    end
    # => nil


	5.class
	# => Fixnum

!SLIDE left

# Flexibilität #

    @@@ ruby
	class Numeric
		def add(x)
			self + x
		end
	end
	# => nil

	5.add(6)
	# => 11

!SLIDE bullets

# Vererbung #

* Keine Mehrfachvererbung
* aber
* "Auslagern" von Code in Module (Mixins)

!SLIDE bullets

# Blöcke #

## __LISP__ als Vorbild ##


    @@@ ruby
	%w[drei vier fünf].map do |zahlwort|
	  puts zahlwort + " Schritte"
    end
	# drei Schritte
	# vier Schritte
	# fünf Schritte
    # => nil

!SLIDE

# Rubygems: extension repository #

    # gem search -r showoff
	
    *** REMOTE GEMS ***

    goncalossilva-showoff (0.4.3)
    mattmatt-showoff (0.2.3)
    showoff (0.4.2)
    showoff-io (0.3.1)

!SLIDE smbullets 
# Rubygems: PRO#

* Einfaches Handling
* Viele Libraries
* Automatische Abhängigkeiten
* Verschiedene Versionen gleichzeitig 

!SLIDE smbullets 
# Rubygems: CONTRA #
* Source-Code-Intrusiv
* Konflikte mit anderen Paketmanagern
* Keine QA/Best Practices (wie zB CPAN)

