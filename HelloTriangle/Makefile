CFLAGS = -std=c++17 -O2
LDFLAGS = -lglfw -lvulkan -ldl -lpthread -lX11 -lXxf86vm -lXrandr -lXi

HelloTriangle: HelloTriangle.cc
	g++ $(CFLAGS) -o HelloTriangle.bin HelloTriangle.cc $(LDFLAGS)

.PHONY: test clean

test: HelloTriangle
	./HelloTriangle.bin

clean:
	rm -f HelloTriangle.bin
