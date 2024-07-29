classDiagram
	class VSE {
	Interface Control Documents
	Electronic schematic diagram
	}
	class PM {
	GVDP
	#Global vehicle development plan
	}
	class Test Operation {
	Test environment
	#open loop or close loop
	Test requirement
	#test interface, simulator, loader, TA requirements
	}
	class Test Platform Development {
	Test instance building documents(test instance layout, wiring documents, components lists)
	Test instance building plan
	Test instance issue management trace
  	}
	class Supplier {
	test instance building execution
	}
	Test Platform Development "1" <--o "*" VSE: fetch
	Test Platform Development "1" <--o "*" PM: fetch
	PM "1" <--o "*" Test platform development: feedback
	Test Platform Development "1" <--o "*" Test Operation: fetch
	Supplier "1" <--o "*" Test Platform Development: Transfer
