# zxing-cpp  
  
API to read QR code from C++.  
Environment that shows installation path: CPPUTILS_ZXING_CPP_ROOT  
  
## Keywords  
QR code image reader  
  

## Build on some OSs  
  
### QtKeychain installation on Windows  
```bat  
git clone https://github.com/davitkalantaryan/zxing-cpp.git --recursive 
cd zxing-cpp  
cmake -S . -B build_x64 -A x64 -DCMAKE_INSTALL_PREFIX=D:\davit\install\zxing\x64
cmake --build build_x64 --config Debug --parallel  
cmake --build build_x64 --config Release --parallel  
cmake --install build_x64 --config Debug  
move D:\davit\install\zxing\x64\lib\ZXing.lib D:\davit\install\zxing\x64\lib\ZXingd.lib
cmake --install build_x64 --config Release  
cmake -S . -B build_arm64 -A arm64 -DCMAKE_INSTALL_PREFIX=D:\davit\install\zxing\arm64 
cmake --build build_arm64 --config Debug --parallel  
cmake --build build_arm64 --config Release --parallel  
cmake --install build_arm64 --config Debug  
move D:\davit\install\zxing\arm64\lib\ZXing.lib D:\davit\install\zxing\arm64\lib\ZXingd.lib
cmake --install build_arm64 --config Release  
```  
