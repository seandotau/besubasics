# Changing the Besu data directory

In this section, we'll learn how to change the data directory that Besu uses to store the blockchain. It is recommended to change the data directory because it allows you to place the potentially very large database folder to a location of your choice. 

As we build our knowledge of common Besu command line flags, here we introduce the [--data-path](https://besu.hyperledger.org/en/stable/Reference/CLI/CLI-Syntax/#data-path) flag which is used to change the location of the database folder and it also allows the folder name to change to something more meaningful.

```text
./besu --network=mainnet --data-path=/database_mainnet --rpc-http-enabled
```

Here, we have changed the database folder name to include a suffix that indicates the network it is connected to which makes it more clear. We have also placed the folder in the root directory but this could easily be anywhere convenient for you.



