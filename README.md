# Python Port Scanner

A fast and efficient port scanner built in Python with service detection and reporting capabilities.

## Features

- Fast port scanning using multi-threading
- Common service detection
- CSV report generation
- Command-line interface
- Progress visualization

## Installation

```bash
# Clone the repository
git clone https://github.com/Jyyoungg/python-port-scanner.git
cd python-port-scanner

# Install requirements
pip install -r requirements.txt
```

## Usage

```bash
# Basic scan
python scanner.py -t 192.168.1.1

# Scan specific port range
python scanner.py -t 192.168.1.1 -p 20-100

# Scan with service detection
python scanner.py -t 192.168.1.1 -s

# Generate report
python scanner.py -t 192.168.1.1 -o report.csv
```

## Options

- `-t, --target`: Target IP address
- `-p, --ports`: Port range (default: 1-1024)
- `-s, --service`: Enable service detection
- `-o, --output`: Output file for report
- `-th, --threads`: Number of threads (default: 50)

## Example Output

```
Port Scanner v1.0
Target: 192.168.1.1
Scanning...

PORT    STATE    SERVICE
21      open     FTP
22      open     SSH
80      open     HTTP
443     open     HTTPS

Scan completed in 2.3 seconds
4 ports found open
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.