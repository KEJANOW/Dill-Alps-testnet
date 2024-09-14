![image](https://github.com/user-attachments/assets/94e0ba96-7db4-44db-88b3-577651358207)

------
# Light Validatör Donanım Gereksinimleri
| Donanım | Gereksinimleri |
| ------------- | ---------------- |
Cpu | 2 Cores
Architecture | x86-64 (x64, x86_64, AMD64, ve Intel 64)
Memory | 2 GB
Operating System | Ubuntu 22.04.2 LTS or higher versions (x86-64)
Storage | 20 GB
Network Bandwidth | 1MB/s 

# Full Validator Donanım Gereksinimleri
| Donanım | Gereksinimleri |
| ------------- | ---------------- |
Cpu | 4 Cores
Architecture | x86-64 (x64, x86_64, AMD64, ve Intel 64)
Memory | 8 GB
Operating System | Ubuntu 22.04.2 LTS or higher versions (x86-64)
Storage | 256 GB
Network Bandwidth | 64Mb/s 

# Dill Public Testnet (Alps Testnet) Bilgileri
| Network Name     | Dill Testnet Alps |
| ------------- | ---------------- |
Ağ Adı | Alps Testnet
Rpc URL | https://rpc-andes.dill.xyz/
Chain ID | 102125
Currency Symbol | DILL
Explorer URL | https://andes.dill.xyz/


## Kurulum Talimatları

- İlk olarak terminali açın. Daha sonra aşağıdaki kodu çalıştırın. Dosyaların inmesini bekleyin.

```
curl -sO https://raw.githubusercontent.com/DillLabs/launch-dill-node/main/dill.sh  && chmod +x dill.sh && ./dill.sh
```
- Dosyalar indikten sonra "Step 1 Completed. Press any key to continue..." çıktsını aldıktan sonra herhangi bir tuşa basın ve devam edin.
- Yeni bir mnemonic oluşturacaksınız 1'i seçin yada mevcut mnemonic'lerinizi kullanacaksınız 2'yi seçerek enter'a basın. Kelimelerinizi kaydetmeyi unutmayın. Ayrıca oluşan kelimelerini dill/validator_keys/mnemonic-xxxxxx.txt dizininde bu dosyada görebilirsiniz. (bu dosyayı yedekleyemeyi kesinlikle unutmayın. Eğer node'nuzu başka bir sunucuya taşımak isterseniz bu lazım olacak.)
- Kelimeleriniz oluştuktan sonra random olarak Validator Keystore şifrenizi oluşturulacak. Bunu da kaydedin. Gene aynı şekilde random oluşan şifrenizi dill/validator_keys/keystore_password.txt dosyasında görebilirsiniz. Tekrar herhangi bir tuşa basın. 
- "Step 2 Completed. Press any key to continue..." çıktısını alınca tekrar herhangi bir tuşa basın ve kuruluma devam edin.
- En sonda "node running, congratulations" çıktısı validator_pubkeyinizi ve alacaksınız ve kurulum tamamlanacak.

## Staking

Not: Node'unuz sync olduktan sonra staking işlemlerini yapmanız tavsiye edilir. Sync kodunu reponun en altına ekledim. Kontrol edebilirsiniz.

  - Öncelikle, Alps kanalından faucet'ten token talep edin. Node'da oluşturduğunuzdan farklı bir cüzdan kullanın ve faucet'i yalnızca bir kez alabileceğinizi unutmayın ($request xxxxx).
  - https://staking.dill.xyz/ adresini ziyaret edin.

![image](https://github.com/user-attachments/assets/3c24ea5d-c728-4ee7-87f3-b2a42abd5dd5)

- Bu siteye deposit_data-xxxxx.json dosyanızı yükleyeceksiniz. Bu dosyayı sunucunuzun içinde /dill/validator_keys dizininden bulup alabilirsiniz.(WinSCP, Mobaxterm gibi uygulamarı kullanabilirsiniz.)
- Deposit_data-xxxx.json dosyasını siteye yükledikten sonra MetaMask'a Bağlan'a tıklayın, yeterli test tokeniniz olduğundan emin olun (>3600 DILL)

 ![image](https://github.com/user-attachments/assets/f8238c5a-b216-476c-a5a3-18fc919211b6)

- Cüzdanı bağladıktan sonra Continue'ya basarak devam edin. Ardından Confirm deposit'e basarak depositini gerçekleştirin.

![image](https://github.com/user-attachments/assets/5b8c045f-6cf8-49e8-a096-d047e940e71f)



























