Aleo is a new layer-1 blockchain platform for creating scalable and private applications applying zero-knowledge cryptography. Aleo uses a hybrid consensus architecture named AleoBFT, which leverages PoS to achieve instant finality for block confirmation, and leverages PoW “coinbase puzzle” that rewards the development of faster techniques for proof generation.

Mining rewards will be settled daily as credits, according to the payout scheme of PPLNS, and then accrue in your f2pool account. Adding wallets and reward withdrawals are currently not supported, we will send payouts according to Aleo’s follow-up post about the details of the incentives. Please stay tuned for our further announcement.

Please kindly note that, in order to receive incentivized testnet rewards, a KYC process is required after launching the mainnet. If f2pool cannot pass through KYC by the Aleo project team, we will not be eligible to receive rewards from the network and thus cannot distribute them to you. Also, we will restrict our services to the regions that are under Aleo official restriction, for more information please check here.

To learn about the requirements and configuration, please refer to the following steps.

Please note:

Aleo is in the Testnet Beta phase. Previous Aleo Testnet 3 mining details can be found on the f2pool website under “ALEO TESTNET3”. Testnet Beta mining information is under “ALEO”.

1. Obtain suitable hardware and software
For hardware:

Mine Aleo with just a CPU, or a CPU and GPU combination.
Best performance with a high-end AMD CPU and a single Nvidia GPU.
Multi-GPU configurations are not supported.
CPUs with more than 24 cores can also be used.
For software:

You need to get the Ubuntu 18.04 or higher operation system ready, and install this mining software (download).

2. Sign up for an f2pool account
You will need to create an f2pool account before mining Aleo on its Testnet Beta. If you do not have one yet, please click here to register.

Setting an account name will be required for configuration. You are free to create multiple subaccounts to monitor your mining machines.

3. Configure mining software
Begin by downloading and extracting the mining software. Next, you will need to execute the commands on Ubuntu.

chmod +x aleo.sh && chmod +x aleo-miner
./aleo.sh stratum+tcp://aleo-asia.f2pool.com:4400 accountname.workername
Before you start:

Ensure to replace accountname with the name of your f2pool account.

Also, you will need to create a customized worker name and assign it to workername.

This workername will function as your miner ID. Feel free to customize it as per your needs. For ease of use, we recommend keeping it within 15 characters, using a combination of lowercase letters or numbers.

If the above command does not start the GPU mining function properly (check with nvidia-smi, if you do not see aleo-miner using the GPU, it means it has not started properly), execute the following commands:

sh

nohup ./aleo-miner -u stratum+tcp://aleo-asia.f2pool.com:4400 -w accountname.workername -d 0 >> ./aleo-miner.log 2>&1 &
Before running, ensure that you customize both the account name and worker name.

If you see the following information in aleo-miner.log about three minutes after executing the above commands, it indicates that the program is running successfully.



To stop mining, execute the following command:

pkill -9 aleo-miner
 
4. Start mining!
Your machines are now ready to mine! You can manage your account settings and monitor your hashrate, rewards and so on in your dashboard or in our f2pool app.

If you run into any problems mining Aleo, please feel free to reach out to our customer service team at support@f2pool.com, open a support ticket, or start a conversation on Reddit.

To stay updated with the latest PoW news and developments, follow us on Twitter!

Happy mining!
