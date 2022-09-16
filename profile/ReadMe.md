fileTestSuite
=============

**We have moved to https://codeberg.org/fileTestSuite**

Under the disguise of "better security" Micro$oft-owned GitHub has [discriminated users of 1FA passwords](https://github.blog/2023-03-09-raising-the-bar-for-software-security-github-2fa-begins-march-13/) while having commercial interest in success of [FIDO 1FA specifications](https://fidoalliance.org/specifications/download/) and [Windows Hello implementation](https://support.microsoft.com/en-us/windows/passkeys-in-windows-301c8944-5ea2-452b-9886-97e4d2ef4422) which [it promotes as a replacement for passwords](https://github.blog/2023-07-12-introducing-passwordless-authentication-on-github-com/). It will result in dire consequencies and is competely inacceptable, [read why](https://codeberg.org/KOLANICH/Fuck-GuanTEEnomo).

If you don't want to participate in harming yourself, it is recommended to follow the lead and migrate somewhere away of GitHub and Micro$oft. Here is [the list of alternatives and rationales to do it](https://github.com/orgs/community/discussions/49869). If they delete the discussion, there are certain well-known places where you can get a copy of it. [Read why you should also leave GitHub](https://codeberg.org/KOLANICH/Fuck-GuanTEEnomo).

---

A spec and a tool that allows you to create unified test suites for data processing software.

Central repo and spec: https://codeberg.org/fileTestSuite/fileTestSuite

Implementations:

* Tier 0: authoring CLI tool, serialization, parsing, testing:
	* [Python](https://codeberg.org/fileTestSuite/fileTestSuite.py)

* Tier 1: serialization, parsing, testing

* Tier 2: parsing, testing:
	* [C++](https://codeberg.org/fileTestSuite/fileTestSuite.c)

* Tier 3: parsing
	* [Kaitai Struct](https://codeberg.org/fileTestSuite/fileTestSuite/tree/master/ksys) - supports `C++`, `C#`, `Go`, `Java`, `JavaScript`, `TypeScript`, `Lua`, `Nim`, `Perl`, `PHP`, `Python`, `Ruby`, `Rust`, `Swift`

* Unimplemented, but needed:
	* Rust

Suites:
* [patch](https://codeberg.org/fileTestSuite/patch.fts)
* [YAML](https://codeberg.org/fileTestSuite/YAML.fts)
* [PKWare `implode` compression](https://codeberg.org/implode-compression-impls/implode_test_files)

Dependencies:
* [TestAbs](https://codeberg.org/fileTestSuite/TestAbs.cpp) - C++ version of FTS relies on it to decouple tests generation from a testing framework
