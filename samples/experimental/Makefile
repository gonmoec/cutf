NVCC=nvcc
NVCCFLAGS=-std=c++14 -arch=sm_61 -I../../include
TARGETS=min_exponent.test fp_mask.test reinterpret.test

all: $(TARGETS)

%.test: %.cu
	$(NVCC) $(NVCCFLAGS) -o $@ $<

clean:
	rm -f $(TARGETS)
