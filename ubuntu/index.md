# Octet Nest Linux Package Repository
This is the Octet Nest Linux Package Repository. To add this repository to your computer, simply run the following command :

``echo "deb https://octetnest.github.io/ubuntu xenial/" |sudo tee --append /etc/apt/sources.list.d/octetnest.list && sudo apt-get update`` 

# Packages

### openconnectutils (ubuntu 16.04)
This package makes it easy for you to connect to a Cisco VPN withouth the hassle of using browser plugins or the proprietary Linux VPN client offered by Cisco. The package installs the required packages necessary to establish a VPN connection through the Ubuntu Network Manager.

  - Run ``apt-get install -f openconnectutils``
  - At the top right corner on your computer, click on the **Network Manager** > **Edit Connections...**
  - A new dialog appears, click on **Add**
  - You now need to choose a connection type. Choose **Cisco AnyConnect Compatible VPN** followed by **Create**
  - A new dialog appears. Enter a **Connection Name**, the VPN hostname in **Gateway**, ensure that **Allow Cisco Secure Desktop trojan** is _selected_, enter _/usr/share/openconnectutils/csd-init.sh_ for **CSD Wrapper Script** and select _RSA SecurID - manually entered_ for **Token Mode**. Finish by clicking **Save**.

You are now ready to establish a VPN connection. Click on the **Network Manager** icon followed by **VPN Connections** and choose the VPN connection you'd like to establish. A new dialog then appears. Click on **Connect**.
