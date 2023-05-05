


我的写法

```rust
fn count_by(x: u32, n: u32) -> Vec<u32> {
    let mut v: Vec<u32> = (1..n+1).collect(); 
    for e in v.iter_mut(){
        *e = *e * x
    }
    v
}
```

```rust
fn count_by(x: u32, n: u32) -> Vec<u32> {
    (1..=n).map(|e| x*e).collect() 
}
```
