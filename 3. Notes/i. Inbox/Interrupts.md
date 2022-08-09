zSeries is interrupt-driven, not [[polling]] based
- When I/O is started, the channel takes responsibility
- When I/O completes, an I/O interrupt is generated
- One CPU is interrupted and 'fields' the I/O interrupt, marking the waiting job 'ready to run'
  Other types of zSeries interrupts:
- Program interrupt - program abend or [[page fault]]
- [[Machine check interrupt]] - hardware error detected
- External interrupt - timer
- [[Restart interrupt]] - Operator requested restart
- [[SVC interrupt]] - Supervisor Call (a user program requesting services from the MVS operating system)