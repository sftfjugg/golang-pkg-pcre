Linux 下有一个 C 实现的 PCRE 库，这个第三方包正是将 PCRE 库应用到 Golang 中。CentOS 下需要先安装 pcre-devel 这个包。

golang-pkg-pcre
===============

This is a Go language package providing Perl-Compatible RegularExpression
support using libpcre++.  Install the package with the current Debian
distribution as follows:

    sudo apt-get install libpcre++-dev
    go get github.com/glenn-brown/golang-pkg-pcre/src/pkg/pcre

Go programs that depend on this package should import this package as
follows to allow automatic downloading:

    import "github.com/glenn-brown/golang-pkg-pcre/src/pkg/pcre"

This is a clone of
[golang-pkg-pcre](http://git.enyo.de/fw/debian/golang-pkg-pcre.git)
by Florian Weimer, which has been placed on github so it can be fetched by
Go's automatic package installer.  The `FindIndex()` and `ReplaceAll()`
functions were added by Glenn Brown, to mimic functions in Go's default
regexp package.
