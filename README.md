# Rust Tools apt repo

This is a simple apt repo hosting popular Rust tools which you can access at [apt.0xe.me](https://apt.0xe.me).

The plan is to update the repo when these tools make new releases, so you automatically get the latest and greatest (and don't have to manually install `.deb` files).


### Current packages available

Currently the list is somewhat small, but suggestions are welcome! Feel free to file an issue at https://github.com/ethanhs/apt.0xe.me

- [bat](https://github.com/sharkdp/bat)
- [fd](https://github.com/sharkdp/fd)
- [hexyl](https://github.com/sharkdp/hexyl)
- [lsd](https://github.com/Peltoche/lsd)
- [ripgrep](https://github.com/BurntSushi/ripgrep)

### How to add the repo

```
$ curl -fsSL https://apt.0xe.me/pubkey.asc | sudo apt-key add -
$ curl -fsSL https://apt.0xe.me/rust-tools.list | sudo tee /etc/apt/sources.list.d/rust-tools.list
$ sudo apt update
$ apt show ripgrep
```
