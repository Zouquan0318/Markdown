classDiagram
	class tools owner {
	tools configuration
	user manual
	}
	class Test platform development { 
	local configuration
	acceptance test log
	}
	class product owner {
	solution deliver plan
	}
	Test platform development "1" <--o "*" tools owner: fetch
  Test platform development "1" <--o "*" product owner: fetch
  product owner "1" <--o "*" Test platform development: transfer
