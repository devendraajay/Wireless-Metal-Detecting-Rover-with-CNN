Literature Review / Relevant Studies

Conventional metal detection systems primarily rely on Very Low Frequency (VLF) or Pulse Induction (PI) techniques to identify sub-surface metallic objects based on electromagnetic response. However, these techniques are challenged by complex soil conditions and non-metallic interference, and they lack intelligent classification capabilities [1]. Salah and Shabaneh addressed this by designing a cost-effective metal detection system that can be embedded in low-resource environments [2].

To overcome the limitations of traditional detectors, researchers have explored vision-based metal identification. Önal et al. proposed a machine learning approach to classify metallic minerals from image data, achieving promising results on a static dataset [3]. Our project extends this by implementing a CNN model for real-time inference using a downward-facing camera on a mobile rover.

For navigation and autonomous exploration, various sensing technologies like IR, ultrasonic, and LiDAR have been employed. Liu et al. reviewed these methods in indoor mobile robots, highlighting IR and ultrasonic sensors as cost-effective solutions for short-range obstacle detection [4]. Zhao and Li also proposed a robot that uses deep learning for real-time obstacle avoidance in unknown environments [5], demonstrating how AI-driven logic can enhance autonomy in robotic systems.

Deployment of CNNs on embedded platforms has seen progress in recent years. Ahmed and Echi developed a system for real-time object detection using surveillance cameras powered by AI models [6]. Vieira et al. extended this work to embedded devices like Raspberry Pi, showcasing CNN inference for violence recognition using low-power systems [7]. This validates our approach of optimizing CNN models (e.g., ResNet50V2, EfficientNet) for mineral classification on Raspberry Pi or an offloaded system.

While individual works have focused on either metal detection, mineral classification, or autonomous navigation, few have combined all three into a unified mobile system. Our project bridges this gap by integrating terrain exploration, real-time mineral detection, and intelligent navigation into one low-cost embedded platform.

References
M. Šimić, D. Ambruš, and V. Bilas, IEEE Sensors Lett., vol. 7, no. 9, pp. 1–4, 2023.

W. A. Salah and A. A. A. Shabaneh, Bull. Electr. Eng. Inform., vol. 13, no. 5, pp. 3100–3111, 2024.

M. K. Önal, E. Avci, F. Özyurt, and A. Orhan, Proc. SIU, pp. 1–4, 2020.

Y. Liu, S. Wang, Y. Xie, T. Xiong, and M. Wu, Sensors, vol. 24, no. 4, Art. 1222, 2024.

D. Zhao and Y.-P. Li, Proc. IEEE IAAI, pp. 166–171, 2020.

A. A. Ahmed and M. Echi, IEEE Access, vol. 9, pp. 63283–63293, 2021.

J. C. Vieira et al., IEEE Access, vol. 10, pp. 25190–25202, 2022.
