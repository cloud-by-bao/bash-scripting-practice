# Day 1: File & Directory Automation

## 📌 Overview
This project is part of my **Bash Scripting Practice Series**.  
The goal was to practice **basic file automation** in Bash by simulating a real-world DevOps task: generating logs and archiving them into a backup directory.

---

## 🛠️ What the Script Does
1. Creates 3 directories: `logs`, `backups`, and `reports`.  
2. Generates 5 timestamped text files inside the `logs/` directory.  
3. Writes a unique message into each file (simulating log entries).  
4. Moves the files into the `backups/` folder (simulating log rotation/archiving).  
5. Prints progress messages to the console for visibility.

---

## ▶️ How to Run
```bash
# Make script executable
chmod +x day1.sh

# Run the script
./day1.sh

# Check that files moved to backups/
ls backups

