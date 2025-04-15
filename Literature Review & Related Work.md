Literature Review / Relevant Studies

1. Metal Detection Techniques
Conventional metal detection techniques are highly dependent on Very Low Frequency (VLF) or Pulse Induction (PI) techniques. These techniques utilize amplitudes in electromagnetic fields to identify sub-surface metal objects. While they are efficient in uncomplicated environments, these techniques are confronted with challenges in complex soil structures, non-metallic targets, or low-conductivity minerals. Analog metal detection gear is also short of automation and real-time classification features.

Previous research [1][2] has discussed how metal sensors could be integrated with IoT modules for remote monitoring and logging. The systems generally do not use smart classification, and sensor readings are not immune to environmental noise-induced false alarms.

2. Vision-Based Metal Identification
To mitigate VLF/PI limitations, vision-based solutions have been suggested. Image classification methods have been utilized to classify metal types based on surface textures and colors. Deep learning techniques like Convolutional Neural Networks (CNNs) are superior to conventional image processing in classification.

In [3], a CNN model was trained using a metallic mineral dataset and was demonstrated to be capable of performing high accuracy in the copper, iron, and aluminum image classification. The research was restricted to static datasets and did not entail real-time applications on embedded systems.

Our work extends this by capturing photos with a bottom-facing USB webcam on a mobile robot to allow real-time processing with trained CNN models on edge devices.

3. Autonomous Robot Exploration
Autonomous ground robots have been exhaustively researched in search and rescue, agriculture, and exploration contexts. Algorithms such as A* search, frontier-based exploration, and zig-zag traversal have been typically utilized for comprehensive area coverage.

For obstacle detection, studies most frequently employ IR sensors, ultrasonic sensors, or LiDAR. A Raspberry Pi-based robot employed IR and ultrasonic sensing for indoor navigation in unknown environments in [4]. Such systems, however, generally do not incorporate object classification modules.

Our solution combines both: terrain coverage exploration algorithm and CNN-based mineral detection, making it dual-use.

4. CNN + Embedded Inference Systems

Deployment of CNN models on Raspberry Pi under resource-constrained settings has been considered in [5], where authors optimized TensorFlow models with TFLite and minimized inference times. Though suitable for small models, large CNNs need external computation or model pruning.

In our setup, we trade model complexity and performance with a ResNet50V2-based model or EfficientNet, tuned for inference on a laptop (originally), and subsequently ported to the Pi via quantization methods.

5. Limitations of Existing Research While individual metal detection, terrain exploration, and image classification have been discussed in existing studies, few of the systems incorporate all these aspects into a solution. Most of the solutions offered are static (tested on datasets) or employ traditional sensor-based detection methods lacking much intelligence.
