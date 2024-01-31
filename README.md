### MIKHMON V3

#### Download update.zip
[update.zip](https://raw.githubusercontent.com/laksa19/laksa19.github.io/master/download/update.zip){:target="_blank"}


#### Update 08-06 2019 V3.17
1. Perbaikan live report.
2. Perbaikan generate users.
3. Penambahan idle tileout (auto logout).
4. Penambahan ping IP Mikrotik di session settings.

#### Update 07-14 2019 V3.16
1. Penambahan address pool di add user profile dan edit user profile
2. Notif new update di admin settings

#### Update 07-02 2019 V3.15
1. Update RouterOS API for support v6.45.x

#### Update 05-09 2019 V3.14
1. Perbaikan time zone untuk print / quick print.
2. Penambahan input comment setelah comment user berubah menjadi tanggal expired.

	![314](https://raw.githubusercontent.com/laksa19/laksa19.github.io/master/img/3.14.gif)

#### Update 04-06 2019 V3.13 r7
1. Perbaikan add user profile (gagal membuat monitor profile di scheduler).
2. Perbaikan edit profile (remove monitor profile untuk expired mode none).
3. Penambahan indikator monitor profile di laman list user profile dan edit user profile (Green = Monitor Profile aktif, Orange = Monitor Profile tidak aktif).

	``` Monitor Profile adalah scheduler yang mengecek expired user ```

	![indicator](https://raw.githubusercontent.com/laksa19/laksa19.github.io/master/img/profile-indicator.png)

#### Update 04-02 2019 V3.13 r6
1. Perbaikan penghitungan tanggal dan jam monitor user profile. 
2. Perubahan global function ke local function. 

	Silakan diupdate kembali user profilenya. (buka user profile dari Mikhmon, simpan kembali masing-masing user profile).

	Setelah update user profile hapus semua environment (system -> scripts -> environment).

	![delenvironment](https://raw.githubusercontent.com/laksa19/laksa19.github.io/master/img/delenvironment.gif)

	Link Video [Update Profile v3.13 r6](https://drive.google.com/file/d/1ezFG0yxr3LOTgymH_ivUulF8MVevO2-V/view?usp=sharing)

#### Update 03-31 2019 V3.13 r5
1. Perbaikan user profile. (user expired dipergantian bulan). Silakan diupdate kembali user profilenya.
	[https://github.com/laksa19/mikhmonv3/issues/5](https://github.com/laksa19/mikhmonv3/issues/5)


#### Update 03-20 2019 V3.13
1. Perbaikan QR Code. Tidak lagi menggunakan Google chart API.
2. Perubahan variable QR Code menjadi <?= $qrcode ?> tanpa tag ```<img>```. 
	  
   ! Perlu penyesuaian untuk template hotspot, ubah 
  ```<img src="<?= $qrcode ?>" >``` menjadi ```<?= $qrcode ?>``` tanpa tag ```<img>```. Bagi yang menggunakan template default bisa reset template default untuk menyesuaikan QR Code.
	  
   Untuk template voucher yang lain bisa menyesuaikan ukuran QR Code dapat menambahkan style sebagai berikut.
   
```html
<style>
  .qrcode{
  height:80px;
  width:80px;
  }
</style>
```

![newqr](https://raw.githubusercontent.com/laksa19/laksa19.github.io/master/img/newqr.gif)
