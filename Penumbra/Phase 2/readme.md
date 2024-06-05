![summoning](https://github.com/fatalbar/Contribution/assets/81378817/100a1242-efbc-47e0-8e75-76b38e47564e)


# Doc
* Official Website : https://penumbra.zone/
* Official Guide: https://summoning.penumbra.zone/
* Read About Ceremony: https://penumbra.zone/blog/summoning-ceremony-launch/
* Discord https://discord.gg/cFtxMF7X5J
  
# Register
* Penumbra Penumbra Summoning Phase 2 Attestations will addy soon
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
![Screenshot_6](https://github.com/fatalbar/Contribution/assets/81378817/16d1018d-2d12-40cc-8b3d-22b2229a7eba)

Make a Coffe and wait until your Contribution accepted, 
Dont worry pcli will output your contribution hash after submission complete

i wanna close my screen without Disconnecting with pcli ? well just `CTRL+A+D`
You can check your contribution result

```bash
screen -x penumbra
```

After you hash 
plese input your contribution here (will update it when ready)

# Important
* The minimum bid for this ceremony is 60penumbra.
Once in the queue, you just have to wait until the command completes. Grabe your Coffe with Cat 💕
* Posting your contribution hash publicly allows others to verify that your contribution was included in the transcript!
* Reconnecting and Rebidding
 To change your bid, you can simply run the command again with a different bid amount. Note that each time you bid with the command above, this adds additional funds to all of the previous bids you've already submitted.
If you get disconnected for some reason, you can simply bid 0penumbra and recover your position in the queue, since all of your previous bids have been recorded.

Thank you




