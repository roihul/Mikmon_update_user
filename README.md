### MIKHMON V3

#### Download


#### Update 
1. Perbaikan live report.
2. Perbaikan generate users.
3. Penambahan idle tileout (auto logout).
4. Penambahan ping IP Mikrotik di session settings.


	![314](https://raw.githubusercontent.com/laksa19/laksa19.github.io/master/img/3.14.gif)


	``` Monitor Profile adalah scheduler yang mengecek expired user ```

	![indicator](https://raw.githubusercontent.com/laksa19/laksa19.github.io/master/img/profile-indicator.png)



	![delenvironment](https://raw.githubusercontent.com/laksa19/laksa19.github.io/master/img/delenvironment.gif)

	Link Video [Update Profile v3.13 r6](https://drive.google.com/file/d/1ezFG0yxr3LOTgymH_ivUulF8MVevO2-V/view?usp=sharing)

	[https://github.com/laksa19/mikhmonv3/issues/5](https://github.com/laksa19/mikhmonv3/issues/5)

	  
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
