# Test Boost and {fmt} with Raspberry Pi

This is a simple project that use Boost Asio and {fmt} on Raspberry Pi 3B+ (Buster 2019-09-26).

## Installing Dependencies
### On the Raspberry Pi:

1. Boost Asio: `sudo apt install libboost-all-dev` (version used: 1.67.0.1).
2. {fmt}: `sudo apt install libfmt-dev'` (version used: 5.2.1+ds-2).
3. Flexbuffers: Download and build Flatbuffers on the Pi itself as the package is not yet available on Buster (version used: 1.11.0).

### On development machine (Windows)

1. Install Visual Studio and Linux workload and the `Embedded and IoT development tools`.

## Notes

1. The Boost Asio requires linking to: `boost_thread`, `boost_system`, `pthread` for a successful build.
2. {fmt} requires linking to: `fmt`.