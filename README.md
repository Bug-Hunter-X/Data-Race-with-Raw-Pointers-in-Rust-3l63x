# Data Race with Raw Pointers in Rust
This repository demonstrates a simple example of a data race in Rust using raw pointers. Data races occur when multiple threads access the same memory location concurrently, without proper synchronization mechanisms. This can lead to unpredictable behavior and crashes. 

**Bug:** The `bug.rs` file contains a program that modifies a vector using a raw pointer without any safeguards.  This is unsafe and can lead to a data race if used in a multi-threaded context.

**Solution:** The `bugSolution.rs` file provides a safe solution that avoids data races by using proper Rust ownership and borrowing mechanisms.

This example highlights the importance of understanding memory management and concurrency in Rust.  Always prioritize safe and predictable code over potentially unsafe techniques.