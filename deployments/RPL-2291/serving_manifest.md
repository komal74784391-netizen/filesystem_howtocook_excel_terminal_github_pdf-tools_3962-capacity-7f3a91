# Standard Serving Replica RPL-2291

One standard serving replica of the Atlas retrieval-augmented QA service.

| Block | Allocation |
| --- | --- |
| weights_store | 320 GB |
| kv_cache_arena | 120 GiB |
| vector_index_map | 40 GB |
| activation_pool | 30 GB |
| telemetry_ring | 10 GB |
| staging_scratch | 8 GB |

Notes:

- Each block is sized from the memory profile in `reference/capacity_profile.csv`.
- Allocation units are quoted exactly as recorded by the platform team.
