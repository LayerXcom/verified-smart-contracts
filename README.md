# LayerX Internal Workshop
## Build
```
cd erc20/zeppelin
make
```

## kprove
```
.build/k/k-distribution/target/release/k/bin/kprove -v  -d .build/evm-semantics/.build/java -m VERIFICATION --z3-impl-timeout 500 specs/zeppelin-erc20/transfer-success-2-spec.k 
```