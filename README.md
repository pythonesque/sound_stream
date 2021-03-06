
SoundStream
===========

A simple-as-possible, *fast* audio I/O stream wrapping PortAudio for Rust! It looks like this:

```Rust
for event in stream {
    match event {
        Event::In(input_buffer) => println!("Incoming audio!"),
        Event::Out(output_buffer) => println!("Time to write to output!"),
        Event::Update(delta_time) => println!("Updatey stuff here."),
    }
}
```


Usage
-----

Put this in your Cargo.toml:

```
[dependencies.sound_stream]
git = "https://github.com/RustAudio/sound_stream"
```

For more details, see [the example](https://github.com/RustAudio/sound_stream/blob/master/examples/test.rs).

PortAudio
---------

SoundStream requires that you have the PortAudio lib installed on your system. Download it [here](http://www.portaudio.com/download.html).

License
-------

Same license as [Rust](https://github.com/rust-lang/rust).

