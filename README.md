# Çalışma alanı oluşturma

------------------------------

# Not

'=>' şeklinde yazılan kodlar terminale girilecektir.

'--' şeklinde yazılan yazılar girilen kodun terminaldeki çıktısıdır.

örn:

=> print("ahmed")

-- ahmed

------------------------------

# Yeni Ortamı oluşturma

=> export ML_PATH="$HOME/ml"

isterseniz yolu değiştirebilirsiniz

=> mkdir -p $ML_PATH

pip sürümünü güncelleyin

=> pip3 install --upgrade pip

-- Collecting pip
[...]
Successfully installed pip-9.0.1

=> pip3 install --user --upgrade virtualenv  # izole bir ortam oluşturmak için pip komutunu çalıştırarak virtualenv'i yükledik

-- Collecting virtualenv
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

ortama eriştiğinizde komut satırınız " (env) demir@demir:~$  " şeklinde gözükecektir. başına (env) gelecek.

------------------------------

# Ortama yeni kütüphaneler kurmak

=> pip3 install jupyter

-- Collecting jupyter
Downloading jupyter-1.0.0-py2.py3-none-any.whl
[...]

jupyter, numpy, pandas, keras, pyqt5 gibi gibi kütüphaneleri kurabilirsiniz.

ve her yükleme sonunda kütüphaneleri ortama dahil etmelisiniz:

=> python3 -c "import jupyter, matplotlib, numpy, pandas, scipy, sklearn"

------------------------------

Bu şekilde sanal çalışma alanı oluşturarak daha verimli makine öğrenmesi projeleri yazabilirsiniz,
ve herhangi bir şekilde çakışan, hata veren kütüphaneleriniz varsa bu ortamda test ediniz.
