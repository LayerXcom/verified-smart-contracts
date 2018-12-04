# LayerX Internal Workshop
## Build

(mac)
```
brew install automake libtool gmp mpfr pkg-config pandoc maven opam z3
cd erc20/zeppelin
make
```

## kprove
```
.build/k/k-distribution/target/release/k/bin/kprove -v  -d .build/evm-semantics/.build/java -m VERIFICATION --z3-impl-timeout 500 specs/zeppelin-erc20/transfer-success-2-spec.k 
```