# pathlib - Object-oriented filesystem paths

## References

- [pathlib documentation](https://docs.python.org/3/library/pathlib.html)
- [PEP 428 : pathlib specification](https://peps.python.org/pep-0428/)

## Interesting blog articles

### Python pathlib Cookbook

- [Python pathlib Cookbook](https://miguendes.me/python-pathlib)

[os](https://docs.python.org/3/library/os.html) / [os.path](https://docs.python.org/3/library/os.path.html) 
provides several functions that manipulate paths represented as plain Python
strings.

Representing paths as strings encourages inexperienced Python developers to
perform common path operations using string method. For example, joining paths
with `+` instead of using `os.path.join()`, which can lead to subtle bugs and
make the code hard to reuse across multiple platforms.

Moreover, if you want the path operations to be platform agnostic, you will
need multiple calls to various os functions such as `os.path.dirname()`,
`os.path.basename()`, and others.

### The Right Way to Run Shell Commands From Python

- [The Right Way to Run Shell Commands From Python](https://martinheinz.dev/blog/98)

If you need to create or delete file/directory; check if file exists; change
permissions; etc., there's absolutely no reason to run system commands, just
use pathlib, it has everything you need. When you start using pathlib, you will
also realise that you can forget about other Python modules, such as `glob`, or
`os.path`.

