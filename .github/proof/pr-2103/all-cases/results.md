# PR #2103 all-cases test run

Preview: https://deploy-preview-2103--snapshot-livenet.netlify.app

| Status | Case | Notes |
| --- | --- | --- |
| PASS | Core onchain route defaults Spaces filter to Any and merged list | https://deploy-preview-2103--snapshot-livenet.netlify.app/#/org/arbitrum/arb1:0xf07DeD9dC292157749B6Fd268E37DF6EA38395B9/proposals?login=random |
| PASS | Treasury onchain route also defaults to Any merged list | https://deploy-preview-2103--snapshot-livenet.netlify.app/#/org/arbitrum/arb1:0x789fC99093B09aD01C34DC7251D0C89ce743e5a4/proposals?login=random |
| PASS | Selecting Treasury narrows list and persists query after reload | https://deploy-preview-2103--snapshot-livenet.netlify.app/#/org/arbitrum/arb1:0xf07DeD9dC292157749B6Fd268E37DF6EA38395B9/proposals?login=random&space=0x789fC99093B09aD01C34DC7251D0C89ce743e5a4 |
| PASS | Selecting Core narrows list and updates query | https://deploy-preview-2103--snapshot-livenet.netlify.app/#/org/arbitrum/arb1:0xf07DeD9dC292157749B6Fd268E37DF6EA38395B9/proposals?space=0xf07DeD9dC292157749B6Fd268E37DF6EA38395B9&login=random |
| PASS | Returning to Any clears space query and restores merged list | https://deploy-preview-2103--snapshot-livenet.netlify.app/#/org/arbitrum/arb1:0xf07DeD9dC292157749B6Fd268E37DF6EA38395B9/proposals?login=random |
| PASS | Status Pending filter works across merged list and persists in URL | https://deploy-preview-2103--snapshot-livenet.netlify.app/#/org/arbitrum/arb1:0xf07DeD9dC292157749B6Fd268E37DF6EA38395B9/proposals?login=random&state=pending |
| PASS | New proposal dropdown lists both Arbitrum spaces |  |
| PASS | Offchain Arbitrum route hides Spaces filter | https://deploy-preview-2103--snapshot-livenet.netlify.app/#/org/arbitrum/s:arbitrumfoundation.eth/proposals?login=random |
| PASS | Invalid space query falls back to Any merged list | https://deploy-preview-2103--snapshot-livenet.netlify.app/#/org/arbitrum/arb1:0xf07DeD9dC292157749B6Fd268E37DF6EA38395B9/proposals?login=random |
| SKIP | Labels filter with merged list | Arbitrum onchain spaces on this preview do not render a Labels dropdown, so there is no labels case to exercise. |