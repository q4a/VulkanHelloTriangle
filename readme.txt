https://github.com/SaschaWillems/Vulkan

https://github.com/krOoze/Hello_Triangle
+ 
https://github.com/google/shaderc or https://github.com/ARM-software/vulkan-sdk

%VULKAN_SDK%/Bin/glslc -mfmt=c -o ./src/shaders/hello_triangle.vert.spv.inl ./src/shaders/hello_triangle.vert
%VULKAN_SDK%/Bin/glslc -mfmt=c -o ./src/shaders/hello_triangle.frag.spv.inl ./src/shaders/hello_triangle.frag
g++ --std=c++14 -Wall -m64 -D_DEBUG -DNO_TODO -I$VULKAN_SDK/include -I./src/ -o./HelloTriangle src/HelloTriangle.cpp -ldl -L$VULKAN_SDK/lib -lvulkan -lglfw

---

amdgpu on rx570:
VulkanTest$ ./VulkanTest
18 extensions supported
VulkanTutorialTriangle$ ./VulkanTutorialTriangle.bin 
validation layers requested, but not available!


---
panfrost on rk3288 with Mali-T760 MP4
VulkanTests ./VulkanTest
