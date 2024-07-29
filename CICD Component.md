sequenceDiagram
    participant I as Integration Cockpit
    participant J as Jenkins Server
    participant T as Test automation system

    I->>J: Test request
    J->>T: Test case execution command
    T->>T: Test case execution
    par
        T->>I: Test status feedback
    END
  
