# Tony Gorez

**Offensive Security Researcher — Apple Platforms**

_Paris, Île-de-France_

<p align="center">
  <a href="mailto:tonygorez@proton.me">mail</a> &nbsp;•&nbsp;
  <a href="https://blog.reversesociety.co" target="_blank">blog.reversesociety.co</a> &nbsp;•&nbsp;
  <a href="https://www.linkedin.com/in/tonygorez" target="_blank">linkedin</a> &nbsp;•&nbsp;
  <a href="https://twitter.com/tonygo_" target="_blank">@tonygo_</a>
</p>

## About

I do vulnerability research and reverse engineering on Apple platforms — macOS and iOS internals, sandbox boundaries, XPC, Mach-O. Credited by Apple for a sandbox escape in App Intents (CVE-2026-28995) and for assistance on WebKit.

Eight years as a systems engineer came first: C, C++ and Objective-C runtimes, native API layers, JavaScript engine internals. That's the part that matters here — I understand the code I'm attacking because I've shipped code exactly like it.

My method is to build the instrument before looking for the answer. When a system is opaque, I write the tool that makes it legible, then publish what it shows me.

## Apple Security Credits

**[CVE-2026-28995](https://support.apple.com/en-us/127110)** — App Intents sandbox escape

> **Impact:** A malicious app may be able to break out of its sandbox
> **Description:** A logic issue was addressed with improved restrictions.
> **Credit:** Vamshi Paili, Tony Gorez (@tonygo_) for Reverse Society

Fixed across [iOS & iPadOS 26.5](https://support.apple.com/en-us/127110), [macOS Tahoe 26.5](https://support.apple.com/en-us/127115), tvOS 26.5, visionOS 26.5, watchOS 26.5 and iOS & iPadOS 18.7.9.

**Apple acknowledgment — WebKit**, [iOS & iPadOS 26.6](https://support.apple.com/en-us/128066) and [macOS Tahoe 26.6](https://support.apple.com/en-us/128067)
Listed under Additional recognition for assistance with WebKit.

## Research & Tooling

**[snixpc](https://github.com/tony-go/snixpc)** — XPC sniffer built on LLDB
Instruments XPC traffic on macOS to make an otherwise opaque IPC surface observable.

**[macho_re](https://github.com/tony-go/macho_re)** — Mach-O parsing library in C
Handles single-architecture and fat (universal) binaries, x86 / x86_64 / ARM / ARM64, dylibs, executables and core dumps, dynamic libraries, and strings resolved to their owning segments and sections. Started as an experiment to learn the format properly rather than read someone else's parser.

**[js-x-ray](https://github.com/NodeSecure/js-x-ray)** (NodeSecure) — JavaScript malware detection
Static analysis of open-source packages. Contributed a suspicious-command probe flagging dangerous `spawn` / `exec` usage.

**[macos-lldb-reverse-engineering](https://github.com/tony-go/macos-lldb-reverse-engineering)** — RE exercise binaries
**[XPCDemo](https://github.com/tony-go/XPCDemo)** · **[TestES](https://github.com/tony-go/TestES)** — XPC and EndpointSecurity experiments
**[antidebug-examples](https://github.com/tony-go/antidebug-examples)** — anti-debugging techniques via fork

## Writing

[**blog.reversesociety.co**](https://blog.reversesociety.co) — macOS and iOS internals through reverse engineering and practical experiment. Publishing since December 2022.

## Toolbox

**Analysis** · Binary Ninja · LLDB · Frida · Instruments
**Languages** · C · C++ · Objective-C · Swift · Rust · TypeScript
**Areas** · Reverse engineering · macOS/iOS internals · Vulnerability research · Static analysis · XPC · Mach-O

## Systems Engineering

The foundation underneath the security work — and what funds it.

**Holepunch** — Systems Engineer, freelance *(2025–present)*
iOS and Android systems work across the [Bare](https://github.com/holepunchto/bare) runtime ecosystem — native modules and platform bindings. Top contributor to [bare-ffmpeg](https://github.com/holepunchto/bare-ffmpeg); also [bare-kit](https://github.com/holepunchto/bare-kit), [bare-sdl](https://github.com/holepunchto/bare-sdl), bare-media, bare-bluetooth and bare-android. This consulting is what funds the research above.

**Postman** — Senior Systems Engineer *(2023–2025)*
Led all Apple platform development (C++, Objective-C, Swift) and shaped cross-OS architecture. Wrapped native Objective-C, Linux and Win32 APIs into a unified C++ layer, then bridged it to JavaScript through JavaScriptCore.

**Node.js** — Collaborator *(2022–present)*
Diagnostics and Single Executable working groups.

**PayFit** — Software Engineer *(2020–2021)*
Built a static analysis service over a payroll DSL used by 100+ engineers — dependency graphs and strongly connected components.

---

<sub>Open to offensive security research roles. Remote.</sub>
