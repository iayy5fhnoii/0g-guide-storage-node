# 0g-guide-storage-node

![0G-bg-3](https://github.com/user-attachments/assets/450eb1ed-57df-4d01-a93f-feb8aff836c5)

## Hardware Requirements
|Key|Value|
|:--|:----|
|**RAM**|16 GB RAM|
|**CPU**|4 cores|
|**DISK**|500GB / 1T NVME SSD|
|**BANDWIDTH**|500 MBps for Download / Upload|

# Installation
## Clone the Sorce Code
```bash
git clone https://github.com/0glabs/0g-storage-client.git
```

## Bild the Source Code
```bash
cd 0g-storage-client
go build
```

## Run the file upload/download commands
```bash
# file upload
./0g-storage-client upload --url <blockchain_rpc_endpoint> --contract <log_contract_address> --key <private_key> --node <storage_node_rpc_endpoint> --file <file_path>
# file download
./0g-storage-client download --node <storage_node_rpc_endpoint> --root <file_root_hash> --file <output_file_path>
# file download with verfication
./0g-storage-client download --node <storage_node_rpc_endpoint> --root <file_root_hash> --file <output_file_path> --proof
```
