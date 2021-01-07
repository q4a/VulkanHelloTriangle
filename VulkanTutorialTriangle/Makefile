CFLAGS = -std=c++17 -O2
LDFLAGS = -lglfw -lvulkan -ldl -lpthread -lX11 -lXxf86vm -lXrandr -lXi

VulkanTutorialTriangle: main.cpp
	g++ $(CFLAGS) -o VulkanTutorialTriangle.bin main.cpp $(LDFLAGS)

.PHONY: test clean

test: VulkanTutorialTriangle
	./VulkanTutorialTriangle.bin

clean:
	rm -f VulkanTutorialTriangle.bin
