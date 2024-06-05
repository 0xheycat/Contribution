![summoning](https://github.com/fatalbar/Contribution/assets/81378817/100a1242-efbc-47e0-8e75-76b38e47564e)


# Doc
* Official Website : https://penumbra.zone/
* Official Guide: https://summoning.penumbra.zone/
* Read About Ceremony: https://penumbra.zone/blog/summoning-ceremony-launch/
* Discord https://discord.gg/cFtxMF7X5J
  
# Register
* Penumbra Penumbra Summoning Phase 2 Attestations https://form.asana.com/?k=THhk7qmp3IDwCvXWTPHkow&d=1206052071402903
# Preq

```bash
sudo apt update && sudo apt upgrade -y
sudo apt-get install git screen curl build-essential pkg-config libssl-dev clang git-lfs -y
```

### Installing pcli

```bash
mkdir penumbra
cd penumbra
```

```bash
curl --proto '=https' --tlsv1.2 -LsSf https://github.com/penumbra-zone/penumbra/releases/download/v0.77.2/pcli-installer.sh | sh
```
```bash
sudo mv /root/.cargo/bin/pcli /usr/local/bin/
```


https://github.com/fatalbar/Contribution/assets/81378817/4d3d44eb-5291-42be-898c-da392bd18c20

### Jump to 1:25 minutes in the video guide to see how to move the package

![Screenshot_1](https://github.com/fatalbar/Contribution/assets/81378817/f69b249c-3aa3-41b2-9982-698d06a24551)

 Confirm the pcli binary is installed by running:
```bash
pcli --version
```

![Screenshot_2](https://github.com/fatalbar/Contribution/assets/81378817/f370362a-a430-4764-a942-87fa5ae677d5)

### Wallet
1. Create new wallet
Make sure you Backup your Seed on safe place
 ```bash
pcli init soft-kms generate
```
2. Import existing wallet (Optional)
 ```bash
pcli init soft-kms import-phrase
 ```
3. Check Address
```bash
pcli view address
```

### 🚨Troubleshooting  If you encounter an error while importing your wallet, you need to remove the config.toml file located at /root/.local/share/pcli/config.toml

https://github.com/fatalbar/Contribution/assets/81378817/672ee20b-3850-4715-b166-99e49f79690d


### Jump to 1:22 - 1:58 minutes in the video guide to see how to remove the config.toml file.

1. delete old pharse/move other place
```bash
rm -rf /root/.local/share/pcli/config.toml
```
2. check config.toml if already deleted
```bash
cat /root/.local/share/pcli/config.toml
```

#Import old pharse 

### Jump to 1:59 - 02:09 minutes in the video guide to see how to import old pharse


1. use this command to start import old pharse

```bash
pcli init soft-kms import-phrase
```

2. enter your old phrase then hit ENTER



![Screenshot_4](https://github.com/fatalbar/Contribution/assets/81378817/2ec4407f-8195-4f83-aa65-ca2e5abf7d9d)


4. Fauchet 
paste your Address on Doscord

![Screenshot_3](https://github.com/fatalbar/Contribution/assets/81378817/5b6e3abe-bd64-4edc-9c0a-d2dbb7822acc)

5. Check Balance
```bash
pcli view balance
```
![Screenshot_5](https://github.com/fatalbar/Contribution/assets/81378817/b4912e1e-85a5-4b4b-a353-c9a0411aee05)


# Contribution 
OK lets fun part 
1. Screen  
```bash
screen -S penumbra
```
2. Start contribution minimal contribution Bid is 60, you can contribute with min BID or below BID (Recommended 60 Bid)
* Dont change Coordinator-address with your wallet
```bash
pcli ceremony contribute --phase 2 --bid 60penumbra

```


https://github.com/fatalbar/Contribution/assets/81378817/4ddd9af9-9ed4-4379-9653-eecb6132da8d


![Screenshot_6](https://github.com/fatalbar/Contribution/assets/81378817/16d1018d-2d12-40cc-8b3d-22b2229a7eba)

Make a coffee and wait until your contribution is accepted. Don't worry, PCLI will output your contribution hash after submission is complete.

If you want to close your screen without disconnecting from PCLI, simply use CTRL+A+D. You can check your contribution result by using

```bash
screen -x penumbra
```

After you receive your hash, please input your contribution here (will update when ready).

Important:
- The minimum bid for this ceremony is 60 penumbra. Once in the queue, you just have to wait until the command completes. Grab your coffee with Cat 💕
Posting your contribution hash publicly allows others to verify that your contribution was included in the transcript!

- Reconnecting and Rebidding:
To change your bid, you can simply run the command again with a different bid amount. Note that each time you bid with the command above, this adds additional funds to all of the previous bids you've already submitted.
- If you get disconnected for some reason, you can simply bid 0 penumbra and recover your position in the queue, since all of your previous bids have been recorded.
Thank you.


twitter thread 
https://x.com/0xheycat/status/1798268660462797012




