# `wordwrap`

[![CI](https://github.com/ilius/go-wordwrap/actions/workflows/ci.yml/badge.svg)](https://github.com/ilius/go-wordwrap/actions/workflows/ci.yml)
[![codecov](https://codecov.io/gh/ilius/go-wordwrap/branch/master/graph/badge.svg?token=4SMgf9x2vv)](https://codecov.io/gh/ilius/go-wordwrap)
[![Go Report Card](https://goreportcard.com/badge/github.com/ilius/go-wordwrap)](https://goreportcard.com/report/github.com/ilius/go-wordwrap)
[![Go Reference](https://pkg.go.dev/badge/github.com/ilius/go-wordwrap.svg)](https://pkg.go.dev/github.com/ilius/go-wordwrap)


Wraps words at a given limit. Wraps at whitespace, hyphens (`-`), and will wrap words that exceed
the given limit. See package documentation for more details.

## Example

```go
lines := wordwrap.WordWrap("this test-string has been successfully wrapped successfully", 10)
for _, line := range lines {
	fmt.Println(line)
}
```

### Output

```console
this test-
string has
been
successful
ly wrapped
successful
ly
```
