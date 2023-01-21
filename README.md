# Moon

**Moon** is a mono inference API for DL models. It powered by tflite or ncnn as optional inference backend, users can using a unique API to do model inference while also able to change different binding backends, by simply specific which backend trait to use in cargo.toml.


Moon is **the next generation base infra** for deeplearning deployment. It still being heavily development.

Goal of moon:

- provide a unified rust inference API, easy to use and intuitive;
- provide Tensor object represents common used high dimentional data, easily extended and debuggable;
- make Tensor in rust able connect with NDArray lib for SIMD for common used Tensor operations;
- link with ncnn c++ lib for inference;
- link with tflite-c for faster inference, possible support for Windows, macOS, Android etc platforms;
- provide a faster way on moving data between NN engine and images, might be a CV package for common operations such as Resize etc.;
  