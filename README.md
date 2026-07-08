# installation_hints
Here one can find hints to compile/install different software  
In case I have fork to any widely used software, I'll use this fork in the examples.  
In the examples I'll use my environment (filesystem username, etc.)  
  
## Install Qt keychain  
  
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
