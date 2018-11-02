## Penn Cloud

Setup Instruction:
In order to successfully run the program, protocol buffer 3.5.0 needs to be installed (and it needs to be 3.5.0), grpc needs to be installed as well, and you need to build from source. For detailed instructions, please check https://github.com/grpc/grpc/blob/master/INSTALL.md .

To compile the program, 
Go to penn-cloud/storage-system/server, type command “make”
Go to penn-cloud/storage-system/client, type command “make”
Go to penn-cloud/Servant, type command “make”

To run the program, 
Always execute “sudo ./stop_system.sh” first
Then “sudo ./run_system.sh”

To restart a failed node,
Go to penn-cloud/storage-system/server, type command “./slave [master address] [slave address] [replication address]" (e.g. ./slave 127.0.0.1:50051 127.0.0.1:10001 127.0.0.1:10001 )
