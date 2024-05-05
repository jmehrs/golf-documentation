## Official Documentation
- [NATS guide](https://docs.nats.io/)
- [NATS client examples](https://natsbyexample.com/)
## Getting started
You can find the latest release of `nats-server` [here](https://github.com/nats-io/nats-server/releases). or you can use `curl` to download a specific version from the CLI
```
curl -L https://github.com/nats-io/nats-server/releases/download/v2.10.14/nats-server-v2.10.14-linux-amd64.zip -o nats-server.zip
```
Then unzip the contents into a folder called `nats-server`:
```
unzip nats-server.zip -d nats-server
```
You should see similar output as below
```
Archive:  nats-server.zip
   creating: nats-server-v2.10.14-linux-amd64/
  inflating: nats-server-v2.10.14-linux-amd64/README.md
  inflating: nats-server-v2.10.14-linux-amd64/LICENSE
  inflating: nats-server-v2.10.14-linux-amd64/nats-server
```
and finally, copy it to the `bin` folder (this allows you to run the executable from anywhere in the system):
```
sudo cp nats-server/nats-server-v2.10.14-linux-amd64/nats-server /usr/bin
```

## Starting the server
After installing the binary, the server can be run with the following command:
```sh
nats-server
```
which will output something like:
```
[5667] 2024/04/24 07:26:39.569231 [INF] Starting nats-server
[5667] 2024/04/24 07:26:39.569307 [INF]   Version:  2.10.14
[5667] 2024/04/24 07:26:39.569316 [INF]   Git:      [ea48105]
[5667] 2024/04/24 07:26:39.569329 [INF]   Name:     NB63ON2CR2M3IK7WQKM5W2DGZC2G3S4LIZY42AKZPCUG22ICLH5W7KGM
[5667] 2024/04/24 07:26:39.569337 [INF]   ID:       NB63ON2CR2M3IK7WQKM5W2DGZC2G3S4LIZY42AKZPCUG22ICLH5W7KGM
[5667] 2024/04/24 07:26:39.570045 [INF] Listening for client connections on 0.0.0.0:4222
[5667] 2024/04/24 07:26:39.570460 [INF] Server is ready
```
### Add user/password authentication
The `--user` & `--pass` arguments can be added to the command :
```
nats-server --user admin --pass password
```
This will require a username of `admin` and password of `password` to be used by any connecting clients.
### Add remote logging (remote syslog)
The `--remote_syslog` argument can be added to the command with a udp/tcp address following it:
```
nats-server --remote_syslog udp://localhost:1514
```
The server logs will be sent to the specified address.
>Note that you will not see the server logs in the terminal output when running the command with the `--remote_syslog` argument

To test that the server is sending logs to the destination, you can listen to UDP port 514 with the `nc` command:
```
nc -u -l 1514
```
In another terminal, if you start the server (pointing the `--remote_syslog` address to port 1514), you should see logs in the terminal running the `nc` command.
### Using a configuration file
Instead of using command-line arguments to configure the NATS sever, you can specify the location to a config file via the `-c` flag:
```
nats-server -c server.conf
```
The structure of the config file can be found [here](https://docs.nats.io/running-a-nats-service/configuration).