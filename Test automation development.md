classDiagram
	class Product Owner {
	Capa list
	Solution development timeline
	}
	class Test Operation { 
	Interface of involved TA tools
	Acceptance test scenario
	}
	class solution vendor {
	SDK for solution
	Source code of access to interface
	}
	class Test Platform Development {
	Scripts of test interface
	Solution develiver plan
	TA requirement
	}
	Test Platform Development "1" <--o "*" Product Owner: fetch
  	Test Platform Development "1" <--o "*" Test Operation: fetch
   	solution vendor "1" <--o "*" Test Platform Development: Capa list
    	Test Platform Development "1" <--o "*" solution vendor: deliver
    	Test Platform Development "1" <--o "*" Product Owner: deliver with PoC
