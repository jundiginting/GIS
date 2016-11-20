# Penggunaan Data Geospasial
	Dalam Sistem Informasi Geografis, masih banyak dianara kita yang belum mengetahui cara penggunaan dari data – data geospasial. Oleh karena itu pada itu pada pertemuan ini menjelaskan bagaimana cara membuat data geospasial dengan import shapefile dan memasukkan variable nya dengan menggunakan bahasa pemrograman phyton dan juga cara penggunaan class dan method pada python.
# Membuat Data Geospasial
1.	Lakukan Import shapefile
2.	Masukan variable, misalkan variable a untuk shapefile.writer( )
  a = shapefile.writer( )
  Jadi, format membuat data geospasial ada 2, yaitu :
1.	.shp => a.point(x,y)
	a.poly [(x,y),(v,w)]
2.	.dbf => a.field (‘name.field’,’c’,’40’)
	a.record (‘bdg’)
Data geospasial tersebut disimpan menggunakan method a.save(‘file.shp’).

Arti dari method pada writer :

-	Point (x,y)		: memasukkan data berbentuk paint ke dalam .shp dan seluruh data harus berformat ESRI.1
-	Poly [(a,b),(c,d)]	: memasukkan data geospasial berbentuk polygon (kembali ke titik awal) atau polyline (tidak kembali ketitik awal).
-	Field (‘nama’,’c’,’40’): artinya membuat atribut polygon dengan table ‘nama’ dengan tipe data varchar dengan panjang 40. Method ini dapat diulang dan dapat dilakukan untuk krbuthan field baru lagi.
-	Record (‘Bandung’)	: Mengisi table yang hanya satu field dengan value ‘Bandung’.
-	Save (‘nama.file’)	: menyimpan file dengan save file.
	
	Kesimpulan dari pertemuan ke5 ini adalah Dengan mendapatkan data shp kita juga belum tentu kita dapat melihat data tersebut namun kita juga harus menggunakan aplikasi sepert Qgis dan Python.

