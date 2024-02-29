# lsp-tree-sitter

[![readthedocs](https://shields.io/readthedocs/lsp-tree-sitter)](https://lsp-tree-sitter.readthedocs.io)
[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neomutt/lsp-tree-sitter/main.svg)](https://results.pre-commit.ci/latest/github/neomutt/lsp-tree-sitter/main)
[![github/workflow](https://github.com/neomutt/lsp-tree-sitter/actions/workflows/main.yml/badge.svg)](https://github.com/neomutt/lsp-tree-sitter/actions)
[![codecov](https://codecov.io/gh/neomutt/lsp-tree-sitter/branch/main/graph/badge.svg)](https://codecov.io/gh/neomutt/lsp-tree-sitter)
[![DeepSource](https://deepsource.io/gh/neomutt/lsp-tree-sitter.svg/?show_trend=true)](https://deepsource.io/gh/neomutt/lsp-tree-sitter)

[![github/downloads](https://shields.io/github/downloads/neomutt/lsp-tree-sitter/total)](https://github.com/neomutt/lsp-tree-sitter/releases)
[![github/downloads/latest](https://shields.io/github/downloads/neomutt/lsp-tree-sitter/latest/total)](https://github.com/neomutt/lsp-tree-sitter/releases/latest)
[![github/issues](https://shields.io/github/issues/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/issues)
[![github/issues-closed](https://shields.io/github/issues-closed/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/issues?q=is%3Aissue+is%3Aclosed)
[![github/issues-pr](https://shields.io/github/issues-pr/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/pulls)
[![github/issues-pr-closed](https://shields.io/github/issues-pr-closed/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/pulls?q=is%3Apr+is%3Aclosed)
[![github/discussions](https://shields.io/github/discussions/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/discussions)
[![github/milestones](https://shields.io/github/milestones/all/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/milestones)
[![github/forks](https://shields.io/github/forks/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/network/members)
[![github/stars](https://shields.io/github/stars/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/stargazers)
[![github/watchers](https://shields.io/github/watchers/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/watchers)
[![github/contributors](https://shields.io/github/contributors/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/graphs/contributors)
[![github/commit-activity](https://shields.io/github/commit-activity/w/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/graphs/commit-activity)
[![github/last-commit](https://shields.io/github/last-commit/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/commits)
[![github/release-date](https://shields.io/github/release-date/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/releases/latest)

[![github/license](https://shields.io/github/license/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter/blob/main/LICENSE)
[![github/languages](https://shields.io/github/languages/count/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter)
[![github/languages/top](https://shields.io/github/languages/top/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter)
[![github/directory-file-count](https://shields.io/github/directory-file-count/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter)
[![github/code-size](https://shields.io/github/languages/code-size/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter)
[![github/repo-size](https://shields.io/github/repo-size/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter)
[![github/v](https://shields.io/github/v/release/neomutt/lsp-tree-sitter)](https://github.com/neomutt/lsp-tree-sitter)

[![pypi/status](https://shields.io/pypi/status/lsp-tree-sitter)](https://pypi.org/project/lsp-tree-sitter/#description)
[![pypi/v](https://shields.io/pypi/v/lsp-tree-sitter)](https://pypi.org/project/lsp-tree-sitter/#history)
[![pypi/downloads](https://shields.io/pypi/dd/lsp-tree-sitter)](https://pypi.org/project/lsp-tree-sitter/#files)
[![pypi/format](https://shields.io/pypi/format/lsp-tree-sitter)](https://pypi.org/project/lsp-tree-sitter/#files)
[![pypi/implementation](https://shields.io/pypi/implementation/lsp-tree-sitter)](https://pypi.org/project/lsp-tree-sitter/#files)
[![pypi/pyversions](https://shields.io/pypi/pyversions/lsp-tree-sitter)](https://pypi.org/project/lsp-tree-sitter/#files)

A core library to support language servers.

I write many language servers and they share some same code so I extract the
shared code to this library.

I've had enough of writing many DSLs in my editor without any LSP support
(completion, hover, ...). So I decide to sacrifice my time to do this work.

## Language servers

- [termux-language-server](https://github.com/termux/termux-language-server/):
  for some specific bash scripts:
  - [`build.sh`](https://github.com/termux/termux-packages/wiki/Creating-new-package)
  - [`PKGBUILD`](https://wiki.archlinux.org/title/PKGBUILD)
  - [`*.ebuild`](https://dev.gentoo.org/~zmedico/portage/doc/man/ebuild.5.html)
  - ...
- [mutt-language-server](https://github.com/neomutt/mutt-language-server):
  for [(neo)mutt](https://github.com/neomutt/neomutt)'s (neo)muttrc
- [More](https://github.com/Freed-Wu?tab=repositories&q=lsp-server)

## What does this library provide

### Schema

A `Trie` to convert a file to a json, then you can use json schema to validate
it to get diagnostics.

Take
[termux-language-server](https://github.com/termux/termux-language-server/) as
an example.

`PKGBUILD`:

```sh
pkgname=hello
pkgver=0.0.1
pkgrel=1
pkgdesc="hello"
arch=(wrong_arch)
license=(GPL3)

build() {
    cat <<EOF > hello
#!/usr/bin/env sh
echo hello
EOF
}

package() {
    install -D hello -t $pkgdir/usr/bin
}
```

```sh
termux-language-server --convert PKGBUILD
```

```json
{
  "pkgname": "hello",
  "pkgver": "0.0.1",
  "pkgrel": "1",
  "pkgdesc": "hello",
  "arch": [
    "wrong_arch"
  ],
  "license": [
    "GPL3"
  ],
  "build": 0,
  "package": 0
}
```

So, we can validate the json by [a json schema](https://github.com/termux/termux-language-server/tree/main/src/termux_language_server/assets/json):

<!-- markdownlint-disable MD013 -->

```sh
$ termux-language-server --check PKGBUILD
PKGBUILD:5:7-5:17:error: 'wrong_arch' is not one of ['any', 'pentium4', 'i486', 'i686', 'x86_64', 'x86_64_v3', 'arm', 'armv6h', 'armv7h', 'armv8', 'aarch64']
```

<!-- markdownlint-enable MD013 -->

![PKGBUILD](https://github.com/neomutt/lsp-tree-sitter/assets/32936898/58614996-bd8a-4e27-b573-87346c82ea2a)

Sometimes it will be more complicated:

`neomuttrc`:

```neomuttrc
set allow_ansi=yes sleep_time = no ispell = aspell
set query_command = 'mutt_ldap_query.pl %s'
```

```sh
mutt-language-server --convert neomuttrc
```

```json
{
  "set": {
    "allow_ansi": "yes",
    "sleep_time": "no",
    "ispell": "aspell",
    "query_command": "mutt_ldap_query.pl %s"
  }
}
```

```sh
$ mutt-language-server --check neomuttrc
neomuttrc:1:33-1:35:error: 'no' is not of type 'number'
```

![neomuttrc](https://github.com/neomutt/lsp-tree-sitter/assets/32936898/75ebf0c1-784a-43db-ae11-59783af57b4f)

We put the result to the json's `.set` not `.` just in order to reserve the
other keys for other usages.

### Finders

Some finders to find the required node in tree-sitter's AST.
Such as, if you want to get the node under the cursor:

```python
@self.feature(TEXT_DOCUMENT_COMPLETION)
def completions(params: CompletionParams) -> CompletionList:
    document = self.workspace.get_document(params.text_document.uri)
    uni = PositionFinder(params.position, right_equal=True).find(
        document.uri, self.trees[document.uri]
    )
    # ...
```

UNI (Universal Node Identifier) is URI + node.

### Utilities

This library also provides many utility functions. Such as converting man page to
markdown and tokenizing it in order to generate the json schema.

```sh
mutt-language-server --generate-schema neomuttrc
```

<!-- markdownlint-disable MD013 -->

````json
{
  "$id": "https://github.com/neomutt/mutt-language-server/blob/main/src/termux_language_server/assets/json/neomuttrc.json",
  "$schema": "http://json-schema.org/draft-07/schema#",
  "$comment": "Don't edit this file directly! It is generated by `mutt-language-server --generate-schema=neomuttrc`.",
  "type": "object",
  "properties": {
    "account-hook": {
      "description": "```neomuttrc\naccount-hook regex command\n```\nThis hook is executed whenever you access a remote mailbox. Useful to adjust configuration settings to different IMAP or POP servers."
    },
    "$comment": "..."
  }
}
````

<!-- markdownlint-enable MD013 -->

![hover](https://github.com/neomutt/lsp-tree-sitter/assets/32936898/22a0347e-3d4f-45c5-833b-e89225ce3b74)

## References

- some [Chinese blogs](https://freed-wu.github.io/tag/lsp/) about how I write
  these language servers
- [tree-sitter](https://tree-sitter.github.io/tree-sitter/)
- [language server protocol](https://microsoft.github.io/language-server-protocol/specifications/specification-current)
- [json schema](https://json-schema.org/specification)
