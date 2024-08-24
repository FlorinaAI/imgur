# Imgur it ✨

Linux terminalinde Imgur ile resim yükleme, bağlantıları yönetme ve indirme işlemlerini kolaylaştıran bir Python betiğidir. Bu araç, komut satırından basitçe `imgur-it` komutunu kullanarak Imgur işlemlerinizi gerçekleştirmenizi sağlar.
 
## Özellikler 🌸

- Tek bir resmi veya bir klasördeki tüm resimleri Imgur'a yükleyin.
- Yüklenen resimlerin bağlantılarını `links.txt` dosyasına kaydedin.
- Imgur bağlantılarından tekli ya da çoklu resim indirin.
- HTML olarak yükleme özeti oluşturun.
- Python bağımlılıkları ve API anahtarlarını yönetin.

## Kurulum 💖

1. **Projeyi klonlayın:**
   ```bash
   git clone https://github.com/FlorinaAI/imgur-it.git
   ```

2. **Projenin klasörüne gidin:**
   ```bash
   cd imgur-it
   ```

3. **Kurulum betiğini çalıştırın:**
    ```bash
    ./install.sh
    ```
4. **Kurulum sırasında sizden Imgur API anahtarlarınızı girmeniz istenecektir. [Client oluşturun!](https://api.imgur.com/oauth2/addclient)**
   
Kurulum başarıyla tamamlandığında, `imgur-it` komutunu terminalden kullanabilirsiniz.

## Kullanım 🎀

Güncel bilgi için: `imgur-it -h`

1. **Tek bir resim yükleme**

   Belirtilen resim dosyasını Imgur'a yüklemek için:

   ```bash
   imgur-it /path/to/image.png
   ```

2. **Klasördeki tüm resimleri yükleme**

   Belirtilen klasördeki tüm resimleri Imgur'a yüklemek için:

   ```bash
   imgur-it -f /path/to/folder/
   ```

3. **Linkleri .txt dosyasına kaydetme**

   Yüklenen resimlerin bağlantılarını .txt dosyasına kaydetmek için:

   ```bash
   imgur-it -f /path/to/folder/ -w
   ```
   .txt dosyasının konumunu belirtmek için:

   ```bash
   imgur-it -f /path/to/folder/ -w /path/to/txt.txt
   ```

4. **Resim indirme**

   Imgur bağlantısından resim indirmek için:

   ```bash
   imgur-it -i https://i.imgur.com/example.png
   ```
   
   Metin dosyasından Imgur bağlantılarını indirmek için:

   ```bash
   imgur-it -i /path/to/links.txt
   ```
   Örnek `links.txt` dosyası:

   https://i.imgur.com/example.png  
   https://i.imgur.com/exapmle.png  
   https://i.imgur.com/example.png

5. **Yükleme özeti (HTML)**

   Yüklenilen resimlerin özetini HTML dosyası olarak oluşturmak için:

   ```bash
   imgur-it -f /path/to/folder/ -s
   ```  
