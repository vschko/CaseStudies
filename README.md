# Case Studies

Write-ups on vulnerabilities I've discovered across iOS and macOS.

| CVE/bug | Summary |
| --- | --- |
| [CVE-2026-84530 (*)](./CVE-2026-84530) | Kernel heap address disclosure through unsanitized AIO kqueue metadata. Fixed in *OS 27. |
| [CVE-2026-43748 (*)](./CVE-2026-43748) | Kernel heap OOB write in the ANE direct path (`ANE_ProgramCheckandPrewireBuffers_gated`). Fixed in *OS 26.6. |
| [CVE-2026-39868 (*)](./CVE-2026-39868/) | XNU/DTrace memory corruption through malformed lazy DOF sections. Fixed in *OS 26.5.2. |
| [CVE-2026-65371 (*)](./CVE-2026-65371) | `gRegistryRoot` KVA disclosure through console-security interest notifications. Fixed in *OS 26.6. |
| [CVE-2026-28827](./CVE-2026-28827/) | macOS sandbox escape through path traversal and unsafe plugin loading in `NetFS.framework`. |
| [AppleM2ScalerCSCDriver IOSurface leak](./no-cve/m2scaler-leak-26.5.2/) | IOSurface KVA and MTE-tag disclosure through an unsanitized diagnostic-log payload. Fixed in *OS 26.6; possibly CVE-2026-64709. |
| [dyld4 protected-stack overflow](./no-cve/dyld-bug-jan2026/) | Protected-stack overflow caused by an excessive chained-fixup bind-target count. Silently fixed in *OS 26.2. |

> Note: An asterisk (*) indicates a vulnerability that I reported to the vendor and for which I received public credit. I also independently discovered several bugs after they had already been fixed in beta releases, so I did not submit reports for them.

