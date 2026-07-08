# QT Keychain  
  
### QtKeychain installation on Windows  
```bat  
git clone https://github.com/davitkalantaryan/qtkeychain.git 
cd qtkeychain  
cmake -S . -B build_x64 -A x64 -DCMAKE_PREFIX_PATH=C:\Qt\6.8.3\msvc2022_64 -DCMAKE_INSTALL_PREFIX=D:\davit\install\qtkeychain\x64 -DBUILD_TEST_APPLICATION=OFF  
cmake --build build_x64 --config Debug --parallel  
cmake --build build_x64 --config Release --parallel  
cmake --install build_x64 --config Debug  
cmake --install build_x64 --config Release  
cmake -S . -B build_arm64 -A arm64 -DCMAKE_PREFIX_PATH=C:\Qt\6.8.3\msvc2022_arm64 -DCMAKE_INSTALL_PREFIX=D:\davit\install\qtkeychain\arm64 -DBUILD_TEST_APPLICATION=OFF  
cmake --build build_arm64 --config Debug --parallel  
cmake --build build_arm64 --config Release --parallel  
cmake --install build_arm64 --config Debug  
cmake --install build_arm64 --config Release  
```  
  
### QtKeychain installation on Linux  
```bash  
sudo apt update
sudo apt install -y libsecret-1-dev
git clone https://github.com/davitkalantaryan/qtkeychain.git 
cd qtkeychain
cmake -S . -B build_x64 -DCMAKE_PREFIX_PATH=/home/kalantar/Qt/6.12.0/gcc_64 -DCMAKE_INSTALL_PREFIX=/home/kalantar/install/qtkeychain/x64 -DBUILD_TEST_APPLICATION=OFF
cmake --build build_x64 --config Release --parallel
cmake --install build_x64 --config Release
```  
  
### QtKeychain installation on Macos  
```bash  
git clone https://github.com/davitkalantaryan/qtkeychain.git 
cd qtkeychain
cmake -S . -B build_arm64 -DCMAKE_PREFIX_PATH=/Users/kalantar/Qt/6.12.0/macos -DCMAKE_INSTALL_PREFIX=/Users/kalantar/install/qtkeychain/arm64 -DBUILD_TEST_APPLICATION=OFF
cmake --build build_arm64 --config Release --parallel
cmake --install build_arm64 --config Release
```  
