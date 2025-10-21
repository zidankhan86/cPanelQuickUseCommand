# cPanel Terminal Cheatsheet

## 1. Navigation & File Management
| Command | Use |
|---------|-----|
| `pwd` | Show current directory path |
| `ls -la` | List all files (including hidden ones like `.env`) |
| `cd folder_name` | Change directory |
| `cd ..` | Go up one directory |
| `mkdir folder_name` | Create a new folder |
| `rm file_name` | Delete a file |
| `rm -rf folder_name` | Delete a folder and all contents (use with caution!) |
| `cp file_name destination` | Copy file |
| `mv old_name new_name` | Rename or move a file |

## 2. Editing Files
| Command | Use |
|---------|-----|
| `nano file_name` | Open file in nano editor |
| `vim file_name` | Open file in vim editor |
| `cat file_name` | View file content in terminal |
| `less file_name` | View file content with scroll support |

## 3. Permissions & Ownership
| Command | Use |
|---------|-----|
| `chmod 755 file_or_folder` | Change permissions (read/write/execute) |
| `chmod 644 file_name` | Common permissions for files |
| `chown user:user file_or_folder` | Change file/folder ownership |

## 4. Laravel Specific
| Command | Use |
|---------|-----|
| `php artisan serve` | Start Laravel development server (mostly local) |
| `php artisan config:clear` | Clear config cache |
| `php artisan cache:clear` | Clear application cache |
| `php artisan config:cache` | Cache config files for performance |
| `php artisan route:list` | List all routes |
| `php artisan migrate` | Run database migrations |
| `php artisan migrate:rollback` | Rollback last migration |

## 5. Git Commands (If using Git in cPanel)
| Command | Use |
|---------|-----|
| `git status` | Check git status |
| `git pull` | Pull latest changes from remote repo |
| `git add .` | Stage changes |
| `git commit -m "message"` | Commit changes |
| `git push` | Push changes to remote repo |

## 6. Searching & Monitoring
| Command | Use |
|---------|-----|
| `grep "text" file_name` | Search for text in a file |
| `tail -f file_name` | Monitor file in real-time (like logs) |
| `top` | View running processes |
| `df -h` | Check disk space usage |
| `du -sh folder_name` | Check folder size |

## 7. Backup & Copy
| Command | Use |
|---------|-----|
| `cp .env .env.backup` | Backup your `.env` file |
| `tar -czvf backup.tar.gz folder_name` | Create compressed backup of folder |
| `tar -xzvf backup.tar.gz` | Extract backup |