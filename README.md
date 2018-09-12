cd $ZEPHYR_BASE/samples/net/wifi_scan
mkdir build && cd build

# On Windows
cd %ZEPHYR_BASE%\samples\net\wifi_scan
mkdir build & cd build


# Use cmake to configure a Ninja-based build system:
cmake -GNinja -DBOARD=disco_l475_iot1 ..

# Now run ninja on the generated build system:
ninja
ninja flash
