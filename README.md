<p style="font-size:14px" align="right">
<a href="https://t.me/IndonesiaAirdropZ" target="_blank">Join our telegram <img src="https://user-images.githubusercontent.com/50621007/183283867-56b4d69f-bc6e-4939-b00a-72aa019d1aea.png" width="30"/></a>
</p>

<h1 align=center><img src="https://assets-global.website-files.com/5e990b3bae81cf4a03433c58/5f347d008da2e477a3c61fca_Aleo-logo-white-p-500.png" width="250"><br>Testnet Tutorial</h1>

## Prepare
1. Hardware Requirement
  <table>
    <tr>
      <th>Component
      <th>Specifications
    </tr>
    <tr>
      <td>CPU	
      <td>Intel Core i3 or i5
    </tr>
    <tr>
      <td>RAM	
      <td>At least 4GB/8GB of memory (RAM)
    </tr>
    <tr>
      <td>Storage
      <td>At least 200GB of SSD disk storage
    </tr>
    <tr>
      <td>Connection
      <td>At least 100mbps network bandwidth
    </tr>
  </table>
  
 2. Recommendation VPS
<table>
    <tr>
      <th>Provider
      <th>Link
    </tr>
    <tr>
      <td>Contabo	
      <td>https://contabo.com/en/vps/
    </tr>
    <tr>
      <td>IONOS	
      <td>https://www.ionos.com/servers/vps
    </tr>
    <tr>
      <td>Digital Ocean
      <td>https://www.digitalocean.com/
    </tr>
</table>

## Usefull Link
- Join Discord : https://discord.gg/aleohq
- Official Github : https://github.com/AleoHQ/snarkOS
- Aleo Developer : https://developer.aleo.org/testnet/getting_started/overview
- Website : https://www.aleo.org/

## Installation

### Download Package
```
git clone https://github.com/AleoHQ/snarkOS.git --depth 1
```

### Go to folder snarkOS
```
cd snarkOS
```

### Installing snarkOS
```
chmod +x build_ubuntu.sh; ./build_ubuntu.sh
source ~/.bashrc
```

## Running Node

### Create your account
```
snarkos account new
```

> Please copy and save ``Private Key``, ``View Key`` and ``address`` to your note

For Example :
```
 Attention - Remember to store this account private key and view key.

  Private Key  APrivateKey1xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  <-- Save This And Use In The Next Step
     View Key  AViewKey1xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  <-- Save This
      Address  aleo1xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  <-- Save This
```

### Run the node
```
chmod +x run-prover.sh; ./run-prover.sh
```
And then you will be inputted your Private Key

## Troubleshoot
### Why my node can't be compiled?
- Check your VPS or OS must installed ``Rust v1.64``, for installing step by step you can visit <a href="https://www.rust-lang.org/tools/install">this link</a>. 
- If large errors appear during compilation, try running ``cargo clean``.
- Ensure snarkOS is started using ``./run-client.sh`` or ``./run-prover.sh``.

### Why my node can't be connected to peers on the network?
- Ensure ports ``4133/tcp`` and ``3033/tcp`` are open on your router and OS firewall.
- You can use this command for open this port :
```
ufw allow 4133/tcp
ufw allow 3033/tcp
```
- Ensure snarkOS is started using ``./run-client.sh`` or ``./run-prover.sh``.

### Why I can't generate new address?
- Before running the command above (``snarkos account new``) try ``source ~/.bashrc``
- Also double-check the spelling of ``snarkos``. Note the directory is ``/snarkOS``, the command is ``snarkos``






