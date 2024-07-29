classDiagram
	class Product Owner {
	Capa list
  Solution development timeline
	}
  class Test Operation { 
  Interface to involved TA tools
  Acceptance test scenario
  }
  class solution vendor {
  SDK for solution
  Source code of access to interface
  }
  Test Platform Development {
  Scripts of test interface
  Solution develiver plan
  TA requirement
  }
	Test Platform Development "1" <--o "*" Product Owner: fetch
  Test Platform Development "1" <--o "*" Test operation: fetch
