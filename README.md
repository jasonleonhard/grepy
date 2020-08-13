# Unit Tests

    cargo run tests sample.text

# Run
### cargo run someStringToSearch someFileName

    cargo run the sample.txt # shows 2 matching lines

    cargo run t sample.txt   # shows 4 matching lines

    cargo run \  sample.txt  # match all lines with spaces, in this case all lines except the new line

# Executable from anywhere

    cargo build --release
    cd ~/code/rust/grepy/target/release
    ./grepy run t sample.txt                                # same as # cargo run t sample.txt
    ~/code/rust/grepy/target/release/grepy run t sample.txt # same as # cargo run t sample.txt

so.... just add rust to your path and you can then run from anywhere

# notice current permissions
these are fine and the same as chmod +x grepy
-rwxr-xr-x   2 `whoami`  staff   327K Aug 13 12:54 grepy

    ./grepy com some/path/to/some/file

it will create a binary file

    ./target/release/grepy

This binary is completely self-contained, so you can move or copy it to somewhere else on your computer.

# Run from anywhere
[This is my first rust lang answer on stack overflow](https://stackoverflow.com/questions/60944480/how-do-i-make-a-rust-program-which-can-be-executed-without-using-cargo-run/63403224#63403224)

# publish

    cargo publish

[ref](https://rust-cli.github.io/book/tutorial/packaging.html#quickest-cargo-publish)
