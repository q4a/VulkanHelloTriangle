CFLAGS = -std=c++17 -O2
LDFLAGS = -lglfw -lvulkan -ldl -lpthread -lX11 -lXxf86vm -lXrandr -lXi

VulkanTest: main.cpp
	g++ $(CFLAGS) -o VulkanTest.bin main.cpp $(LDFLAGS)

.PHONY: test clean

test: VulkanTest
	./VulkanTest.bin

clean:
	rm -f VulkanTest.bin
