# ESP32-FreeRTOS-Synchronization-with-Mutex-and-Queues
Overview

This project demonstrates the use of a **FreeRTOS mutex** to protect a shared resource: the serial output (printf / screen).

Two tasks print different messages, and the mutex ensures that the output is never mixed or corrupted.

---

 Key Concepts
- FreeRTOS Tasks
- Mutex (xSemaphoreCreateMutex)
- Task synchronization
- Critical section protection

---
How It Works

- `maTache` prints a French message
- `myTask` prints an English message
- Both tasks share the same output resource
- The mutex `ecranMutex` ensures exclusive access
