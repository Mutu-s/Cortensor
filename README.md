# Cortensor

 > [Discord](https://discord.gg/cortensor)

ETH mainnette 10$  COR Alıp stake etmeniz gerekiyor ve Formu doldurun
https://forms.gle/JX2zpR8dvkiHvjWu5
 > [Form](https://forms.gle/JX2zpR8dvkiHvjWu5)
 > [Uniswap](https://app.uniswap.org/swap)
 >  CA: 0x8e0EeF788350f40255D86DFE8D91ec0AD3a4547F
    
       git clone https://github.com/cortensor/installer
       cd installer
       ./install-docker-ubuntu.sh
       ./install-ipfs-linux.sh
       /root/bin/ipfs version
       ./install-linux.sh

 Şifre girelim . Name girdikten sonra enter hepsine y basalım

      ls -al /usr/local/bin/cortensord
      ls -al /etc/systemd/system/cortensor.service

servis dosyalarımız da tamam şimdi key alalım

    /usr/local/bin/cortensord ~/.cortensor/.env tool gen_key
    
Keyimizi kayıt edelim ve ARB Sepolia gönderelim

    /usr/local/bin/cortensord ~/.cortensor/.env tool register


Daha sonra dc de modu etiketleyerek bu şekilde testnet kanalına  mesaj atalım ![image](https://github.com/user-attachments/assets/5a91cec8-c565-4096-b4cc-0151d63dfade)

WL eklendikten sonra 

    /usr/local/bin/cortensord ~/.cortensor/.env tool verify

Başlat 

    /bin/start-cortensor.sh

Durdurma komutu

    /bin/stop-cortensor.sh

Log Kontrol

    tail -f /var/log/cortensord.log
    ls -alh /var/log/cortensord.log
    
Düğüm Adresini ve Kimliğini Kontrol Edin

    /usr/local/bin/cortensord ~/.cortensor/.env tool id
