
# Server Manager CLI Tool

A simple and efficient Bash script for managing a list of servers with automatic logging capabilities.

## Description

`server_manager.sh` is a command-line interface (CLI) tool that allows you to add, list, and remove servers from a centralized list. All operations are automatically logged with timestamps for audit and tracking purposes.

## Features

- ✅ Add servers to your inventory
- ✅ List all registered servers
- ✅ Remove servers from the list
- ✅ Automatic logging of all operations with timestamps
- ✅ Input validation and error handling
- ✅ Simple and intuitive command structure

## Requirements

- Bash shell (Linux/Unix/macOS)
- Basic file system permissions (read/write)

## Installation

1. Clone this repository:
```bash
git clone https://github.com/estebsal/server_manager.sh.git
cd server_manager.sh
```

2. Make the script executable:
```bash
chmod +x server_manager.sh
```

## Usage

### Add a server
```bash
./server_manager.sh add <IP_ADDRESS>
```
Example:
```bash
./server_manager.sh add [IP_ADDRESS]
```

### List all servers
```bash
./server_manager.sh list
```

### Remove a server
```bash
./server_manager.sh remove <IP_ADDRESS>
```
Example:
```bash
./server_manager.sh remove [IP_ADDRESS]
```

### Display help
```bash
./server_manager.sh
```

## Files Generated

- **servers.txt**: Contains the list of all registered servers
- **server_manager.log**: Contains timestamped logs of all operations

## Example Workflow

```bash
# Add multiple servers
./server_manager.sh add [IP_ADDRESS]
./server_manager.sh add [IP_ADDRESS]
./server_manager.sh add [IP_ADDRESS]0.0.5

# List all servers
./server_manager.sh list

# View operation logs
cat server_manager.log

# Remove a server
./server_manager.sh remove [IP_ADDRESS]

# Verify removal
./server_manager.sh list
```

## Log Format

All operations are logged in the following format:
```
[YYYY-MM-DD HH:MM:SS] Operation description
```

Example:
```
[2026-04-06 02:10:15] Servidor agregado: [IP_ADDRESS]
[2026-04-06 02:10:20] Lista de servidores consultada
[2026-04-06 02:10:25] Servidor eliminado: [IP_ADDRESS]
```

## Error Handling

- The script validates that an IP address is provided for add/remove operations
- Checks if the servers file exists before listing or removing
- Provides clear error messages for invalid operations

## Author

**Esteban Salazar** (estebsal)

## Training Context

This script was created as part of **Week 1, Day 5** of DevOps and Systems Developer training, focusing on Bash scripting fundamentals including:
- CLI tool development
- Function creation and reusability
- File handling (read/write operations)
- Logging mechanisms
- Input validation
- Error handling

## License

This project is open source and available for educational purposes.

## Contributing

Feel free to fork this repository and submit pull requests for improvements.

## Support

For questions or issues, please open an issue in the GitHub repository.

---

**Created**: 2026-04-06  
**Last Updated**: 2026-04-06  
**Versio
