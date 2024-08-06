sequenceDiagram
    participant A as Artifactory management
    participant R as Resource management
    participant C as CICD workflow
    participant T as Test automation system

    A->>C: Test environment initial by test plan and test
    C->>C: Manual test or Automatic test start
    C->>T: Test Job deploy
        par
        T->>R: Test status feedback
    END
    T->>T: TA execution
    T->>C: TA log feedbak
    C->>A: Test log synchronization
    C->>A: Test result synchronization
