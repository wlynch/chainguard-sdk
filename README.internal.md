# SDK Release

Contents in this directory will be exported to the public sdk directory.

## Workflow

```mermaid
sequenceDiagram
    participant mono
    participant sdk-staging as sdk-staging<br/>PRIVATE
    participant sdk as sdk<br/>PUBLIC
    mono->>sdk-staging: Open PR
    sdk-staging->>sdk-staging: Human approve PR
    sdk-staging->>sdk: Push main
```
