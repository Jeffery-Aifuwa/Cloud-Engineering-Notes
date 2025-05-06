# Understanding Processes in Computing

A process is simply a program that is currently running on a computer. Think of it like an app you open on your phone—once it starts running, it becomes a process.

## Ways to Run a Process
There are two ways a process can run:

- **Foreground (fg)** – The process runs in front of you, and you interact with it directly.  
  *Example:* Writing a document in a text editor.

- **Background (bg or &)** – The process runs behind the scenes without direct interaction.  
  *Example:* A music player running while you browse the internet.

The very first process that starts when a computer boots up is called `init`, and all other processes come from it.

## Types of Processes
- **Parent Process** – A process that starts (or "spawns") another process.
- **Child Process** – A process that was created by another process (the parent).
- **Orphaned Process** – A child process that loses its parent but keeps running.
- **Zombie Process** – A process that has finished running but still lingers in the system.  
  *Example:* You finish a job but forget to clock out. You’re no longer working, but you’re still on the record.
- **Daemon Process** – A process that runs in the background and performs system tasks (like handling print jobs or monitoring networks).  
  *Example:* Imagine your phone’s alarm app. You’re not using it directly, but it keeps running to alert you at the right time. Similarly, a daemon could be watching for USB devices or handling network traffic.

## Commands to Manage Processes
You can check and manage processes using the following commands:

```bash
ps        # Shows a list of running processes
ps aux    # Displays more detailed information about all processes
ps -ef    # Lists processes from all users with extended details
ps euxf   # Shows processes in a structured tree format
```

## Monitoring and Controlling Processes

```bash
top       # Displays active processes and their resource usage in real time
htop      # A user-friendly version of top with better visuals and interaction
kill      # Terminates a process (useful when a program is unresponsive)
sleep     # Delays for the time specified
```

Understanding processes helps you manage system performance and troubleshoot issues effectively. If you ever find your computer running slow, checking active processes can give you a clue about what’s consuming resources!
