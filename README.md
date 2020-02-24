# Çalışma alanı oluşturma

------------------------------

# Not

'=>' şeklinde yazılan kodlar terminale girilecektir.

'-' şeklinde yazılan yazılar girilen kodun terminaldeki çıktısıdır.

'#' şeklinde yazılan yazılar yorum satırıdır. açıklama içindir, koda dahil değildir.

örn:

=> print("ahmed")
-ahmed

------------------------------

# Yeni Ortamı oluşturma

=> export ML_PATH="$HOME/ml"  # isterseniz yolu değiştirebilirsiniz

=> mkdir -p $ML_PATH

pip sürümünü güncelleyin

=> pip3 install --upgrade pip

- Collecting pip
[...]
Successfully installed pip-9.0.1

=> pip3 install --user --upgrade virtualenv  # izole bir ortam oluşturmak için pip komutunu çalıştırarak virtualenv'i yükledik

- Collecting virtualenv
[...]
Successfully installed virtualenv

=> cd $ML_PATH

=> virtualenv env

artık ortamı oluşturma işlemi bitti.

------------------------------

# Ortama erişmek

Bu ortamı her etkinleştirmek istediğinizde aşağıdaki komutları kullanacksınız.

=> cd $ML_PATH

=> source env/bin/activate

