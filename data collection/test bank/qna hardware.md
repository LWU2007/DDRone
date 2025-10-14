MULTIPLE CHOICE QUESTION

Which of the following hardware components is most commonly used to accelerate deep learning training?
 - A. Central Processing Unit (CPU)
 - B. Graphics Processing Unit (GPU)
 - C. Hard Disk Drive (HDD)
 - D. Sound Card
- ✅ Correct Answer: B. GPU
 Explanation: GPUs are massively parallel processors that handle the large matrix multiplications and tensor operations required for deep learning more efficiently than CPUs.

Why are GPUs better than CPUs for training neural networks?
 - A. GPUs have larger hard drives
 - B. GPUs use less power than CPUs
 - C. GPUs have thousands of cores optimized for parallel computation
 - D. GPUs run at higher clock speeds than CPUs
- ✅ Correct Answer: C. GPUs have thousands of cores optimized for parallel computation
 Explanation: Neural network operations (like matrix multiplications) can be broken into many parallel tasks, which GPUs handle more effectively due to their highly parallel architecture.

Why is AI acceleration/Deep learning known as ‘embarrassingly parallel'?
 - I. Because little or no effort is needed to split the problem into a number of parallel tasks.
 - II. Because GPUs are positioned parallel to the motherboard
 - III. GPUs have thousands of cores optimized for parallel computation
	- A. I, III
 	- B. I, II
 	- C. I
 	- D. I, II, III
- ✅ Correct Answer: C. GPUs have thousands of cores optimized for parallel computation
 Explanation: Neural network operations (like matrix multiplications) can be broken into many parallel tasks, which GPUs handle more effectively due to their highly parallel architecture.

Which of the following best describes the role of high-bandwidth memory (HBM) in AI accelerators?
 - A. It replaces the GPU cores for faster computation
 - B. It provides very fast data transfer between memory and compute units
 - C. It acts as permanent storage for trained models
 - D. It controls data center cooling systems
- ✅ Correct Answer: B. It provides very fast data transfer between memory and compute units Explanation: HBM is placed close to the processor die to minimize latency and maximize bandwidth, enabling faster feeding of data to GPUs or TPUs

Which interconnect technology is commonly used to link multiple GPUs together in large AI training clusters to minimize communication bottlenecks?
 - A. PCIe Gen 2
 - B. NVLink
 - C. SATA
 - D. Thunderbolt
- ✅ Correct Answer: B. NVLink
 Explanation: NVLink (developed by NVIDIA) offers much higher bandwidth than PCIe, allowing multiple GPUs to share memory and communicate quickly, which is critical for scaling training across many devices.
 
When using many GPUs together to train a large AI model, what is one common problem that can slow training down?
 - A. The GPUs run out of power instantly
 - B. Data transfer between GPUs can become slower and take more time
 - C. The GPUs stop working after a few hours
 - D. The model automatically finishes training faster
- ✅ Correct Answer: B. Data transfer between GPUs can become slower and take more time
 Explanation: When many GPUs are used together, sending data back and forth between them can become a bottleneck if communication isn’t fast enough.
 
Why do companies use special AI chips like TPUs or advanced GPUs like the H100 for large AI projects?
 - A. Because they look cooler
 - B. Because they are slower but easier to use
 - C. Because they are designed to handle AI tasks faster and more efficiently
 - D. Because they are the only chips that can connect to the internet
- ✅ Correct Answer: C. Because they are designed to handle AI tasks faster and more efficiently
 Explanation: Custom AI chips have special designs that speed up training and save energy, which is useful for very large models.


TRUE OR FALSE

Statement: GPUs are widely used in AI because they can process many operations in parallel.
✅ Answer: True
Explanation: Parallelism is the main reason GPUs accelerate deep learning — they can handle thousands of simultaneous operations efficiently.

Statement: CPUs are generally faster than GPUs for training deep neural networks.
✅ Answer: False
Explanation: While CPUs are better for general tasks, GPUs significantly outperform them in parallelized mathematical operations common in neural network training.

Statement: High-bandwidth memory (HBM) helps reduce data transfer bottlenecks between the processor and memory in AI accelerators.
✅ Answer: True
Explanation: HBM provides very high data throughput, which is essential for feeding data to GPU/TPU cores without slowing computation.

Statement: ASIC-based AI accelerators can be reprogrammed for different neural network architectures easily.
✅ Answer: False
Explanation: Unlike FPGAs or GPUs, ASICs are hardwired for specific tasks, so they are extremely efficient but not easily reprogrammable.

Statement: Scaling AI training across multiple accelerators is mostly limited by computation power, not communication bandwidth.
✅ Answer: False
Explanation: As systems scale, communication and synchronization overhead (e.g., gradient exchange) often becomes the primary bottleneck, not raw compute power.

When many GPUs are used together, moving data between them can become a problem that slows down training.
✅ Answer: True
Explanation: Communication between devices can become a bottleneck if not managed efficiently.

Special AI chips like TPUs are built to make AI training faster and use less energy compared to regular GPUs.
✅ Answer: True
Explanation: TPUs and similar accelerators are optimized specifically for AI operations, making them more efficient for large-scale workloads.


OPEN-ENDED QUESTIONS

1. 
Question:
 Explain why using multiple GPUs or AI accelerators can speed up training for large models, and describe one challenge that arises when scaling to many devices.
Expected Points to Cover:

- Multiple GPUs can split large datasets or model layers, allowing parallel processing → faster training

- However, challenges include communication overhead, synchronization delays, or data transfer bottlenecks between devices



2. 
Question:
 Compare the roles of GPUs and specialized accelerators (like TPUs or ASICs) in large-scale AI systems. What are the advantages and trade-offs of each?
Expected Points to Cover:
- GPUs: flexible, programmable, widely available, good for both training & research

- TPUs/ASICs: faster and more energy-efficient for specific tasks, but less flexible and usually designed for large data centers

- Trade-offs between flexibility vs. efficiency and cost
