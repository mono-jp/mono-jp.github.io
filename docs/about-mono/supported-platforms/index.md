---
title: Supported Platforms
redirect_from:
  - /Supported_Platforms/
  - /Platforms_Supported/
  - /Template%3APlatforms_Supported/
---

Mono has support for both 32 and 64 bit systems on a number of architectures as well as a number of operating systems.

### Supported Operating Systems

**Operating Systems**

-   [Linux](/docs/about-mono/supported-platforms/linux/)
-   [Mac OS X](/docs/about-mono/supported-platforms/osx/), [iOS, tvOS, watchOS](/docs/about-mono/supported-platforms/apple/)
-   [Sun Solaris](/docs/about-mono/supported-platforms/solaris/)
-   [BSD](/docs/about-mono/supported-platforms/bsd/) - OpenBSD, FreeBSD, NetBSD
-   [Microsoft Windows](/docs/getting-started/install/windows/)
-   [Nintendo Wii](/docs/about-mono/supported-platforms/wii/)
-   [Sony PlayStation 3](/docs/about-mono/supported-platforms/playstation3/)
-   [Sony PlayStation 4](/docs/about-mono/supported-platforms/playstation4/)

### Supported Architectures

Mono has both an optimizing just-in-time (JIT) runtime and a interpreter runtime. The interpreter runtime is far less complex and is primarily used in the early stages before a JIT version for that architecture is constructed. The interpreter is not supported on architectures where the JIT has been ported.

|Supported Architectures|Runtime|Operating system|
|:----------------------|:------|:---------------|
|[s390, s390x (32 and 64 bits)](/docs/about-mono/supported-platforms/s390/)|JIT|Linux|
|[SPARC (32)](/docs/about-mono/supported-platforms/sparc/)|JIT|Solaris, Linux|
|[PowerPC](/docs/about-mono/supported-platforms/powerpc/)|JIT|Linux, Mac OSX, Wii, PlayStation 3|
|[x86](/docs/about-mono/supported-platforms/x86/)|JIT|Linux, FreeBSD, OpenBSD, NetBSD, Microsoft Windows, Solaris, OS X, Android|
|[x86-64](/docs/about-mono/supported-platforms/amd64/): AMD64 and EM64T (64 bit)|JIT|Linux, FreeBSD, OpenBSD, Solaris, OS X|
|[IA64](/docs/about-mono/supported-platforms/ia64/) Itanium2 (64 bit)|JIT|Linux|
|[ARM](/docs/about-mono/supported-platforms/arm/): little and big endian|JIT|Linux (both old and new ABI), iPhone, Android|
|Alpha|JIT|**not maintained**. Linux|
|[MIPS](/docs/about-mono/supported-platforms/mips/)|JIT|Linux|
|HPPA|JIT|**not maintained** Linux|

Note that the Alpha, MIPS, ARM big-endian and HPPA architectures are community-supported and may not be as complete as the other architectures.

Support for SPARC64 works in older versions of Mono, but not in the recent versions.

 Packages for most platforms are available from the [Downloads](/download/) page.

### Embedded systems

To make mono more suitable for some architectures used as embedded systems have a look at the [Small footprint](/docs/compiling-mono/small-footprint/) page.
