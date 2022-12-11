# Aleo-pool
### Connecting to the Haruka pool is one of the Maestros of the Aleo project, so in my opinion it will be reliable, but you have to make the decision yourself, you can look for other pools 
## I advise you to run through screen because without it you can be thrown out of the pool after closing the SSH session 
```
screen -S Aleo 
```
## If rust is already installed: Make sure you have at least Rust 1.65. Check with 
```
rustc --version.
```
## Install the latest version of Rust using rustup. Run the following line:
and press the "y" in the second "1"
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
### (If the rast is not updated, try to exit and enter the terminal again) 
## On Debian / Ubuntu, running the following command should be enough:
```
sudo apt update
sudo apt install git clang libssl-dev pkg-config --no-install-recommends
```
## Clone the prover repo:
```
git clone https://github.com/HarukaMa/aleo-prover -b testnet3-new
cd aleo-prover
```
## Build the prover using cargo:
```
cargo build --release
```
## If the build successes, Run the prover:
### "aleo1your_address_here" - Your wallet address aleo 
```
cargo run --release -- -a aleo1your_address_here -p pool.hamp.app:4444
```

![Screenshot_1](https://user-images.githubusercontent.com/110123270/206908893-3788e965-c3c5-40c5-9f60-eb823a3f1639.png)
##If you see something like this, then you have successfully joined the pool. 

