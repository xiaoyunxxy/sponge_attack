# sponge_attack

compile the cuda code: 

`nvcc saxpy.cu -ptx`

As the environment variables are not all set on polyland, please use:

`/usr/local/cuda-12.1/bin/nvcc` 

or (depends on different nodes of polyland)

`/usr/local/cuda-12.2/bin/nvcc` 

# cuda may have different architectures for GPU, to check avaiable arch:
`nvcc --list-gpu-arch`

`nvcc --list-gpu-code`

to compile with a specific arch:


`nvcc x.cu --generate-code arch=compute_50,code=sm_50`
