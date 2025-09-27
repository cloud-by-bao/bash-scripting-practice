# Day 1: File & Directory Automation

## 📌 Overview
This script practices **file management and automation** using Bash.  
It simulates a common DevOps task: generating logs and moving them into a backup directory (similar to log rotation and archiving in production).

## 🛠️ Script: `day1.sh`
```bash
#!/bin/bash

echo "📁 Creating directories..."
mkdir -p logs backups reports

echo "📝 Creating 5 log files..."
for i in {1..5}
do
    filename="logs/file_$i_$(date +%Y%m%d%H%M%S).txt"
    echo "This is file $i created on $(date)" > $filename
    echo "Created $filename"
done

echo "📦 Moving files to backups..."
mv logs/*.txt backups/

echo "✅ Task complete! Files moved to backups/"

