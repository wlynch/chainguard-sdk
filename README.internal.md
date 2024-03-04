# SDK Release

Contents in this directory will be exported to the public sdk directory.

Contents are exported to [sdk-staging](https://github.com/chainguard-dev/sdk-staging) first to prevent accidentally exfiltrating mono.

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
