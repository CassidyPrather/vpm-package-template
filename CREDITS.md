# Credits

Third-party and vendored assets. The project's own code is AGPL-3.0-or-later;
see [LICENSE](LICENSE) and the VRChat/Unity linking exception in
[LICENSE_ADDENDUM](LICENSE_ADDENDUM). This file tracks everything that came
from somewhere else.

**The convention:** every asset gets a line here at intake — name, source URL,
author, license, date added. Art, audio, fonts, shaders, vendored packages, all
of it. Thirty seconds now versus archaeology later.

| Asset | Source | Author | License | Added |
| --- | --- | --- | --- | --- |
| `Packages/com.vrchat.core.bootstrap/` | VRChat's package bootstrapper, vendored unmodified from <https://github.com/vrchat-community/template-package> | VRChat | [VRCHAT DISTRO LICENSE FILE](Packages/com.vrchat.core.bootstrap/License.md) | 2026-08 |

The bootstrapper is left byte-for-byte: on first editor open it downloads the
VPM resolver, which in turn installs the SDK, so nothing non-redistributable
ever enters git. Its `License.md` scopes VRChat's terms to that folder alone —
which is exactly why it stays in its own folder.

Assets that cannot be published at all — store purchases, licensed packs — do
not get committed even with a credit line. They ride the private `Assets/Vendor`
submodule (see README → Vendored assets) and still get a row here, license
column included, so the paper trail survives even where the bytes cannot.
