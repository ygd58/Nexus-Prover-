# Nexus-Prover
Nexus Prover
**Nexus Prover**; merkeziyetsiz kanıtlayıcı ağına (prover network) bağlanmak için geliştirilen bir betik ve sistem hizmetidir. Bu araç, belirli hesaplama işlemlerini doğrulayan bir sistem olan **Nexus** projesi kapsamında çalışır ve verilerin güvenilirliğini sağlamak amacıyla kullanılabilir. Kullanımı özellikle Ubuntu sistemleri (hem yerel hem de VPS) için optimize edilmiştir.

### **Sistem Gereksinimleri**
- Minimum 4 GB RAM, ancak 6 GB RAM önerilir.
- Ubuntu tabanlı bir sistem veya VPS kullanımı gereklidir.

### **Kurulum Komutları**
Aşağıdaki komutlardan birini kullanarak Nexus Prover'ı kurabilirsiniz:

1. **Curl ile Kurulum:**
   ```bash
   sudo apt install curl && [ -f "nexus.sh" ] && rm nexus.sh; curl -sSL https://raw.githubusercontent.com/zunxbt/nexus-prover/main/nexus.sh | bash
   ```

2. **Wget ile Kurulum:**
   ```bash
   sudo apt install wget && [ -f "nexus.sh" ] && rm nexus.sh; wget -qO - https://raw.githubusercontent.com/zunxbt/nexus-prover/main/nexus.sh | bash
   ```

### **Hizmet Durumunu Kontrol Etme**
Kurulum sonrası hizmetin çalıştığını doğrulamak için şu komutu kullanabilirsiniz:
```bash
systemctl status nexus.service
```

Logları görüntülemek için:
```bash
journalctl -u nexus.service -f -n 50
```

### **Web Tarayıcısı ile Entegrasyon**
Web tarayıcınızdan Nexus Prover kimliğinizi CLI ile eşleştirmek için şu adrese gidin: [Nexus Beta Sitesi](https://beta.nexus.xyz/) ve profil bölümünden kimliğinizi alın.

Daha fazla detay ve güncellemeler için [Nexus Prover GitHub Sayfası](https://github.com/zunxbt/nexus-prover) adresine göz atabilirsiniz.
