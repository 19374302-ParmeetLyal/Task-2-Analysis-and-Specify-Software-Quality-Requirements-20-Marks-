# Task-2-Analysis-and-Specify-Software-Quality-Requirements-20-Marks-

My allocation of responsibility is the development of the UniDorm Student Subsystem. The function requirement I selected is FR-ST-2.1 (Digital Key Access).

# Security and Privacy protection
Digital key transmission such as bluetooth, Wi-Fi, NFC, must be encrypted in order to prevent cloning, inception and replay attacks. Therefore, the app has to require a secure PIN or biometric authentication. Data of which doors students open etc, must also be made as anonymous as possible and access controlled.

# Performance
The time taken to disengage the physical lock once a student activates a digital key should not take longer than 2 seconds under normal conditions. The payload size must also be minimal. The token validation payload between the cloud API and the app must be less than 4KB per transaction in order to reduce network traffic and the latency. The Physical lock controller must have an Access Point Capacity high enough to support multiple sequential lock requests per minute without any buffer overflow. 

# Reliability
The digital key should always be available as unavailability would result in students being locked out. Due to this, the system should implement a failover such as an encrypted access token so that if a digital transmission system fails, students will still have access.

# Scalability
The API gateway and authenticator should be able to process thousands of unlock requests with no performance degradation. In the morning when students leave for lectures at the same time, the peak load handling must be able to process a baseline peak.


