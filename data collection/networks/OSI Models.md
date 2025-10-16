The OSI Model is a framework outlining how different components of a network should interact and function together. This enables different operating systems to still communicate with one another, thus bypassing the issue of differing internal architectures. This model helps ensure that all parts of a network coordinate effectively.

The OSI Model was developed by the International Organisation for Standardisation.

The  framework is structured into 7 layers that each outline how network components should interact. These layers are:

- Physical: Handles the physical connection and transmission of data (ie, network cables)

This layer transmits raw bits over a physical medium, as well as defining hardware specifications to ensure proper data transfer

- Data link: Manages the connection between devices and error detection

Organises bits into frames, adds addressing information, and ensures error checking for reliable node to node communication

- Network: Responsible for data routing and addressing

Manages packet delivery across networks, using logical addresses (such as IP addresses) that remain constant, while physical addresses can change at different nodes

- Transport: Ensures reliable data transfer and error recovery

Oversees end-to-end message delivery, breaking messages into packets, ensuring they arrive in order, and retransmitting lost packets

- Session: Controls sessions between applications

controls communication sessions, maintaining synchronisation whilst allowing recovery from failures by setting synchronisation points

- Presentation: Translates data formats for the application layer

Handles data format translation, compression and encryption/decryption for security. Note that these functions are often integrated into other layers in modern networks

- Application: Interfaces with end-user applications

facilitates user access to network services, enabling various applications that support communication and resource sharing

Devices in a network may utilise and implement one or more layers based on the layer's function. When data is sent, it passes through these layers, with headers and trailers being added for control. At the receiving end, these are stripped away as the data is processed back to the application layer.