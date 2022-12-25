## <h1 align="center">Fleek Network</h1>
![image](https://user-images.githubusercontent.com/101149671/209468276-05345f01-8643-4a57-8109-77d24ba8f622.png)


### Sistem Gereksinimleri ; 
```
4 CPU
4 RAM
```

# Kuruluma geçelim ; 

```
sudo su
```
```
sudo apt update && sudo apt upgrade
```
```
sudo apt install screen curl tar wget jq build-essential
```
```
sudo apt install make clang pkg-config libssl-dev cmake
```
```
sudo apt install curl build-essential gcc make
```

# rustup'u kuruyoruz:
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
source ~/.profile
source ~/.cargo/env
```

## sccache ve protobufer'i kuruyoruz:
```
cargo install sccache
```
```
sudo apt-get install protobuf-compiler
```

# fleek-network/ursa.git` 'i klonluyoruz.

* `make install` kurulum uzun sürer.
* daha sonra version kontrol ediyoruz: `ursa --version`
* version: `ursa 0.1.0`

```
cd $HOME 
git clone https://github.com/fleek-network/ursa.git
cd ursa
```
```
make install
```

# ursa adlı bir screen oluşturup node çalıştırıyoruz:

* Loglar akması gerekiyor.
* Loglar aktıktan sonra CTRL + A + D ile çıkıyoruz.

```
screen -S ursa
```
```
cd $HOME
cd ursa 
ursa
```
# altta ki dosyayı indirelim ve kontrol edelim:
```
curl https://ipfs.io/ipfs/bafybeidqdywrzg7c3b4dmm332m4b7uiakgitplz2pep2zntederxpj3odi -o basic.car
```
```
ursa rpc put basic.car
```
```
ursa rpc get bafybeifyjj2bjhtxmp235vlfeeiy7sz6rzyx3lervfk3ap2nyn4rggqgei ./output
```
```
ls -hl ./output
```

[image](https://user-images.githubusercontent.com/101149671/209468216-0aa9927c-c28f-4f0d-9423-2cde745a4f63.png)

# Kurulum bu kadar.















