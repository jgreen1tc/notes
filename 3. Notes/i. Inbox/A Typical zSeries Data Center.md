![[Screenshot 2022-08-08 11.41.16 AM.png]]
Above shows processors, I/O devices, and network

Each **CPU** consists of up to 16 processors and up to 64 GB memory

The **Channel subsystem** is the key to the zSeries I/O throughput: essentially separate computers that are dedicated to getting data in and out of memory

The **FICON director** allows "hot plugging" of new I/O devices for high availability. It is connected to the CPU via a FICON channel (fast fiber optic cable)

A **Controller** is required for most I/O devices, such as tape and disk ([[DASD]]) drives. Traditionally these were separate units but are now inegrated into large drive arrays such as the IBM RAMAC RAID drive arrays and the EMC Symmetrix DASD

The **35x5 controller** (also called a Front End Processor) may be attached to a channel via older bus and tag cables. This devices is used to interface to an IBM-specific SNA network. SNA networks are rapidly being integrated intp IP networks, rendering the 3745 as a "legacy" device.

The two CPUs are interconnected via a **channel-to-channel (CTC)** connection *and* a FICON connection for connetion to an integrated coupling facility, used in a Parallel SysPlex configuration

The **router** can now be directly connected to the zSeries, using Ethernet. Recent processors support multiple 10 Gigabit Ethernet connections for tremendous network bandwidth.