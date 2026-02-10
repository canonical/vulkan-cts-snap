# Vulkan CTS Snap

This snap provides an easy way to install and run the tests found in
[Khronos's Vulkan Conformance Test Suite](https://github.com/KhronosGroup/VK-GL-CTS)

## Build

```
snapcraft pack
```

# Install

```
snap install --dangerous vulkan-cts_1.0_<your_arch>.snap
```

# Run

## List available test caselists
```
vulkan-cts.list-tests
```

## Run tests

Run a specific test case:
```
vulkan-cts.test dEQP-VK.info.build
```

Or run tests from a mustpass caselist:
```
vulkan-cts.test --caselist=mustpass/main/vk-default/api.txt
```
