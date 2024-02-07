# FIO_SPDK-GUI-3.0
GUI for Performing FIO Benchmarking using SPDK as IO Engine with 4 SSD's in SSH logged Server

## Features
* Runs FIO benchmark on remote server using SPDK as IO engine
* Supports 4 SSDs
* User-friendly GUI
* Saves output to a file

## Prerequisites
- Python 3.6 or later
- Install Tkinter
- Install paramiko
- SSH client
- SPDK installed with FIO on the remote server
  - You can refer to the following link for installing SPDK with FIO:

https://github.com/ajin412/FIO_SPDK_GUI-2.1.0/blob/main/SPDK_Installation.md

- SPDK NVMe driver binded with all the NVMe drives that we need to benchmark on the remote server.

## How to use
1. Clone the repository to your local machine
2. Open the `FIO_SPDK_GUI-3.0.py` file in terminal
3. Run the program
4. Enter the SSH host, username, and password
5. Select the SPDK path
6. Enter the PCI addresses of the 4 SSDs
7. Enter the size, rw, bs, and iodepth
8. Click the "Run FIO" button to run the benchmark.

## Troubleshooting
If you encounter any problems, please check the following:
- Make sure that the SSH host, username, and password are correct.
- Make sure that the SPDK path is correct.
- Make sure that the PCI address of the disk is correct.
- Make sure that the size, read/write command, block size, and IO depth are valid.
- Make sure that the FIO got installed on the remote server.
- Make sure that the SPDK NVMe driver is binded with all the NVMe drives that we need to benchmark on the remote server.
- You can manually bind the SPDK NVMe driver with the NVMe drives by doing the following:
  - Go to the SPDK directory via terminal.
  - Run the following command:
  
```
sudo ./scripts/setup.sh
```
## Contributing
If you would like to contribute to this project, please fork the repository and submit a pull request.

	

