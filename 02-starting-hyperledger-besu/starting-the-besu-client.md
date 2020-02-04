# Starting the Besu client

Starting the Hyperledger Besu client is as simple as running the command 

```text
./besu
```

but it is important to understand what is happening in the background. This command by  default connects to Ethereum Mainnet and downloads the Ethereum blockchain to a folder called database in the Besu installation directory.

![Directory before starting the Besu client](../.gitbook/assets/besu-directory-before.png)

![Directory after the Besu client has started](../.gitbook/assets/besu-directory-after.png)

Two other files, key and DATABASE\_METADATA.json can also be seen. 

{% hint style="info" %}
To run the ./besu only, you will have to already be in the Besu/besu-1.3.8/bin folder. Otherwise you will have to explicitly state the full path of the besu executable. eg ./Besu/besu-1.3.8/bin/besu

This will be important for the remainder of this book.
{% endhint %}

